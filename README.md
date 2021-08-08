# Wi-Cache

Wi-Cache is an SDN based distributed caching system for the WiFi edge.
It is based on Odin framework ([Odin Wi5](https://github.com/Wi5/odin-wi5/wiki)).

It enables file/content to be cached on WiFi APs and deliver the cached content to wireless clients.

Wi-Cache consists mainly of three components:
1. Wi-Cache controller: This consists of the Wi-Cache module and the Odin framework. The Wi-Cache controller runs on a dedicated system or alongside the system where the files are stored. The main functions of the Wi-Cache controller are: <br /> <br />
(i) Split the files in to segments, distribute the segments across the WiFi APs, or read a configuration file that specifies file/segment distribution. <br /> 
(ii) Route the file/content request coming from the wireless clients to the appropriate Wi-Cache AP-caches for delivery. <br /> <br /> 
Detailed information on building, running the Wi-Cache controller, etc. are provided in <br />  <br /> https://github.com/hrchhangte/Wi-Cache-Controller 

2. Wi-Cache agent (at Wi-Cache WiFi AP): This consists of the Wi-Cache agent that handles caching and file delivery, and the Odin agent. The Wi-Cache runs on WiFi acess points (that runs Linux OpenWrt). <br /> <br /> Detailed information on building, running the Wi-Cache agent, etc. are provided in <br /> <br /> https://github.com/hrchhangte/Wi-Cache-Agent

3. Wi-Cache client/client-side-module: This consists of the Wi-Cache module at the client side that interacts with the Wi-Cache controller and Wi-Cache agent for file download. A client application at the wireless client can use the client-side-module to use the sevices provided by Wi-Cache. <br /> Detailed information on running and using the client-side-module are provided in <br /> <br /> https://github.com/hrchhangte/Wi-Cache-Client
