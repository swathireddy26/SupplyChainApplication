# SupplyChainApplication
1. Created basic supply chain application where we can keep track of items in all stages starting from creation to delivery.
2. Seller can create a product, an address will be associated with this product and anyone who wants to buy this product can send specified ether to that address. Once the payment is done, seller will get the notification to send the product.
3. We will perform event triggers for every action taken in the supply chain.

# Project Diagram

<img width="1655" alt="Supply_Chain" src="https://user-images.githubusercontent.com/10496268/126784507-20a16437-2b0a-47f2-8005-85359ebf82ad.png">

# Reference:
https://ethereum-blockchain-developer.com/050-supply-chain-project/00-overview/

# Tools needed:
1. Truffle box for Local DAPP Developemnt: https://github.com/truffle-box/react-box
2. Metamask for Deploying it in Test networks:  https://metamask.io/
3. Ganache by Truffle for Local blockchain testing:  https://www.trufflesuite.com/ganache

# Installation
1. npm install -g truffle ---> Truffle intsallation
2. truffle unbox react    ---> Unbox the React box

## How to execute the DAPP?
1. Connect ganache to the Metamask using Custom RPC option in Metamask and import the accounts from Ganache
2. Make Sure that Ganache is running Locally (We can start Ganache either with GUI or by using the Ganache-CLI("ganache-cli --port 7545 --chainId 5777")
3. Run the React Application using "npm run start", this will start our React application in localhost:3000
4. We can supply the Cost and Item Name in the application and click on create button. Item state would be "create" at this point in time.
5. Then, we will be supplied with a popup window to send the Item cost to the contract address. We can send the amount either by using metamask or by uisng truffle console.
6. After successful payement, Item state would change to Paid and a pop up window will appear asking to deliver the product.
7. Item can now be dispatched from warehouse
8. We can either use Ganache or any Test network to deploy the application on blockchain. We use Infura to deploy the app on test networks.

