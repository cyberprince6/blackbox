# blackbox
A Basic hack tool which consist of the following features.
1. Port Scanning
2. Network Sniffer
3. Password cracking
4. Email/Phone/Banner
5. Vunerability Scanner
6. Running Service

1. Port Scanning
TCP port scanner that allows you to do stealth scans.

Currently, it can do:

    SYN scanning
    XMAS scanning
    FIN scanning
    NULL scanning
    ACK scanning
    
    usage: blackbox [-h] [--version] -p PORTS PORTS -t TARGET -m MODE
     --ports PORTS PORTS Port interval to scan -t TARGET, --target TARGET Target host -m MODE, --mode MODE scan mode: 1-syn, 2-xmas, 3-fin, 4-null, 5-ack 
    \
   
 2.Network Sniffer
 
 A packet sniffer. Collect packets until ctrl+c pressed or after -t seconds

usage:
optional arguments:
  -h, --help            show this help message and exit
  -f FILENAME, --filename FILENAME
                        pcap file name (don't give extension)
  -nr, --noraw          No Raw mode, Stops printing raw packets
  -t TIME, --time TIME  Capture time in second
  \

3.Password cracking

Command line is fairly straight forword, here are the options:

-h [hash]

-t [type]

-w [wordlist]

-n [numbers bruteforce, used in place of -w]

-v [verbose, slows down cracking time though :( ]

-i [help and info]

usage:
Hashcrack with a wordlist and verbose mode

-h <hash> -t <hash_type> -w <Wordlist.txt> -v 
