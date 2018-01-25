# centos7-docker
Base CentOS 7 with Docker.

References the Kickstart file [here](https://gist.github.com/cavemandaveman/3eec19420edd3011db119587eed91ae5)

Creates a VM with 2 CPU, 1 GB memory, 20 GB system disk (LVM partitioned), 20 GB Docker disk (direct-lvm devicemapper).

Pass in the `admin` password on build, like so:
```
packer build -var "user_pw=PASSWORD" centos7-docker.json
```