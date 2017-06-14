Openstack IDR Network
=====================

Create an Openstack network including optional external router for use with the IDR playbooks.


Role Variables
--------------

Defaults: `defaults/main.yml`

Required variables:
- `idr_network_name`: Base name for the IDR network components

Optional variables:
- `idr_network_route_external`: Create an externally-routable network.
   If `auto` (default) automatically lookup the external network.
   If this is a string then route to the external network with this name or id (if you have multiple external networks you must use this to avoid problems).
   If `''` create an internal router only.
- `idr_network_subnet`: Subnet CIDR
- `idr_network_subnet_name`: Subnet name
- `idr_network_router_name`: Router name
- `idr_network_dns`: List of DNS servers (default: Google's DNS servers)


Author Information
------------------

ome-devel@lists.openmicroscopy.org.uk
