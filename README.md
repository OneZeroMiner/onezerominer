# OneZeroMiner 1.0.1

Optimized GPU miner for crypto projects. This is the initial release and the only supported algorithm is DynexSolve.
### Links 

![GitHub all releases](https://img.shields.io/github/downloads/OneZeroMiner/onezerominer/total)

Website: http://onezerominer.com

Discord server : https://discord.gg/mXnyrHa

Releases: https://github.com/OneZeroMiner/onezerominer/releases

Options
------------------------------------------           
 ```                                                                                                   
Options:                                                                                            
  -a, --algo <algo>                                                                                 
          The algorithm to use for mining. Currently supported algorithms are:                      
                - dynex   (dnx)                                                                     
                                                                                                    
           [possible values: dynex]                                                                 
  -o, --pool <pool>                                                                                 
          Pool URL address                                                                          
  -w, --wallet <wallet>                                                                             
          Wallet address/Pool Username                                                              
  -p, --pass <pass>                                                                                 
          Pool Password [default: X]                                                                
      --api-host <api_host>                                                                         
          Host of the API [default: 127.0.0.1]                                                      
      --api-port <api_port>                                                                         
          Port of the API [default: 3001]                                                           
      --api-disable                                                                                 
          Disable API                                                                               
  -d, --devices <devices>                                                                           
          Comma seperated list of devices to use                                                    
      --chips-memory <chips-memory>                                                                 
          Percentage of memory allocated for dynex chips.                             
  -i, --intensity <intensity>                                                                       
          Intensity multiplier for the pow part. Number of pow hashes in one round = intensity * 32 
      --mallob-endpoint <mallob_endpoint>                                                           
          Mallob endpoint for Dynex                                                                 
      --log-file <log_file>                                                                         
          log file path                                                                             
  -h, --help                                                                                        
          Print help                                                                                
  -V, --version                                                                                     
          Print version  
```

Dev fee
------------------------------------------

Algorithm           |  Fee 
--------------------| ---- 
dynex               | 3%


Requirements
------------------------------------------ 
* Minimum Compute Capability of 6.0.
* Binary file have been built with CUDA 12.0 and minimum supported Nvidia driver version is 525.60.13. 

HiveOS
------------------------------------------
#### HiveOS package name is onezerominer-x.x.x.tar.gz
#### Sample Flight Sheet:

![HiveOS](https://github.com/OneZeroMiner/onezerominer/raw/main/hiveos.png?raw=true)
