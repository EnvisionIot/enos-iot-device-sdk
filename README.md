# EnOS™ IoT Device SDK

EnOS™ provides device SDKs that encapsulates protocols for data transmission between devices and EnOS Cloud.

For MQTT-based transmission, we support:

- [EnOS Device SDK for MQTT (C)](https://github.com/EnvisionIot/enos-mqtt-sdk-c)
- [EnOS Device SDK for MQTT (Java)](https://github.com/EnvisionIot/enos-mqtt-sdk-java)
- [EnOS Device SDK for MQTT (Node.js)](https://github.com/EnvisionIot/enos-mqtt-sdk-nodejs)
- [EnOS Device SDK for MQTT (Python)](https://github.com/EnvisionIot/enos-mqtt-sdk-python)

For HTTP-based transmission, we support:

- [EnOS Device SDK for HTTP (Java)](https://github.com/EnvisionIot/enos-http-sdk-java)

For information on how to obtain and use the device SDK for your programing language, see the README file of their GitHub source code repo.

## Function Availability and Comparison

The following table shows an overview of which functions are available in different device SDKs.


| **Function List**              |                                      | **Java** | **Node.js** | **C** | **Python** |
|--------------------------------|--------------------------------------|----------|-------------|-------|------------|
| Protocol                       | MQTT                                 | √        | √           | √     | √          |
|                                | CoAP                                 |          |             |       |            |
|                                | HTTP \*1                              | √        |             |       |            |
| Connectivity and Authentication   | Secret-based authentication - per-device secret \*2 | √        | √           | √     | √          |
|                                | Secret-based authentication - per-product secret \*3  | √        | √           | √     | √          |
|                                | X.509-certificate-based authentication \*4       | √        | √           | √     | √          |
| Uploading data to cloud (device to cloud) | Device tags | √        | √           | √     | √          |
|                                           | Attributes  | √        | √           | √     | √          |
|                                           | Measuring points | √        | √           | √     | √          |
|                                           | Events   | √        | √           | √     | √          |
|                                           | Uploading data in pass-through mode \*5             | √        | √           | √     | √          |
| Issuing command to device (cloud to device) | Setting measuring point values | √        | √           | √     | √          |
|                                             | Invoking services              | √        | √           | √     | √          |
|                                             | Receiving data in pass-through mode | √        | √           | √     | √          |
| Subdevice Management  | Subdevice registeration | √        | √           |       | √          |
|                       | Login and logout of subdevices | √        | √           |       | √          |
|                       | Subdevice lifecycle management | √        | √           |       | √          |
| Firmware Upgrade OTA           | Uploading and receiving firmware information  | √        |             |       | √          |
| Message Integration            |                                      | √        |             |       | √          |
| Feature availability           | Auto Re-connection                   | √        | √           | √     | √          |
|                                | Connection state reporting           | √        | √           | √     | √          |
|                                | Asynchronous data reporting          | √        | √           | √     | √          |

### Supplementary Information

The following information supplements the above table to provide details about relevant fucntions of the SDKs.

\*1 For HTTP protocol, we currently support reporting file type of data through
measuring point.

\*2 Per-device secret authentication

\*3 Per-product secret authentication

\*4 X.509-certificate-based authentication 

\*5 Pass-through mode


