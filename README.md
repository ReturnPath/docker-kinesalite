# Overview

This image contains a copy of Kinesalite on Alpine.
Kinsalite is an AWS Kinesis emulator written by Michael Hart.

Kinesalite can be found here: https://github.com/mhart/kinesalite.

# How-to/usage

Kinsalite is the entrypoint so you simply need to run the container: Any options you pass in after the image will be passed directly to kinsalite.

To run kinsalite as a daemon, mapping `localhost:4567` to the kinsalite port in the container run:

  docker run -d -p 4567:4567 returnpath/docker-kinsalite:latest

If you want to run a specific version of kinsalite you can replace `latest` with the actual version number (the tags on the git repo are the available image tags).

