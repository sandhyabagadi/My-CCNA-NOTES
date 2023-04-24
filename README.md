# My-CCNA-NOTES

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
