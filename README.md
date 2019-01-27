
# Buildscript

vulnerability scanner tool is using nmap and nse scripts to find vulnerabilities

This tool puts an additional value into vulnerability scanning with nmap. 
It uses NSE scripts which can add flexibility in terms of vulnerability detection and exploitation.
Below there are some of the features that NSE scripts provide  

- Network discovery
- More sophisticated version detection
- Vulnerability detection
- Backdoor detection
- Vulnerability exploitation

This tool uses the path ```/usr/share/nmap/scripts/``` where the nse scripts are located in kali linux 

The tool performs the following 

- check the communication to the target hosts by cheking icmp requests
- takes as input a protocol name such as http and executes all nse scripts related to that protocol
- if any vulnerability triggers it saves the output into a log file
- it may perform all of the above actions for a range of IP addresses
 

###Usage: 

```[Usage:] ./buildscript.sh <ip_range> <protocol> <port> <Pn (optional)>```



###How to run:

1)
```./buildscript.sh 192.168.162.90 http 80``` 

2)
```./buildscript.sh 192.168.162.10-90 http 80```


###References :
- https://nmap.org/book/nse.html
- https://nmap.org/nsedoc/



