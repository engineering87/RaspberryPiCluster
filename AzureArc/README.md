The azure-cli deb package does not support ARM64 architecture, so we need to user **Docker** as a workaround.

# Docker install

```sudo apt-get install apt-transport-https ca-certificates software-properties-common -y```

```curl -fsSL get.docker.com -o get-docker.sh && sh get-docker.sh```

```sudo usermod -aG docker pi```

```sudo curl https://download.docker.com/linux/raspbian/gpg```

```sudo curl https://download.docker.com/linux/raspbian/gpg```

```nano /etc/apt/sources.list```

Add the following line and save:   

```deb https://download.docker.com/linux/raspbian/ stretch stable```

```sudo apt-get update```

```sudo apt-get upgrade```

# Azure cli

```sudo docker run -it --rm --platform linux/arm64 debian:bullseye```
