# Tamper Proof Data

At Bequest, we require that important user data is tamper proof. Otherwise, our system can incorrectly distribute assets if our internal database is breached. 
Only the user is able to update their own data.


**1. How does the client insure that their data has not been tampered with? Assume that the database is compromised.**
<br />
**2. If the data has been tampered with, how can the client recover the lost data?**


Edit this repo to answer these two questions using any technologies you'd like, there any many possible solutions. Feel free to add comments.

### To run the apps:
```npm run start``` in both the frontend and backend

## To make a submission:
1. Clone the repo
2. Make a PR with your changes in your repo
3. Email your github repository to robert@bequest.finance


# Solution

## Server:

1. Hash is added to check tamper
2. Added verify-data api to check the data is tempered or not
3. Added backup database for recovery and recover-data api to recover data


## Client:

1. Implemented verifyData method which check the data is tampered or not
2. This data is compared with hashed data on the server
3. If the data is tampered recover API call is made to fetch backup data