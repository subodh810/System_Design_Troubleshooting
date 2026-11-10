Q. 1. Order Created but Payment Service never receives the event. How would you debug?

#Check:

>Producer logs, Topic data, Consumer group lag, Deserialization issues & Network connectivity


Q. 2. Payment succeeded but Order status remains PENDING. What might be wrong?

#Check:

>Event publication, Consumer failures, Dead Letter Topic & Saga execution


Q. 3. Customer was charged twice. How would you identify the root cause?

#Check:

>Duplicate events, Retry behavior, Missing idempotency & Manual reprocessing


Q. 4. Payment failed but Inventory remains reserved. How would you solve this?

#Expected solution:

>Saga Pattern, Compensation event, Inventory release event


Q. 5. Database updated successfully but Kafka event was never published. What is the issue?

>>Dual-write problem & Transactional Outbox Pattern required


Q. 6. One microservice becomes slow and all other services start failing. Why?

#Cascading failure

>>Solution:

Ci>rcuit Breaker, Timeouts & Bulkhead pattern


Q. 7. Service-to-service calls are timing out intermittently. How would you troubleshoot?

#Check:

>Network, DNS, API Gateway, Thread pools, Connection pools


Q. 8. A service suddenly starts returning 503 errors. What would you investigate?

>Pod status, CPU/Memory utilization, Downstream dependency failures, Thread exhaustion


Q. 9. Inventory count becomes negative. How would you identify the cause?

#Check:

>Concurrent updates, Duplicate events, Missing locking strategy


20. Different services show different status for the same order. Why?

Expected Answer:

Eventual consistency issue
