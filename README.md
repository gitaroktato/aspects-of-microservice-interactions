# Aspects of Microservice Interactions
What are the recent challenges of microservice interactions? Have you ever had any issues with service-to-service calls which were especially hard to manage? Were you wondering about the reasons?
Unfortunately, there are some rules we can not bend. For instance, we can't modify the laws of physics and statistics. But luckily some problems are easily solvable. 

In this presentation I will look at the different aspects of microservice interactions and compare the most popular technologies available, so you can pick the most favorable one for your specific use case.



### Ideas
- libreate and conservative rule for APIs
- API secure, latent, performant, cacheable, etc.
-- Principles of Package design, SOLID!
-- API changeabiltiy, versiongin
- resiliency ...
- Existing talks (sync, async, Martin Kleppman two generals)
- Sam Newmann, versioning, runtime dependency, etc.
- sync vs async (little's law, queuing theory)
- Existing microservice 
- Size of microservice (drivers, SRP, bounded context, rewrite)
- OSI model from Distributed Systems 3rd Edition
- Service Mesh (Circuit breaker, backpressure differences)
- A little bit of SRE

### Additional Notes
- sync VS async (which one is better, timeouts, failure scenarios in sync mode)
- Architecture patterns => SAGA
- Example: Shopping cart: Fallback to sync mode and polling
- Example: Message ordering - Randy Shoup
- 12factor rules apply - request/reply queue example from Mark Richards
- Latency metrics and fallacies - design principle
- Circuit breakers
- No such thing as unbounded queue => Java tread pool
- Example: Remote call at startup -> rollback stuck (StyxPres)
- Separate critical paths and various workloads (sync/async, queue as a backpressure) => example LOMS
