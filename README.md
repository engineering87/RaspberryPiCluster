# Raspberry Pi Cluster
Reference repository for testing a Raspberry Pi cluster, it contains information on the construction, scripts and analysis of the results obtained.

<img src="https://github.com/engineering87/RaspberryPiCluster/blob/main/img/cluster001.jpg" width="500">

### Purpose of the project
The aim of the project is to create a cluster based on Raspberri Pi to experiment with different uses, such as Kubernetes configurations, distributed algorithm and blockchain testing.

### Why Raspberry Pi?
The idea of using different Raspberry Pi to create the cluster is because it allows you to easily simulate scenarios with different machines and different cores.
It's slightly more cost-effective and usually more power-efficient to build or buy a small NUC machine that has more raw CPU performance, more RAM, a fast SSD, and more expansion capabilities.

### Hardware configuration
The cluster is made up of 4 Raspberry Pi connected through a 10/100/1000 Mbps switch. Below is the detail of the 4 Raspberry Pi:
* 1xRaspberry Pi 4 Model B 4GB ARM-Cortex-A72 4X 1,50 GHz
* 1xRaspberry Pi 3 Model B 1GB CPU 1.2 GHz Quad Core
* 1xRaspberry Pi 2 Model B 1GB Quad Core CPU 900 MHz
* 1xRaspberry Pi 1 Model B+ 512MB Broadcom BCM2835 700MHz

The choice of having different versions of the board is due to the need to simulate different scenarios which include non-homogeneous machines with different performances.

### Operating system and configuration
Raspberry Pi OS operating system with Kernel 4 version is installed on all the boards that make up the cluster.
