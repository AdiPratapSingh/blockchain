# Coin
This is an implementation of core concepts in cryptocurrncy. Flask is used to deploy the nodes.

# Dependencies
- ```pip install flask```
- Postman app

# Local testing
In order to run a node, simply run
```python Coin_5000.py```
You can start other nodes at disired port by editing the port number in the last line.

To interact with the node, we need postman app. After downloading postman you can do following:
- Add nodes by making a post request of json file in the format of nodes.js. If you are running at port 5000 then make the post request at
```http://127.0.0.1:5000/connect_node```
- Add a transaction by making a post request in json fromat as via postman. If you are running at port 5000 then make the post request at
```http://127.0.0.1:5000/new_transaction```
- Mine a block. This will place all the unconfirmed transaction in mempool into the upcomming block. If you are running at port 5000 then make the get request at
```http://127.0.0.1:5000/mine_block```
- Follow a concensus by getting the longest valid chain in the whole network. If you are running at port 5000 then make the get request at
```http://127.0.0.1:5000/get_longest```
- View the current full chain. If you are running at port 5000 then make the get request at
```http://127.0.0.1:5000/full_chain```

A sample output can be seen in consensus.json


