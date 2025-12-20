Docker is used mainly in the space for developing, shipping, testing, and running applications through isolated environments called containers.

Containers are:
* isolated, doesn't rely on what is on the host computer
* can be run simultaneously
* has everything that is used to run an application
* can be shared

Docker is great for Continuous integration and continous delievery workflows (CI/CD)
* develop code locally on an exact reannactment of the server system
* run automated and manual tests in a test environment every push
* easily push the environment used for bugfixing to live systems


## Architecture
client-server architecture. Either with docker client and docker daemon
![[Pasted image 20250122205557.png]]
The daemon takes images, builds, runs and distributed into shippable containers. These images can be built from scratch or come as part of a registry of other images, extensions, and plugins

**Docker Daemon (dockerd)**: listens to docker api requests and manages Docker objects such as images, containers, networks, and volumes. A daemon can also communicate with other daemons to manage Docker services.

**Docker client (docker)**: how the user ussually interacts with the daemon(s).

**Docker desktop**: GUI version of the client, daemon, compose, and other stuff.

**Docker registeries**: stores docker images. **Docker hub** is a public registry for loading images. Pulling and pushing comes from the configuration files specified for the configuration registry

Images: read-only templates 
 