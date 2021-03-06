---
layout: blog_section 
title: Download
permalink: /download/
---


## Download

Choose which version of CloudRouter you need from the following formats. For more information, please see the [Getting Started](http://www.cloudrouter.org/getting-started/) page. 

### Virtual Images

#### Minimal 

The minimal image is a Fedora Remix with the CloudRouter repository pre-configured. Use this image if you don't want all of the pre-installed packages provided by the full install. 

* [x86_64 Minimal Image (raw)](https://repo.cloudrouter.org/fedora/2/images/CloudRouter-2.0-BETA-fedora-minimal.raw.xz)
* [x86_64 Minimal Image (vmdk)](https://repo.cloudrouter.org/fedora/2/images/CloudRouter-2.0-BETA-fedora-minimal.vmdk)
* [Image Checksum](https://repo.cloudrouter.org/fedora/2/images/CloudRouter-2.0-BETA-fedora-minimal.checksum.txt) 
* [Manifest](https://repo.cloudrouter.org/fedora/2/images/CloudRouter-2.0-BETA-fedora-minimal.manifest) 

#### Full

The full image is also a Fedora Remix with the CloudRouter repository pre-configured. In addition, it includes the following packages:

* [BIRD](http://bird.network.cz/)
* [Quagga](http://www.nongnu.org/quagga/)
* [OpenDaylight Lithium](http://www.opendaylight.org/) 
* [Capstan](https://github.com/cloudius-systems/capstan/blob/master/README.md)
* [Mininet](http://mininet.org/)
* [ONOS](http://onosproject.org/)

Use this image if you're unsure of which packages you might need for your setup. This is also suitable for live USB and CD images. 

* [x86_64 Image (raw)](https://repo.cloudrouter.org/fedora/2/images/CloudRouter-2.0-BETA-fedora-full.raw.xz)
* [x86_64 Image (vmdk)](https://repo.cloudrouter.org/fedora/2/images/CloudRouter-2.0-BETA-fedora-full.vmdk)
* [Image Checksum](https://repo.cloudrouter.org/fedora/2/images/CloudRouter-2.0-BETA-fedora-full.checksum.txt)
* [Manifest](https://repo.cloudrouter.org/fedora/2/images/CloudRouter-2.0-BETA-fedora-full.manifest)

### Docker

A set of containerized CloudRouter images is also available. To run a CloudRouter container: 

* Search for CloudRouter public images on the Docker registry by running the following command: 

`sudo docker search cloudrouter` 

* Choose which container you want based on the application you'd like to use. This example uses [BIRD](http://bird.network.cz/. Pull the image from the registry:

`sudo docker pull cloudrouter/bird-fedora` 

* Run the docker image: 

`sudo docker run cloudrouter/bird-fedora` 

### CD/DVD Images

Use these images for removable media such as USB sticks or CDs/DVDs. 

#### Live CD

* [CloudRouter live CD image](https://repo.cloudrouter.org/fedora/2/images/CloudRouter-Live-2.0-BETA-fedora.iso)

#### Live DVD

* [CloudRouter live DVD image](https://repo.cloudrouter.org/fedora/2/images/CloudRouter-DVD-x86_64-2.iso)

### Amazon EC2

These images are pre-formatted Hardware Virtual Machine Amazon Machine Images (HVM AMIs). 

* [ap-southeast-2 :: (*ami-fdd392c7*)](https://console.aws.amazon.com/ec2/v2/home?region=ap-southeast-2#LaunchInstanceWizard:ami=ami-fdd392c7)
* [us-west-2 :: (*ami-01a5aa31*)](https://console.aws.amazon.com/ec2/v2/home?region=us-west-2#LaunchInstanceWizard:ami=ami-01a5aa31) 

### OSv Images

CloudRouter is working on developing OSv images. _Note: this image is for CloudRouter version 1.0._

[CloudRouter OpenDaylight OSv image](https://repo.cloudrouter.org/repo/beta/images/CloudRouter-Beta-OSv-OpenDaylight-20150320.qemu.xz)

### Metadata ISO image 

For enhanced security, CloudRouter images ship without any default credentials. A default user called **cloudrouter** is provided, but no password is set. To generate a user profile and set a password, you need to create a metadata ISO. An ISO is a file that emulates a CD. Download or generate the ISO then attach it to the CloudRouter virtual machine (much like you would place a physical CD into a CD disk drive on your computer). 

If you're only testing CloudRouter, you can use the pre-generated metadata ISO we've provided. 

[Metadata ISO](https://repo.cloudrouter.org/fedora/2/images/cloudrouter-init.iso)
