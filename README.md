# Create a locally hosted & networked Software Defined Radio (SDR) network!
This repo contains the files needed to install [OpenWebRX] (https://www.openwebrx.de/), a web-based SDR receiver running in a Docker container, connected to a SDR streaming over your local network.

<img src="https://github.com/Robert-litts/sdr-network/blob/main/remote_sdr_diagram.png" width="450" height="450">

1. Within the "OpenWebRX" folder, follow the directions to run the Docker Container which will run a web-server with an admin user.
2. Within the "SDR-network-stream", follow the directions to stream your SDR over the network.
3. Navigate to the OpenWebRX web-server and connect to the networked SDR using either rtl_tcp or SoapySDR.
4. Enjoy listening!

# RTL-SDR LXC Passthrough
1. Within the "Proxmox_LXC" folder is the lxc.conf file to run an unprivleged LXC and pass through the RTL-SDR device to the container. This allows you to create a low-resource container and use SoapySDR or rtl_tcp to stream the radio traffic onto the network.
