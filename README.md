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

### LAB on Floating Static Routes

![image](https://user-images.githubusercontent.com/110488017/233990243-728c4544-91e3-4487-9a62-0314a21a56a7.png)

![image](https://user-images.githubusercontent.com/110488017/233994644-54bc0dec-3ec1-4916-912c-e22a6b0df234.png)

![image](https://user-images.githubusercontent.com/110488017/233994746-f145d5be-da78-4192-8ae9-060c2820d4ea.png)

![image](https://user-images.githubusercontent.com/110488017/233994832-9e489a98-9faf-4b15-95d4-2056e351ef38.png)

![image](https://user-images.githubusercontent.com/110488017/233995021-50de8811-a84a-4fbc-a1cb-ced4bf8d9cae.png)



