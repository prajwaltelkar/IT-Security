# IT-Security

In this repository I have added some work related to network security.

## Tcpdump

In this experiment we shall some features of tcpdump which is an efficient tool to analyse network traffic and troubleshoot.

#### Tcpdump <br>
<t> tcpdump is a data-network packet analyzer computer program that runs under a command line interface. It allows the user to display TCP/IP and other packets being transmitted or received over a network to which the computer is attached.
<br>
  <br>
  
##### 1.To note the configuration of network and to use tcpdump to start listening for any packets on the interface.
<img src="tcpdump/images/ifconfig.JPG" width="800" height="400"><br>
##### 2.Summary of the capture performed, showing the number of packets captured, filtered, or dropped:
<img src="tcpdump/images/packets.JPG" width="800" height="400"><br>
##### 3.Verbose mode<br>
The verbose flag, you also get all the details of the IP header, like time-to-live, IP ID number, IP options, and IP flags.<br>
The output now provides more details for each packet:<br>
<img src="tcpdump/images/verbose_mode.JPG" width="800" height="400"><br>
##### 4.Filtering<br>
Host 8.8.8.8 specifies that we only want packets where the source or destination IP address matches what we specify (in this case 8.8.8.8).<br>
The port 53 portion means we only want to see packets where the source or destination port matches what we specify (in this case, DNS). These two filter statements are joined together with the logical operator "and". This means that both halves of the filter statement must be true for a packet to be captured by our filter.<br>
<img src="tcpdump/images/filtering.JPG" width="800" height="400"><br>
This uses the dig utility to query a specific DNS server (in this case 8.8.8.8), asking it for the A record for the specified domain (in this case "google.com").
Back in the original terminal, you should now see two captured packets, as our filter rules should filter out any other traffic.<br>
##### 5.Saving captured packets
<img src="tcpdump/images/saving_pcap.JPG" width="800" height="400"><br>
##### 6.pcap_file<br>
A binary file containing the packets we just captured, called http.pcap, will also have been created.<br>
<img src="tcpdump/images/http_pcap.JPG" width="800" height="400"><br>
<img src="tcpdump/images/http_pcap_1.JPG" width="800" height="400"><br>
