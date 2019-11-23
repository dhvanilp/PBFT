# Blockchain Project

## Config 
The config.js can be changes for the following
- The number of nodes in the network
- Min transaction threshold for block formation

## Running
Make sure npm and node is installed
```
npm install 

First node: 
SECRET="NODE0" P2P_PORT=5000 HTTP_PORT=3000 node app

Second node: 
SECRET="NODE1" P2P_PORT=5001 HTTP_PORT=3001 PEERS=1 node app

Third node: 
SECRET="NODE2" P2P_PORT=5002 HTTP_PORT=3002 PEERS=2 node app
.
.
so on for multiple nodes
```

## Endpoint 
We made use of POSTMAN, curl or any other can be used

Following are the API endpoints :
- POST : ‘/transact’ — creates transactions, request object consists of data to be stored in the transaction
- GET : ‘/transactions’ — sends the transactions in the transaction pool as a response
- GET : ‘/blocks’ — sends the chain of the blockchain as a response