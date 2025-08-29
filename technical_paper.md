# Technical Paper: Service-Oriented Architecture (SOA)

## Introduction
Our system is big single block (monolith). It become slow, hard to change, and hard to scale. Service-Oriented Architecture (SOA) cut this big block into small parts (services). Each part do one job and talk with other by API.

## Problems with Monolithic System
- Whole system in one block  
- Slow when traffic increase  
- One shared database get heavy  
- Hard to add new feature or fix bug  
- Logs and error tracking not good  

## What is SOA
SOA break system into small services. Each service:  
- Do only one work  
- Keep own data  
- Talk to other with API or message  
- Can change without breaking whole system  

### Example Services
- Payment Service → handle payments  
- User Service → manage accounts, logins  
- Report Service → make reports  

## Benefits of SOA
- **Scalable**: Only grow busy parts  
- **Faster**: Each service can run better alone  
- **Quick build**: Teams work on different services  
- **Reliable**: One service fail, others still work  

## Challenges of SOA
- Many services hard to manage  
- Network talk add delay  
- Data must stay same in all services  
- Need good logs and monitoring  

## Plan to Use SOA
1. Start with one problem part (payment or report)  
2. Add basics: API gateway, logging, monitoring, service discovery  
3. Build and test first service  
4. Slowly move other parts one by one  

## Conclusion
SOA not magic fix. But step by step it make system faster, more strong, and easy to grow. Start small, track everything, learn on way.

## References
- [Service-Oriented Architecture on Wikipedia](https://en.wikipedia.org/wiki/Service-oriented_architecture)  
- [SOA Principles by IBM](https://www.ibm.com/cloud/learn/soa)  
- [Microservices vs SOA by Red Hat](https://www.redhat.com/en/topics/cloud-native-apps/soa-vs-microservices)  
