############################################################
#
# Update Packages for arm64.
# Additional build dependencies.
#
############################################################
FROM opennetworklinux/builder9:1.6
MAINTAINER Jeffrey Townsend <jeffrey.townsend@bigswitch.com>

RUN apt-get update && apt-get upgrade -y

# Docker shell and other container tools.
#
COPY docker_shell /bin/docker_shell
COPY container-id /bin/container-id
