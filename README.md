# rpcscanner
dcerpc协议解析识别，利用impacket框架识别epmapper接口，OXIDResolver的ServerAlive2接口

# Example Run
```bash
$python rpcscanner.py 192.168.150.147                      
[*] Retrieving network interface of 192.168.150.147
Address: WIN-ASFCEO2CAMW
Address: 192.168.150.155
Address: 192.168.150.147

[*] Retrieving endpoint list from 192.168.150.147
Protocol: N/A 
Provider: iphlpsvc.dll 
UUID    : 552D076A-CB29-4E44-8B6A-D15E59E2C0AF v1.0 IP Transition Configuration endpoint
Bindings: 
          ncacn_ip_tcp:192.168.150.147[49154]
          ncacn_np:\\WIN-ASFCEO2CAMW[\PIPE\atsvc]
          ncalrpc:[senssvc]
          ncalrpc:[OLEFB25E6403A994900B593855D0DB1]
          ncalrpc:[IUserProfile2]
          ncalrpc:[LRPC-646ea7cb5c97b229fa]

Protocol: N/A 
Provider: schedsvc.dll 
UUID    : 0A74EF1C-41A4-4E06-83AE-DC74FB1CDD53 v1.0 
Bindings: 
          ncalrpc:[senssvc]
          ncalrpc:[OLEFB25E6403A994900B593855D0DB1]
          ncalrpc:[IUserProfile2]
          ncalrpc:[LRPC-646ea7cb5c97b229fa]

Protocol: N/A 
Provider: nsisvc.dll 
UUID    : 7EA70BCF-48AF-4F6A-8968-6A440754D5FA v1.0 NSI server endpoint
Bindings: 
          ncalrpc:[LRPC-503e16876e73e8736c]
          ncalrpc:[OLE4BCDC33AF2D94FB48768E4E09A55]

Protocol: [MS-CMPO]: MSDTC Connection Manager: 
Provider: msdtcprx.dll 
UUID    : 906B0CE0-C70B-1067-B317-00DD010662DA v1.0 
Bindings: 
          ncalrpc:[LRPC-b602a59621da2075ab]
          ncalrpc:[LRPC-b602a59621da2075ab]
          ncalrpc:[LRPC-b602a59621da2075ab]
          ncalrpc:[LRPC-b602a59621da2075ab]

```

# reference

- [The OXID Resolver](https://airbus-cyber-security.com/the-oxid-resolver-part-1-remote-enumeration-of-network-interfaces-without-any-authentication/)
- [impacket](https://github.com/SecureAuthCorp/impacket)
