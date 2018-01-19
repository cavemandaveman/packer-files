# base-centos7-x86_64
Base CentOS 7 install from minimal ISO.

References the Kickstart file [here](https://gist.github.com/cavemandaveman/3eec19420edd3011db119587eed91ae5)

Creates a VM with 2 CPU, 1 GB memory, 20 GB disk (LVM partitioned).

Pass in the `admin` password on build, like so:
```
packer build -var "user_pw=PASSWORD" base-centos7-x86_64.json
```