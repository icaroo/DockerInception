# DockerInception
run docker within docker


Just save that content to a file called Dockerfile within an empty directory,
navigate to that directory and run
# Build
docker build .

Then when the image is built, all you have to do is make sure to run it with the  --priviledged flag. 
E.g.
# Run in the background
docker run -d --privileged [image ID]

# run in interactive mode
docker run -it --privileged [image ID] /bin/bash
