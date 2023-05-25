# Land_registration_system

<img src="https://img.shields.io/badge/Ethereum-20232A?style=for-the-
badge&logo=ethereum&logoColor=white">

<img src="https://img.shields.io/badge/Flutter-%2302569B.svg?style=for-the-
badge&logo=Flutter&logoColor=white">

## Land Registration & Transaction using Blockchain
## Problem it Solves:
1. The elimination of middlemen: The elimination of middlemen or brokers makes the process of
land registration less expensive. Brokers who try to defraud uninformed people will be unable to
do so any longer. Brokers frequently take a long time to finish procedures, thus our project will
help people save time.
2. A distributed tamper-proof ledger that prohibits ownership fraud.
## Technology Stack:
1. Ethereum Blockchain
2. Web3Dart
3. Flutter
4. Metamask
## Demo
Our Dapp is demonstrated in this video [here](https://youtu.be/0Coz_ivOaHs)
## To Run Application Locally
1. Clone the github repository and cd to the folder
2. Install the flutter 3.0.2, nodejs
3. Install ganache and truffle as shown below:
```
npm install -g truffle
```
4. Open Ganache and keep it running in the Background
5. Install the Metamask chrome extension, choose the local network and import the accounts
6. Compile and run our migrations from the command line as shown below:
```
truffle compile
truffle migrate
```
6 .Copy contract address as seen in the image below and paste in variable `contractAddress`
located in the file `./lib/constant/constant.dart`
<pre>
2_deploy_migration.js
=====================
Replacing 'Land'
----------------
> transaction hash:
0x427b2b402f767ac6a90334ab3c687b086b274de747fe10d6e194743b15057d78
> Blocks: 0 Seconds: 0
<b>>contract address: 0xed690C24C60A48F8A9819c9A15AD75B70CFBEa5a</b>
> block number: 3
> block timestamp: 1650602828
> account: 0x33e94e4619f0AecDf81e9676Eb82c109FBa53356
> balance: 99.9154895
> gas used: 3996227
> gas price: 20 gwei
> value sent: 0 ETH

> total cost: 0.07992454 ETH
</pre>
7. In `constant.dart` file, change the value of the variable `chainId` to `'1337'` and change the
value of the variable `rpcUrl` to `"http://127.0.0.1:7545"`
8. Run the flutter web app
```
flutter pub get
flutter run -d web-server --web-port 5555
```
9. Open the browser and the dapp will be running in http://localhost:5555/
10. Create mapbox api key from https://www.mapbox.com/ and Replace it with
`mapBoxApiKey`in `constant.dart` file
11. Create nftstorage api key from https://nft.storage/ and replace it.
## Project Flowchart
<img src="screenshots/flowchart.png" height="450">
## Screenshots
Home Page | User Selection
<img src="screenshots/1.png" height="225"> |<img src="screenshots/2.png" height="225">

Login Page | Contract Owner Dashboard
<img src="screenshots/3.png" height="225"> |<img src="screenshots/4.png" height="225">

Land Inspector Dashboard | User Verification
<img src="screenshots/5.png" height="225"> |<img src="screenshots/6.png" height="225">

User Dashboard | Adding land on Map
<img src="screenshots/7.png" height="225"> |<img src="screenshots/8.png" height="225">

Buy Request. | Witness info,photo capture,transfer ownership
<img src="screenshots/9.png" height="225"> |<img src="screenshots/10.png" height="225">