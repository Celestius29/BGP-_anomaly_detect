# BGP-_anomaly_detection
Using ML algorithm to detect anomaly in wireless networks.
THis project undertakes a dataset with the following columns:
H+M,H , M,	S,	NoA,	NoW,	NoA NLRI prefixes,	NoW NLRI prefixes,	Avg AS PL,	Max AS PL,	Avg UAS PL,	No DA,	No WA,	No IW,	AED,	MED,	IAT,	No IGP packets,	No EGP packets,	No of Incomplete packets,	Packet size (B),	regular or anomalous.<br>

These columns signify the following:<br>
Columns 1-4: time (column 1: hour+minute; column 2: hour; column 3: minute; column 4: second)<br>
Columns 5-21: features<br>
Column 22: labels for the regular (-1) and anomalous (1) data.<br>
Note that for RNN algorithms, the PyTorch library requires that label (-1) be changed to (0).<br>

List of features extracted from BGP update messages:<br>
5 Number of announcements<br>
6 Number of withdrawals<br>
7 Number of announced NLRI prefixes<br>
8 Number of withdrawn NLRI prefixes<br>
9 Average AS-path length<br>
10 Maximum AS-path length<br>
11 Average unique AS-path length<br>
12 Number of duplicate announcements<br>
13 Number of duplicate withdrawals<br>
14 Number of implicit withdrawals<br>
15 Average edit distance<br>
16 Maximum edit distance<br>
17 Inter-arrival time<br>
18 Number of Interior Gateway Protocol (IGP) packets<br>
19 Number of Exterior Gateway Protocol (EGP) packets<br>
20 Number of incomplete packets<br>
21 Packet size (B)<br>


Link to the dataset: (http://www.sfu.ca/~ljilja/cnl/projects/BGP_datasets/index.html)
![image](https://github.com/Celestius29/BGP-_anomaly_detect/assets/60284629/3b49a3fe-212b-409e-86a9-ad42be07a69b)

Use the code provided for the 3 different datasets we have for the 3 different ransomware attacks. Visualizations and results will be attached.
