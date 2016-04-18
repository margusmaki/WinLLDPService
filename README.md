# WinLLDPService
Small LLDP Windows Service. 

Used by network switches to list network devices - https://en.wikipedia.org/wiki/Link_Layer_Discovery_Protocol

Sends LLDP packets to switch. Switch must have LLDP capability. It **doesn't** query switches' internal LLDP data. Errors are logged to Windows Event Log.

See homepage for more information and download `.msi` installer - https://raspi.github.io/winlldpservice/

Uses 

* SharpPcap - https://www.nuget.org/packages/SharpPcap/
* Packet.NET - https://www.nuget.org/packages/PacketDotNet/

Programmed in C#
 
# How to build
Uses WiX to build .msi installer package. See `build` directory for more information.

# License
MIT
