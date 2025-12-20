Docker can be used to create environments outside of the host machine, useful for making deployable environments anywhere and at any time.

basic commands:

``` bash
docker  # run docker commands
# Makes a docker image from the specified docker file

docker build -f <docker_file_path> -t <image_name> . 

# Runs a docker image
# -it runs it in an interactice terminal mode
# specifically the i means interactive mode (keep stdin open) and t means to have a pseudo-TTY environemnt (terminal)
# --rm removes the previous version
# -v sets a volume (technically a bind mount, as the values are viewable from host machine and not just the container) 
docker run -it --rm -v <volume_path>:<volume_name_in_container> <name_of_image> 
```

What I run:
```bash
cd ~ && docker build -t my-ros-image . && docker run -it --rm -v /media/johnzhou/SN580:/src my-ros-image
```

Docker image management:
``` bash
# view image
docker image list

# remove an image 
docker rmi -f <IMAGE_ID>
docker image prune # clean up all images
docker system prune # clean up dangling images and containers used by images

```

If you want to get rid of the sudo instances, you need to let yourself be a part of the sudo group and then run the sudodocker command every terminal instance:
```
# sudo usermod -aG docker $johnzhou
# sudo groupadd docker
# sudo gpasswd -a johnzhou docker
alias "sudodocker"="newgrp docker"
```