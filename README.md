# Bresser Weather Station
Intercepting Bresser Weather Station Data

This is a guide on how to intercept the weather data produced from the Bresser 5-in-1 WiFi weather station. This uses a combination of a DNS intercept and webserver to replicate what is expected by the remote webserver to which the data would normally go.

Once the data is intercepted and store locally, its then forwarded to the relevant weather provider as originally planned e.g. Weatherunderground. Additionally as the data is now intercepted, you can publish the data to any weather service API. In the guide under "POST TO WOW MET OFFICE", I also publish the data to the UK Met Office weather API.

Operating System: Proxmox VE 6.4.x

Container (LXC) Host Operating System: Ubuntu 20.04 Standard

https://www.bresseruk.com/Weatherstations/Weather-Center/BRESSER-WIFI-color-weather-center-with-5in1-profi-sensor.html

# Network

Topology: Weather Station > PiHole DNS > XAMPP Server > Local MQTT & WAN (Weatherunderground)

Firewall/Router: No modifications required
