# PhoenixMiner DevFee interceptor


## What is this?
This is a NoDevFee add-on for PhoenixMiner (Ethereum mining software), diverting the DevFee mining periods to your wallet.


## How does it work?  
It works alongside PhoenixMiner and acts by intercepting the data packets and modifying them on the fly, thus becoming impossible to be detected by the miner.

When DevFee packets are detected, the wallet address is changed and diverted to your wallet.
  

## Usage

1.  Download the zip file from the releases section and unpack it
2.  Launch PhoenixMiner DevFee interceptor by double-clicking `divert.exe`    
3.  Launch PhoenixMiner as usual

Result:
![Example](https://i.imgur.com/E8AjHgt.png)    

## How to check if NoDevFee is working correctly?
Look at your pool and check whether an `eth1.0` worker appears.
![Example](https://i.imgur.com/lqkiqGa.png)   
  
## Is this a scam?  
Of course not. We know the internet is full of NoDevFee scams. Our team made this software to help the community. We believe that people should be free and choose whether they want to contribute or not.

## Does it contain virus?  
Absolutely not. Here’s the virustotal report:
![Example](https://antiscan.me/images/result/VUZgjtszgKoI.png)

## How to start it on boot before PhoenixMiner?
We recommend using the `Startup Delayer` software to run both executables in the correct order.

## What can I do if the detected wallet address is incorrect?  
Make sure you started PhoenixMiner interceptor before PhoenixMiner.  
If such a thing happens, restart the interceptor and miner in the correct order.

## Technical info  
This interceptor uses the WinDivert lib (https://github.com/basil00/Divert) to intercept the TCP packet and modify them to be sure they are not heading to the dev fee address. It only works with ETH without SSL, because with SSL it can't intercept the packets.

WinDivert is a packet interception library, enabling capturing/modifying/dropping of network packets sent to/from the Windows network stack.
  

## Requirements
NET Framework 4.7.2 Runtime
  

## Donate
#### ETH: `0x851EAa1169f02D4Da54994f9c1C1556636b97279`