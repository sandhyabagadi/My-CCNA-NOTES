## Dynamic Routing

### 2 Types

- IGP - Share routes within single AS
- EGP - Share routes with different AS

![image](https://user-images.githubusercontent.com/110488017/233979142-4da6b85a-d249-44fb-8484-47e20aff0e76.png)

- If there are 2 routes to the destination with the same metric, then the traffic is load balanced.

![image](https://user-images.githubusercontent.com/110488017/233981959-c12ab77e-a175-4278-8040-285dfd8e295c.png)

![image](https://user-images.githubusercontent.com/110488017/233982233-c793e476-16fe-4e4e-a782-f40a2740c47b.png)

### Admistrative Distance

- used to determine which routing protocol is preferred.
- Lower AD is preferred.

![image](https://user-images.githubusercontent.com/110488017/233985523-4f705e6c-817c-4aa3-b70a-a60d390d3150.png)


### Floating Static Routes

- A floating static route is used as a backup route. It has a manually configured administrative distance greater than that of the primary route and therefore would not be in the routing table until the primary route fails.

### LAB on Floating Static Routes

![image](https://user-images.githubusercontent.com/110488017/233990243-728c4544-91e3-4487-9a62-0314a21a56a7.png)

![image](https://user-images.githubusercontent.com/110488017/233994644-54bc0dec-3ec1-4916-912c-e22a6b0df234.png)

![image](https://user-images.githubusercontent.com/110488017/233994746-f145d5be-da78-4192-8ae9-060c2820d4ea.png)

![image](https://user-images.githubusercontent.com/110488017/233994832-9e489a98-9faf-4b15-95d4-2056e351ef38.png)

![image](https://user-images.githubusercontent.com/110488017/233995021-50de8811-a84a-4fbc-a1cb-ced4bf8d9cae.png)

## RIP

- Metric - Hopcount (MAX-15)
- 3 versions - 1,2, RIPng(RIP next gen) for IPV6
- 2 types of messages 
  - request and response
- Sends the table every 30 secs by default
- Multicast to - 224.0.0.9

![image](https://user-images.githubusercontent.com/110488017/234011428-9a16735d-ebc0-448a-a57b-265116c6e837.png)

- The network command will look for infaces which fall under that classfull network and activate RIP on those interfaces.
- Form adjacencies with the neighboring RIP enabled routers
- Advertise the prefix.

### Passive interface

- RIP routers which are not connected to other routers should be kept in passive so that unnessesary advertisements wont take place.

![image](https://user-images.githubusercontent.com/110488017/234012858-3f522869-fc71-4c11-873f-7268de9cbcc4.png)

### Default information originate

- To share the configured default route to other routers.

![image](https://user-images.githubusercontent.com/110488017/234013170-cbb66e26-9e4a-48e8-af5c-cec8790979a1.png)

## Enhanced Interior Gateway Routing Protocol (EIGRP)

- Advanced/ Hybrid Distance vector routing protocol
- can perform unequal cost Load balancing
- Doesnt have a hop limit like RIP
- uses wildcard mask (Inverted Subnetmask)

![image](https://user-images.githubusercontent.com/110488017/234041490-11f16f50-2810-4296-8fa2-711597bb6032.png)

### Example of wildcards

![image](https://user-images.githubusercontent.com/110488017/234016513-5e19e709-6bfd-427c-9e12-d38480540a28.png)

#### Metric

- EIGRP determines the value of the path using five metrics: bandwidth, load, delay, reliability and MTU.
- EIGRP uses five different messages to communicate with its neighbor routers. EIGRP messages are Hello, Update, Query, Reply, and Acknowledgement.

#### Router ID
- The router ID, a 32-bit number, uniquely identifies the router within an autonomous system (AS) (see Autonomous systems)

- EIGRP automatically selects the highest IP address on any active loopback interface as the router ID. If there is no loopback interface then the highest IP address on any active interface is used.

![image](https://user-images.githubusercontent.com/110488017/234020344-32b737c6-8361-4426-9fbd-c4713159aae1.png)

## LAB on EIGRP

![image](https://user-images.githubusercontent.com/110488017/234035111-8ca12b11-c3b4-4c59-a9f3-a445dd756a88.png)

![image](https://user-images.githubusercontent.com/110488017/234016187-6316e371-a528-44f1-b1db-377afacfd041.png)

### Loopback Interfaces
![image](https://user-images.githubusercontent.com/110488017/234034830-29e36b8e-d446-409e-85d8-b5103bd06833.png)

### To enable EIGRP on all interfaces at once ( doing invidually is recommended )
![image](https://user-images.githubusercontent.com/110488017/234039510-22bc0e6a-6bd0-4e67-a39b-b08ecbea6c2c.png)
