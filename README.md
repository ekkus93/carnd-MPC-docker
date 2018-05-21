# carnd-MPC-docker
# docker container for mpc

I was having problems with the ipopt version for the Mac so I created this docker container to get around that.

## Requirements

If you don't have docker installed, go here to install docker:
```
https://www.docker.com/community-edition
```

## To Run

Here's the command to run the docker container:
```
docker run -it -v {{ your CarND-MPC-Project dir }}:/home/ubuntu/work -p 4567:4567 ekkus93/carnd-mpc bash
```

Replace "{{ your CarND-MPC-Project dir }}" with the directory of your project's repo.  Here's an example:
```
docker run -it -v /Users/phillipcchin/work/carnd/CarND-MPC-Project:/home/ubuntu/work -p 4567:4567 ekkus93/carnd-mpc bash
```

(It's easier if your repo directory is in your home directory otherwise you might have to give docker permissions to mount it.)

Once the docker container is running, you should be logged in as the ubuntu user and your current directory will be your project's repo directory.





