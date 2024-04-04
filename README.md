# Leader_Board_Task
Develop a leaderboard service for Tanx, ranking traders on the Decentralised Exchange by their
trading volume.
The task involves:
1. Leaderboard Service:
a. This service receives user IDs and their trading volumes, ranks them in real-time,
and
b. provides an API endpoint for accessing the current leaderboard list, including
user ID, cumulative volume, and rank.
2. Trade Producer Service:
a. This service periodically sends trade data, which has user IDs and volumes.
Infrastructure of the Service would be
● EC2_A - Leaderboard Service and Trade Producer Service
- EC2_B, EC2_C … are the instances where the technologies involved in the
project are hosted. Example -
■ EC2_B could have Postgres
■ EC2_C could have redis
- So, consider making different docker-compose files for various technologies used
in your assignment. [such as Postgres and Redis.] Create separate
docker-compose files for EC2_A, EC2_B and EC2_C
● Web traffic directed to the Leaderboard Service on port 80.
Brownie Points
- Implement a Message Queue for enhanced functionality.
- Adding a reverse proxy for Leaderboard API
- Cache the API responses for better read throughput.
-
