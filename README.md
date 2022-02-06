# dnsmasq-in-kubernetes

This is to deploy DNS service in k3s cluster.

The dnsmasq container image is stored in hub.docker.com. YML file is provided for deployment. 

To make easy to change configuration, design to store the setting/configuration files in NFS. Three files MUST be presented in the mount point

1. file:hosts
2. file:dnsmasq.conf
3. file:resolv.conf

Example of the files is given. 

1. hosts file to store the DNS records. Edit the file accordingly.
2. dnsmasq.conf is the configuration file of dnmasq.  Change your setting accordingly.
3. resolv.conf records the DNS forwarder IP adddress


hub.docker.com URL:
https://hub.docker.com/r/cwalterhk/dnsmasq

