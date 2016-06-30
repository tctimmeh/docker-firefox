# Docker-Firefox

Docker images for specific versions of firefox that won't auto-update.

Run like this:

    docker run --name firefox -v /tmp/.X11-unix:/tmp/.X11-unix -e DISPLAY=$DISPLAY tctimmeh/firefox

Note that you may need permit your X server to accept connections from the container. Try this:

    xhost local:root

