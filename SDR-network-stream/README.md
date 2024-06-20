# Follow these instructions to stream your SDR over the local network

### Option 1: [rtl_tcp](https://manpages.ubuntu.com/manpages/trusty/man1/rtl_tcp.1.html) IQ Spectrum Server
1. Install rtl-sdr
```
sudo apt install rtl-sdr
```
2. Run the rtl_tcp server on your device IP address (found using "ip -a" on linux) -- subsitute "192.168.x.x" in the below command with your device IP address

```
rtl_tcp -a 192.168.x.x -p 9000
```

### Option 2: [Soapy SDR](https://github.com/pothosware/SoapySDR)
1. Install SoapySDR
```
sudo apt install soapyremote-server soapysdr-tools soapysdr-module-rtlsdr
```
2. Run the SoapySDR Server
```
SoapySDRServer --bind
```
Alternatively, can be run using:

```
systemctl start SoapySDRServer
systemctl status SoapySDRServer #to view the status of the server
systemctl stop SoapySDRServer 
```
3. SoapySDR server is now streaming to localhost:55132
