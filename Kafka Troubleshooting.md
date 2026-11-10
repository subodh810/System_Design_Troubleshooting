Q. 1. Consumer lag suddenly increased from 1,000 to 5 million. How would you investigate?
>>Check:<br>
Consumer health, CPU/Memory, GC pauses, Database bottleneck, Network latency, Number of partitions && Consumer scaling.

Q. 2. Messages are being produced but consumers are not receiving them. What would you check?
>>Is the consumer running?<br>
Correct topic name?, Correct consumer group?, Offset position?, Deserialization errors? && ACL/Authorization issues?

Q. 3. Producer reports success but consumer never receives the message. How would you troubleshoot it?
>>Check:<br>
Producer ack settings, Topic existence, Partition assignment, Retention policy, Consumer offset & Producer logs


Q. 4. Consumer application is running but not consuming records. Why?

#Possible causes:<br>
All messages already consumed, Wrong consumer group, Rebalance stuck, Poll loop issue & Listener failure


Q. 5. Consumers are processing duplicate messages. How will you investigate?

#Check:<br>

>Consumer restart, Offset commit failure, Auto-commit settings, Retry mechanism & Producer retries.


Q. 6. Messages are arriving out of order. Why?

#Check:<br> 

>Multiple partitions, Missing message key, Multiple producers, Retry-based reordering


Q. 7. Kafka broker crashed. What happens and how do you verify recovery?

#Check:<br>

> Replication factor, ISR, Leader election, Controller logs


Q. 8. Consumer crashes after DB update but before offset commit. What happens?

#Investigate:

>Duplicate processing, Idempotency implementation, Commit strategy


Q. 9. Topic disk usage suddenly grows to several hundred GB. What would you check?

>retention.ms, retention.bytes, Log compaction, Consumer lag & Unconsumed records


Q. 10. Kafka cluster is healthy, but application latency increased. How would you debug?

#Check:

>Consumer lag, Database response times, External API latency, GC activity & Thread pool exhaustion
