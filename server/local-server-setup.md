# Local Server Setup (Docker via Windows PowerShell)

Run these commands in Windows PowerShell to deploy the required lab infrastructure. Ensure Docker Desktop is running before executing.

### 1. Start the MQTT Broker
First, ensure you have placed the `mosquitto.conf` file in a folder located at `C:\mqtt\`.
```powershell
docker run -d --name mosquitto --restart unless-stopped -p 1883:1883 -v C:\mqtt\mosquitto.conf:/mosquitto/config/mosquitto.conf eclipse-mosquitto
