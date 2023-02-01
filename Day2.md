# Total Cost of Ownership (TCO)

![image](https://user-images.githubusercontent.com/98258627/216125870-5272b1db-71c8-49b9-a2fb-9cd5b109e9fc.png)

# Capital vs Operational Expenditure 

## CapEx
- The up-front spending of money on physical infrastructure .
- Costs from CapEx have a value that reduces over time.   
## OpEx 
- The spending and billing of services or prodeucts as needed.
- Expenses are deducted in the same year . 

![image](https://user-images.githubusercontent.com/98258627/216125946-ca351a1b-17ea-4105-ab82-4b7e0f9d47f1.png)

# Cloud Architecture Terminologies

- **Availiability** - Ability to ensure a service remains availiable (**Highly Availiable(HA)**)
- **Scalability** -  Ability to grow rapidly or unimpeded
- **Elasticity** - Ability to shrink and gorw to meet the demand
- **Fault Tolerance** - Ability to Prevent a failure
- **Disaster Recovery** - Ability to recover from a failure (**Highly Durable**)
## High Availiability 

Ability of a service to remain availiable by ensuring there is `no single point of failure` and ensure a certain level of performance

![image](https://user-images.githubusercontent.com/98258627/216126035-a8a8d7aa-427e-424a-b32e-658d0724e26a.png)

Running your workloads across multiple Availability Zones ensures that if 1 or 2 AZs become unavailable your service remains available. 
### How would you manage the traffic ?

#### Azure Load Balancer
A load Balance allows you to evenly distribute traffic to multiple servers in one or mor datacenters . If a datacenter or server becomns unavilable (unhealthy) the load balanceer will route the traffic to only availiable datacenters with servers.

## High Scalability 
Ability to increase your capacity based on the increasing demand or traffic , memory and computing power.

![image](https://user-images.githubusercontent.com/98258627/216126128-4bd6ed56-21f6-4d54-90b4-3e50ee868722.png)

## High Elasticity

Ability to automatically increase or decrease the capacity based on the current demand of traffic , memory and computing power.

![image](https://user-images.githubusercontent.com/98258627/216126168-3d929108-d747-4b49-a611-ead5160c6e5b.png)

### How do you accomplish being elastic on Azure ?

#### Azure VM Scale Sets
Automatically increae or decrease in response to demand or a defined schedule

#### Sql Server Stretch Database
Dynamically stretch warm and cold transactional data from Microsoft SQl Server 2016 to Microsoft Azure

## High Durability

Ability to recover from a disaster and to prevent the loss of data Solutions that recover from a disaster is known as **Disaster Recovery (DR)**

Questions relevant to high durability 

```
Do you have a backup?
How fast can you restore that backup ?
Does your backup still work ?
How do you ensure current live data is not corrupt ?
```
