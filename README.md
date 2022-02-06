# dnsmasq-in-kubernetes

This is to deploy DNS service in k3s cluster.

The dnsmasq container image is stored in hub.docker.com. YML file is provided for deployment. 

To make easy to change configuration, design to store the setting/configuration files in NFS. Three files MUST be presented in the mount point

file:hosts
file:dnsmasq.conf
file:resolv.conf

Example of the files is given. 

1. hosts file to store the DNS record
2. dnsmasq.conf is the configuration file of dnmasq
3. resolv.conf records the DNS forwarder IP adddress


hub.docker.com URL:
https://hub.docker.com/r/cwalterhk/dnsmasq

