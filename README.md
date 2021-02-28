Sample packer setup to build a centos/ubuntu container running nginx

To build (default distro=ubuntu):
`$ sudo packer build packer-nginx.json`

To build with centos:
`$ sudo packer -var 'distro=centos' build packer-nginx.json`

To run with ubuntu:
`$ sudo docker run -v /tmp/html:/html -p 8888:80 austin987/nginx-ubuntu:latest`

To run with centos:
`$ sudo docker run -v /tmp/html:/html -p 8888:80 austin987/nginx-centos:latest`
