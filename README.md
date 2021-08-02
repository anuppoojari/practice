# practice
practice piece of code

# Assignment1

### Execution

 ```sh
 python3 random_number.py
 ```

Will return you something like


```sh
[10, 1, 4, 7, 9, 2, 3, 5, 8, 6]
```

# Assignment2

There are few measures we need to take care for our SSL offloading proxy server for the better stability, proxy server is a Crucial Resource. In order to serve the customer centric service it's our duty to keep the application in super relaible with higher performance.

let's monitor the few stats of our SSl offloading server.


1. CPU Stats:\
   SSL Offloading is cpu sensitive process so its important to monitor CPU metrics. (user,system,io,nice)
2. Disk Stats:\
   To measure DISK I/O of the server while performing Encrytion / Decryption. (/proc/diskstats)
3. Filesystem:\
   Filesystem statistics, such as disk space used.To track the disk space of the server from different partitions.
5. Loadaverage:\
   System’s workload for last 15 minutes. (/proc/loadavg or top) Load averages can be useful for a quicker response to avoid the breakdown.
6. netstat:\
   Network statistics from /proc/net/netstat key network metrics from SSL-offloading server
7. meminfo:\
   Exposes the memory statistics	Memory related metrics of server to identify memory issues
8. iostat:\
   To monitor the i/o statustics.
9. Bandtwidth monitoring\
   Number of connections per second
   Queues fullfilment, errors, collisions, drops
   Packet loss, round trip average
10. Network Card\
    IP protocol statistics `/proc/net/snmp`  `/proc/net/netstat`.
    UDP protocol statistics `/proc/net/snmp`  `/proc/net/udp`
    ethtool -S 
    Check hardware interrupt stats `/proc/interrupts
11. Target Host Health\
    5xx Status Codes
    Latency

To Monitor these metrics we can use any enterprise or opensource tools.

`AWS - Cloudwatch` with SNS notification and alert mecahnisam.\
`Zabbix` - One of the tool for metrics monitoring.\
`Wavefront` - Vmware enterprise tool for visualization and metrics monitoring with alert

### Challenges:
- Overall Traffic View 
- Producing Meaningful Context of Events 
- Certificate Management 
- Firewall rules

   
   
 
