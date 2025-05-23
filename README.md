# IT Capstone Home Lab - HomeNode
HomeNode - the all-in-one home lab infrastructure designed for cloud storage, secure remote access but also an optional easy to use home server dashboard. Everything can be implemented via a docker-compose.yaml file(s). 

- **VMware** - Hypervisor (for advanced virtualization needs)
- **Ubuntu Server** - Host OS
- **Portainer** - Docker Management GUI
- **Nextcloud** - Personal Cloud Storage
- **Tailscale** - Secure remote access
- *Optional* **Home Assistant** - Device Automation


## Prerequisities

- VMware ESXi for virtualization (latest version of [VMware Workstation Pro]([url](https://www.vmware.com/products/desktop-hypervisor/workstation-and-fusion)) - free for personal use) https://www.vmware.com/products/desktop-hypervisor/workstation-and-fusion
- Ubuntu Server 22.04+ - https://ubuntu.com/download/server
- Docker & Docker Compose - https://docs.docker.com/engine/install/ubuntu/
- On mobile device from device app store:
    - Tailscale
    - NextCloud


# Services 

Service  |  URL/Access

1. Portainer | http://ip-address:9000 or http://localhost:9000
2. Nextcloud | http://ip-address:8080 or http://localhost:8080
3. Tailscale | Runs as VPN - mild configuration needed 
4. *Optional* Home Assistant | http://ip-address:8123 or http://localhost:8123

*Each service has its own directory for volume persistence or custom configuration (where needed)*  
*Ensure there are no overlapping ports for that will cause conflicts in performance* 
