# OneZeroMiner 

Optimized GPU miner for crypto projects. 
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
                - zilliqa  (zil)
          
          

      --a2 <algo2>
          The second algorithm

  -o, --pool <pool>
          You can use ssl:// or stratum+ssl:// prefix for SSL/TLS encrypted connections.

      --o2 <pool2>
          List of pools for the second algorithm

  -w, --wallet <wallet>
          Wallet address/Pool Username

      --w2 <wallet2>
          Wallet address/Pool Username for the second algorithm

  -p, --pass <pass>
          Pool Password
          
          [default: X]

      --p2 <pass2>
          Pool Password for the second algorithm
          
          [default: X]

      --worker <worker>
          Worker name
          
          [default: worker]

      --worker2 <worker2>
          Worker name for the second algorithm
          
          [default: worker]

      --api-host <api_host>
          Host of the API
          
          [default: 127.0.0.1]

      --api-port <api_port>
          Port of the API
          
          [default: 3001]

      --api-disable
          Disable API

  -d, --devices <devices>
          Comma seperated list of devices to use

      --d2 <devices2>
          Comma seperated list of devices to use for the second algorithm

      --chips-memory <chips-memory>
          Percentage of total memory allocated for dynex chips. Default uses 96% of free memory instead of total memory

      --mallob-endpoint <mallob_endpoint>
          List of Mallob endpoints for Dynex

      --log-file <log_file>
          log file path

      --cclk <cclk>
          list of core clocks. Use * to skip a GPU

      --cclk2 <cclk2>
          list of core clocks for the second algorithm. Use * to skip a GPU

      --coff <coff>
          list of core clocks offsets. Use * to skip a GPU

      --coff2 <coff2>
          list of core clocks offsets for the second algorithm. Use * to skip a GPU

      --mclk <mclk>
          list of memory clocks. Use * to skip a GPU

      --mclk2 <mclk2>
          list of memory clocks for the second algorithm. Use * to skip a GPU

      --moff <moff>
          list of memory clocks offsets. Use * to skip a GPU

      --moff2 <moff2>
          list of memory clocks offsets for the second algorithm. Use * to skip a GPU

      --fan <fan>
          list of fan speeds. Use * to skip a GPU

      --fan2 <fan2>
          list of fan speeds for the second algorithm. Use * to skip a GPU

      --pl <pl>
          list of power limits. Use * to skip a GPU

      --pl2 <pl2>
          list of power limits for the second algorithm. Use * to skip a GPU

      --max-no-acc <max_no_acc>
          Maximum number of minutes that the pool can stay connected without an accepted share
          
          [default: 15]

      --no-cert-validation
          This option is not recommended. If you set this flag, the miner will accept any certificate including invalid, expired or self signed certificates.

      --nt <nt>
          Tuning parameter. This is a comma separated list and the acceptable values for each gpu are 1, 2, 4, 8, 16, 32. Use * or 0 to skip a GPU

      --nr <nr>
          Tuning parameter. This is a comma separated list and the acceptable values for each gpu are 1, 2, 4, 8. Use * or 0 to skip a GPU

      --zil-before-script <zil_before_script>
          script to run before Zilliqa sessions

      --zil-after-script <zil_after_script>
          script to run after Zilliqa sessions

      --zil-test
          Simulates zil sessions with a local test pool that has a session every 2 minutes. This can be useful for testing oc settings

      --zil-test-port <zil_test_port>
          Port of the Zil test pool

  -h, --help
          Print help (see a summary with '-h')

  -V, --version
          Print version
```

Dev fee
------------------------------------------

Algorithm           |  Fee 
--------------------| ---- 
dynex               | 3%
zil                 | 0%


Requirements
------------------------------------------ 
* Minimum Compute Capability of 3.5.
* Binary file have been built with CUDA 11.8 and minimum supported Nvidia driver version is 450.80.02.

HiveOS
------------------------------------------
#### HiveOS package name is onezerominer-x.x.x.tar.gz
#### Sample Flight Sheet:

![HiveOS](https://github.com/OneZeroMiner/onezerominer/raw/main/hiveos.png?raw=true)
