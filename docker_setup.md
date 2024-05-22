---
layout: default
#title: "Setup and Installation"
#description: Setup and installation of a Plummrs workspace
permalink: "/docker_setup"
---

## Use production image of Plummrs

Coming up! I'll upload an image soon. For now, you can build locally
the development image.

### Build development image

1. Clone the docker repository:
   ```
   git clone git@github.com:traclabs/plummrs_docker.git
   cd plummrs_docker
   ```
2. Pull the plummrs code:
   ```
   ./clone_plum.sh
   ```
3. Build the image:
   ```
   ./docker_build.sh
   ```
   This will take a while.
   
[back](./)
