# CGminer


CGminer is the most common interface tool used for bitcoin mining when operating in terminal simply type "cgminer" and it will launch the application. however since it will probably be your first time using this program we will start with the basics


COMMAND: cgminer -help 

cgminer 4.9.2
Built with avalon avalon2 avalon4 bflsc bitfury cointerra drillbit hashfast icarus klondike mining support.
Usage: cgminer [-DlmpPqUTouOchnV] 
Options for both config file and command line:
--anu-freq <arg>    Set AntminerU1/2 frequency in MHz, range 125-500 (default: 250.0)
--api-allow <arg>   Allow API access only to the given list of [G:]IP[/Prefix] addresses[/subnets]
--api-description <arg> Description placed in the API status header, default: cgminer version
--api-groups <arg>  API one letter groups G:cmd:cmd[,P:cmd:*...] defining the cmds a groups can use
--api-listen        Enable API, default: disabled
--api-mcast         Enable API Multicast listener, default: disabled
--api-mcast-addr <arg> API Multicast listen address
--api-mcast-code <arg> Code expected in the API Multicast message, don't use '-'
--api-mcast-des <arg> Description appended to the API Multicast reply, default: ''
--api-mcast-port <arg> API Multicast listen port (default: 4028)
--api-network       Allow API (if enabled) to listen on/for any address, default: only 127.0.0.1
--api-port <arg>    Port number of miner API (default: 4028)
--api-host <arg>    Specify API listen address, default: 0.0.0.0
--au3-freq <arg>    Set AntminerU3 frequency in MHz, range 100-250 (default: 225.0)
--au3-volt <arg>    Set AntminerU3 voltage in mv, range 725-850, 0 to not set (default: 775)
--avalon-auto       Adjust avalon overclock frequency dynamically for best hashrate
--avalon-cutoff <arg> Set avalon overheat cut off temperature (default: 60)
--avalon-fan        Set fanspeed percentage for avalon, single value or range (default: 20-100)
--avalon-freq       Set frequency range for avalon-auto, single value or range
--avalon-options <arg> Set avalon options baud:miners:asic:timeout:freq:tech
--avalon-temp <arg> Set avalon target temperature (default: 50)
--avalon2-freq      Set frequency range for Avalon2, single value or range, step: 25
--avalon2-voltage   Set Avalon2 core voltage, in millivolts, step: 125
--avalon2-fan       Set Avalon2 target fan speed
--avalon2-cutoff <arg> Set Avalon2 overheat cut off temperature (default: 98)
--avalon2-fixed-speed Set Avalon2 fan to fixed speed
--avalon2-polling-delay <arg> Set Avalon2 polling delay value (ms) (default: 20)
--avalon4-automatic-voltage Automatic adjust voltage base on module DH
--avalon4-voltage   Set Avalon4 core voltage, in millivolts, step: 125
--avalon4-freq      Set frequency for Avalon4, 1 to 3 values, example: 445:385:370
--avalon4-fan       Set Avalon4 target fan speed range
--avalon4-temp <arg> Set Avalon4 target temperature (default: 42)
--avalon4-cutoff <arg> Set Avalon4 overheat cut off temperature (default: 65)
--avalon4-polling-delay <arg> Set Avalon4 polling delay value (ms) (default: 20)
--avalon4-ntime-offset <arg> Set Avalon4 MM ntime rolling max offset (default: 4)
--avalon4-aucspeed <arg> Set Avalon4 AUC IIC bus speed (default: 400000)
--avalon4-aucxdelay <arg> Set Avalon4 AUC IIC xfer read delay, 4800 ~= 1ms (default: 19200)
--balance           Change multipool strategy from failover to even share balance
--benchfile <arg>   Run cgminer in benchmark mode using a work file - produces no shares
--benchfile-display Display each benchfile nonce found
--benchmark         Run cgminer in benchmark mode - produces no shares
--bflsc-overheat <arg> Set overheat temperature where BFLSC devices throttle, 0 to disable (default: 85)
--bitburner-voltage <arg> Set BitBurner (Avalon) core voltage, in millivolts
--bitburner-fury-voltage <arg> Set BitBurner Fury core voltage, in millivolts
--bitburner-fury-options <arg> Override avalon-options for BitBurner Fury boards baud:miners:asic:timeout:freq
--bxf-bits <arg>    Set max BXF/HXF bits for overclocking (default: 54)
--bxf-debug <arg>   BXF: Debug all USB I/O, > is to the board(s), < is from the board(s) (default: 0)
--bxf-temp-target <arg> Set target temperature for BXF/HXF devices (default: 82)
--bxm-bits <arg>    Set BXM bits for overclocking (default: 54)
--btc-address <arg> Set bitcoin target address when solo mining to bitcoind (mandatory)
--btc-sig <arg>     Set signature to add to coinbase when solo mining (optional)
--compact           Use compact display without per device statistics
--cta-load <arg>    Set load for CTA devices, 0-255 range (default: 0)
--ps-load <arg>     Set power supply load for CTA devices, 0-100 range (default: 0)
--debug|-D          Enable debug output
--disable-rejecting Automatically disable pools that continually reject shares
--drillbit-options <arg> Set drillbit options <int|ext>:clock[:clock_divider][:voltage]
--drillbit-auto <arg> Enable drillbit automatic tuning <every>:[<gooderr>:<baderr>:<maxerr>]
--fix-protocol      Do not redirect to stratum protocol from GBT
--hfa-hash-clock <arg> Set hashfast clock speed (default: 550)
--hfa-fail-drop <arg> Set how many MHz to drop clockspeed each failure on an overlocked hashfast device (default: 10)
--hfa-fan           Set fanspeed percentage for hashfast, single value or range (default: 10-85)
--hfa-name <arg>    Set a unique name for a single hashfast device specified with --usb or the first device found
--hfa-noshed        Disable hashfast dynamic core disabling feature
--hfa-options <arg> Set hashfast options name:clock (comma separated)
--hfa-temp-overheat <arg> Set the hashfast overheat throttling temperature (default: 95)
--hfa-temp-target <arg> Set the hashfast target temperature (0 to disable) (default: 88)
--hro-freq          Set the hashratio clock frequency
--hotplug <arg>     Seconds between hotplug checks (0 means never check)
--klondike-options <arg> Set klondike options clock:temptarget
--load-balance      Change multipool strategy from failover to quota based balance
--log|-l <arg>      Interval in seconds between log output (default: 5)
--lowmem            Minimise caching of shares for low memory applications
--monitor|-m <arg>  Use custom pipe cmd for output messages
--nfu-bits <arg>    Set nanofury bits for overclocking, range 32-63 (default: 50)
--net-delay         Impose small delays in networking to not overload slow routers
--no-submit-stale   Don't submit shares if they are detected as stale
--osm-led-mode <arg> Set LED mode for OneStringMiner devices (default: 4)
--pass|-p <arg>     Password for bitcoin JSON-RPC server
--per-device-stats  Force verbose mode and output per-device statistics
--protocol-dump|-P  Verbose dump of protocol-level activities
--quiet|-q          Disable logging output, display status and errors
--quota|-U <arg>    quota;URL combination for server with load-balance strategy quotas
--real-quiet        Disable all output
--rock-freq <arg>   Set RockMiner frequency in MHz, range 125-500 (default: 270.0)
--rotate <arg>      Change multipool strategy from failover to regularly rotate at N minutes
--round-robin       Change multipool strategy from failover to round robin on failure
--sched-start       Set a time of day in HH:MM to start mining (a once off without a stop time)
--sched-stop        Set a time of day in HH:MM to stop mining (will quit without a start time)
--sharelog          Append share log to file
--shares <arg>      Quit after mining N shares (default: unlimited)
--socks-proxy <arg> Set socks4 proxy (host:port)
--suggest-diff <arg> Suggest miner difficulty for pool to user (default: none)
--syslog            Use system log for output messages (default: standard error)
--temp-cutoff       Temperature where a device will be automatically disabled, one value or comma separated list (default: 0)
--text-only|-T      Disable ncurses formatted screen output
--url|-o <arg>      URL for bitcoin JSON-RPC server
--usb <arg>         USB device selection
--user|-u <arg>     Username for bitcoin JSON-RPC server
--userpass|-O <arg> Username:Password pair for bitcoin JSON-RPC server
--verbose           Log verbose output to stderr as well as status output
--widescreen        Use extra wide display without toggling
--worktime          Display extra work time debug information
Options for command line only:
--config|-c <arg>   Load a JSON-format configuration file
See example.conf for an example configuration.
--default-config <arg> Specify the filename of the default config file
Loaded at start and used when saving without a name.
--help|-h           Print this message
--ndevs|-n          Display all USB devices and exit
--version|-V        Display version and exit


and this is what usually gets spit out. an index of command lines to configure your cgminer interface to the network.
