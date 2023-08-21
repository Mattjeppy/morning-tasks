# Load Balancing
​
Can you decide what type of load balancing from the notes might work best for the following situations;
​
## A chat service where users maintain active connections for a while

Least connection would be suitable for this because some users may maintain connection for a while and to balance the servers, requests should be made to those that are least active.
​
## An AI image generation API with paid tiers

Weighted Round Robin would be suitable because each tier can have a dedicated / weighted server for the demand (tier specific capacity). 

​
## A social media website that has users all over the world

Least response time, in which availability zones are available across the globe. This ensures users get the quickest response possible. Weighted Round Robin would also be a good choice for this because servers can be weighted to handle and upscale demand in each AZ.
​
## An authorisation service that takes the same amount of time for each request

Round robin would make the most sense because as each request takes the same amount of time, there won't be an issue when the round robin comes back around.
​
## A gaming server that requires low latency

Least response time due to the requirement to have low latency