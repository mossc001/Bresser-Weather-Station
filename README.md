# Bresser-Weather-Station
Intercepting Bresser Weather Station Data

This is a guide on how to intercept the weather data produced from the Bresser 5-in-1 WiFi weather station. This uses a combination of a DNS intercept and webserver to replicate what is expected by the remote webserver to which the data would normally go.

Operating System: Proxmox VE 6.4.x

Container (LXC) Host Operating System: Ubuntu 20.04 Standard

https://tailscale.com

# Network

Topology: Weather Station > PiHole DNS > XAMPP Server > Local MQTT & WAN (Weatherunderground)

Firewall/Router: No modifications required
