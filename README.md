# Nutanix-project-1


1.- A network configuration was created for the NTP and DNS services

2.- Two networks were created, one managed for production services (IPAM / DHCP) and one unmanaged for services in development environments

3.- A vlan (vlan-0) was created for production with a range of IP's to manage using the 172.31.0.0/24 network. The IP pool will use a starting address of 172.31.0.210 and an ending address of 172.31.0.230

4.- Vlan (vlan-101) was created for unmanaged development over the 172.31.101.0/24 network

5.- The virtual servers (VM) of database (windows), application server (linux-CentOs) and web server (linux-CentOs) were created for production and development environments with 1 vCPU, 2 cores and 4 GB of RAM each

6.- the servers that were created are:
db-prod (production database)
app-prod (production application server )
web-prod (production web server )
db-develop (develop database)
app-develop (develop application server)
web-develop (develop web server)


7.- Data protection settings were created by snapshot of virtual machines and no more than 1 hour of data loss after a failure

8.- The recovery snapshot of the production virtual machines was tested.
