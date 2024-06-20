# Create a locally hosted networked Software Defined Radio (SDR) network!
This repo contains the files needed to install [OpenWebRX] (https://www.openwebrx.de/), a web-based SDR receiver running in a Docker container, connected to a SDR streaming over your local network.

1. Within the "OpenWebRX" folder, follow the directions to run the Docker Container which will run a web-server with an admin user.
2. Within the "SDR-network-stream", follow the directions to stream your SDR over the network.
3. Navigate to the OpenWebRX web-server and connect to the networked SDR using either rtl_tcp or SoapySDR.
4. Enjoy listening! 
