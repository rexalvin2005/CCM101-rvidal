#Enterprise Cloud Architecture - Laboratory 10 Handover Manual

##1. System Overview & Architecture
- **Virtualization** Oracle VM VirtualBox running Ubuntu Server  64-bit with the network adapter set to Bridged Adapter mode.
- **Networking** Fixed Static IP configuration (`192.168.1.58/24`) managed via Netplan (`/etc/netplan/00-installer-connfig.yaml`).
- **Containerization** Docker & Docker Compose orchestrating an enterprise Wordpress web application tied to an isolated MYSQL database container (`enterprise_mysqql_db`) with persistent storage volumes.
- **Security & Access:** Configured firewall policies via UFW, restricting exposure while exposing necessary ports for SSH (22), HTTP (80), HTTPS (443) and the application container port (`8080`).

##2. Deployment Instructions
To replicate or deploy this specific stack on a fresh target Ubuntu environment:

1. Clone the project repository and navigate into the working directory.
2. Apply the static network configuration:
   - Edit `/etc/netplan/00-installer-config.yaml` to include your static IP allocation (`192.168.1.58/24`). 
   - Run the netplan applicator"
      ```bash
      sudo netplan apply
     
      ```
3. Spin up the multi-container stack using Docker Compose:
 
   ```bash
   docker-compose up -d
