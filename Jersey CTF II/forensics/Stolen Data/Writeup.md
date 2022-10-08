**Title:** Stolen Data

*Description:* Someone accessed the server and stole the flag. Use the network packet capture to find it.

*Solution:* 
We are given the file stolen_data.pcap, which we need to analyze to find the flag. Hmm, TCP streams look interesting, but there are too many.
Let's try looking through the Statistics > Conversations. Ooh, port 4444 looks very interesting. Let's try to view the TCP stream for it.

![image](https://user-images.githubusercontent.com/86359182/194690091-eb57b5bf-717c-4ea6-b0cf-c0956b1de811.png)

There is a PDF in this stream! Let's export it as a file and view it.

And there we go! We have our flag!

Flag: ```jctf{0v3r_7h3_w1r3}```
