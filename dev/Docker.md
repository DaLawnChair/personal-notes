Docker can be used to create environments outside of the host machine, useful for making deployable environments anywhere and at any time.

basic commands:

``` bash
sudo docker  # run docker commands
# Makes a docker image from the specified docker file 
sudo docker build -t <name_of_image> <path_to_docker_file>

# Runs a docker image
# -it runs it in an interactice terminal mode
# --rm removes the previous version
# 

sudo docker run -it --rm <name_of_image> 

# 
sudo docker run -it --rm <name_of_image> 


```

What I run:
```bash
cd ~ && sudo docker build -t my-ros-image . && sudo docker run -it --rm -v /media/johnzhou/SN580:/src my-ros-image
```