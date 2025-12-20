
# Control Operators
## boolean operators
cmd1 && cmd2 = run cmd2 if cmd1 succeeds
cmd1 || cmd2 = run cmd2 if cmd1 fails

## boolean operators instead of if-statements
common bashism is for the use case of using boolean operators instead of if statements:

# consider you want to authenticate that an can delete their account

`prompt_username && get_password && comfirm_delete || exit`
Here we will progress through steps for account deletion, and at any point it fails, we exit from the sequence.
To write this with bash statements requires a lot of if-statements.

## other commands
cmd1 ; cmd2 = run cmd1 and cmd2 sequentially
cmd & = have previous command run in the background 
cmd1 | cmd2 = redirects the stdout from cmd1 to cmd2



# Replacement:
$(cmd) = replace with the command
$((cmd)), $((2+5)) = perform arithmetic


# Background
```bash
# [1] is the job number, and 784695 is the pid
$ sleep 20 &
[1] 784695
# using `jobs`, we can view the commands that are ran in the background
$ jobs
[1]+  Running                 sleep 20 &
# after the 20 seconds, job is done
$ jobs
[1]+  Done                    sleep 20


# if we want to do things with the pid, ie kill the process, we can do so
$ kill %1 # kills base on job name, effectively the same as pid
[1]+  Terminated              sleep 20

# note this works because kill is a shell builtin, and a not a shell instance
$ type -a kill 
kill is a shell command
kill is /bin/kill
$ /bin/kill %1 # fails
kill: illegal process id: %1

# For the last job, you can use %%
$ kill %% 
[1]+  Terminated              sleep 20
```

# Temporary files

Consider the commond workflow of needing to chain commands. We typically store temporary files that we do not care about.
Consider file1 and file2, where file2 is a reordering of file1.
If we want to compare these files, we would need to do:
```bash
sort file1 file1_temp
sort file1 file2_temp
diff file1_temp file2_temp
```
Since we do not care about those files, we can make a short form of this:
```bash
diff <(sort file1) <(sort file2)
```
**Why would you want to do this? This will read and write, instead of read and write, then read and write again, which is far quicker**
This is also faster than pipeine for this exact reason.

**How does this work?**
Process subsitution
`(cmd)` treats cmd as a file.

If we do this in reverse:
```bash
$ ls -l >(cat)
l-wx------ 1 johnzhou johnzhou 64 Dec 17 01:24 /dev/fd/63 -> 'pipe:[2745387]'
```
/dev/fd/63 is a temorary, writable file that when written to, sends to cat stdin, it will then be cat'ed out to stdout

**More examples**
this can be useful for logging.
```bash
example > >(less) 2> >(tee errors.txt) 
```
assuming example will output output and errors, we will send out stdout to less and tee errors to errors.txt.

another example is uncompressing files over ssh without unarchiving it locally:
Suppose you want to backup data inside of directory over 2 different servers. You will archive the local version, send that over to the servers, and then they will unarchive it.
```bash
tar cf - directory | tee >(ssh server1 tar xf -) >(ssh dietpi@10.0.0.88 tar xf -) > /dev/null
```
because of `> /dev/null`, we expect nothing for our local drive.

Using 
```bash
$ nvim <(cat file1 file2) # this is an actual temporary file that you can edit and then save 
$ cat file1 file2 | nvim # you can view the catted files here, but to save you would need to make a new file
```


# SSH 

ssh dietpi@10.0.0.88

If you don't want to enter in a password everytime:
```bash
ssh-keygen
ssh-copy-id dietpi@10.0.0.88
ssh dietpi@10.0.0.88
```

# alternatively


```



# References:
[Understanding `bg` and `&` to background jobs in Bash - You Suck at Programming #050](https://www.youtube.com/watch?v=IhT5QSTCPps)
* background and bg.

[extremely cool shell trick I did not know about - Bread and Penguins](https://www.youtube.com/watch?v=2A4bs40scSo)
* temporary files with `<(cmd)`
