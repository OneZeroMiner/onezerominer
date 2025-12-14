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
                - dynex
                - xelishashv3
                - cryptix_ox8
                - qhash
                - zilliqa
          
          

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

      --max-memory <max-memory>
          Maximum memory allocated in percentage. eg: 70 (alias: chips-memory)

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
          Tuning parameter for Dynex. This is a comma separated list and the acceptable values for each gpu are 1, 2, 4, 8, 16, 32. Use * or 0 to skip a GPU

      --nr <nr>
          Tuning parameter for Dynex. This is a comma separated list and the acceptable values for each gpu are 1, 2, 4, 8. Use * or 0 to skip a GPU

      --zil-before-script <zil_before_script>
          script to run before Zilliqa sessions

      --zil-after-script <zil_after_script>
          script to run after Zilliqa sessions

      --zil-test
          Simulates zil sessions with a local test pool that has a session every 2 minutes. This can be useful for testing oc settings

      --zil-test-port <zil_test_port>
          Port of the Zil test pool

      --xelis-solo
          Xelis solo mining mode

      --disable-amd
          Disable AMD GPUs

      --disable-nvidia
          Disable Nvidia GPUs

      --disable-telemetry
          Disable data analytics

      --hashrate-avg <hashrate_avg>
          Number of seconds to average the hashrate over. Default is 10
          
          [default: 10]

      --dns-over-https
          DNS resolution over HTTPS

      --proxy <proxy>
          SOCKS5 proxy connection. Format: <host>:<port> or <user>:<pass>@<host>:<port>

      --kernel <kernel>
          Supported only for qubitcoin. Default is 1, kernel 2 is for cmp cards. eg: --kernel 1,1,2

      --dual-intensity <dual-intensity>
          comma seperated list of intensity pairs of the two algorithms for dual mining( Use * to skip a GPU). Format: <intensity_algo1>_<intensity_algo2>. eg: 9_7, *, 10_8

  -h, --help
          Print help (see a summary with '-h')

  -V, --version
          Print version
```

Supported algorithms
------------------------------------------

Algorithm           |  Nvidia | AMD |
--------------------| --------|-----|
dynex               | 2%      | x   |
xelishashv3         | 2%      | 2%  |
cryptix_ox8         | 2%      | x   |
qhash               | 3%      | x   |
zil                 | 0%      | x   |

Supported dual mining pairs
------------------------------------------
xelishashv2-qhash (Nvidia only)




Requirements
------------------------------------------ 
* Minimum Compute Capability of 6.0.
* Binary file have been built with CUDA 12.8 and minimum supported Nvidia driver version is 528.33.
* AMD ROCM drivers 5.6 or later
* Latest Microsoft Visual C++ Redistributable package on Windows. Direct link: 
https://aka.ms/vs/17/release/vc_redist.x64.exe

HiveOS and mmpOS
------------------------------------------
#### Custom package name is onezerominer-x.x.x.tar.gz
