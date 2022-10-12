# OnlineVotingSystemUsingAWS

The app architecture leverages a few AWS managed services. Managed services help you reduce cost and maintenance.

API Gateway: This creates a POST endpoint for user votes, and forwards an event to Lambda.


Lambda: These are scalable containers for the app. There are two Lambda functions:

Function 1: Updates the database with a user’s vote
Function 2: Updates the website with the latest results


DynamoDB: The data is stored in a managed NoSQL database.
S3: HTML/CSS/JS files are hosted as a website. A JSON file on S3 caches the latest tallies, which reduces the number of calls to DynamoDB.

Develop an Voting Application The sample app in the presentation is a simple voting website. As a user, you pick a presidential candidate on a form. The results are tallied on the bottom with Display Results Project on AWS Cloud using DynamoDB, Lambda Function S3 Bucket






