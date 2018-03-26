
### General

This Vagrant file spinns up an infrastructure dependencies for developer environment such as:
 * Nomad (NAT to localhost and available over private network as node)
 * Consul (NAT to localhost)

In order to run specific versions feel free to change `BASE_IMAGE`, `NOMAD_VERSION` and `CONSUL_VERSION` variables.
In case you need to have nomad node to be available on specific IP, change `VM_HOSTONLY_STATIC_IP` var.

### Prerequirements
You should have installed Vagrant and any of VM provider (VirtualBox 5.2+ as recommended) 

### Usage

Just run in current folder the following:

`$ vagrant up`

It will build the VM and run NOMAD and CONSUL processes reporting logs with corresponding prefixes.