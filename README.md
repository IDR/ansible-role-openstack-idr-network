Openstack IDR Network
=====================

Create an Openstack network including optional external router for use with the IDR playbooks.


Role Variables
--------------

Defaults: `defaults/main.yml`

Required variables:
- `idr_network_name`: Base name for the IDR network components

Optional variables:
- `idr_network_route_external`: If `True` automatically lookup and connect to an external network, if `False` create an internal router only, default `True`
- `idr_network_subnet`: Subnet CIDR
- `idr_network_subnet_name`: Subnet name
- `idr_network_router_name`: Router name
- `idr_network_dns`: List of DNS servers (default: Google DNS server)


Author Information
------------------

ome-devel@lists.openmicroscopy.org.uk
