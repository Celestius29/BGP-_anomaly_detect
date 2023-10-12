# BGP-_anomaly_detect
Using ML algorithm to detect anomaly in wireless networks.
THis project undertakes a dataset with the following columns:
H+M,H , M,	S,	NoA,	NoW,	NoA NLRI prefixes,	NoW NLRI prefixes,	Avg AS PL,	Max AS PL,	Avg UAS PL,	No DA,	No WA,	No IW,	AED,	MED,	IAT,	No IGP packets,	No EGP packets,	No of Incomplete packets,	Packet size (B),	regular or anomalous.

These columns signify the following:
Columns 1-4: time (column 1: hour+minute; column 2: hour; column 3: minute; column 4: second)
Columns 5-21: features
Column 22: labels for the regular (-1) and anomalous (1) data.
Note that for RNN algorithms, the PyTorch library requires that label (-1) be changed to (0).

List of features extracted from BGP update messages:
5 Number of announcements
6 Number of withdrawals
7 Number of announced NLRI prefixes
8 Number of withdrawn NLRI prefixes
9 Average AS-path length
10 Maximum AS-path length
11 Average unique AS-path length
12 Number of duplicate announcements
13 Number of duplicate withdrawals
14 Number of implicit withdrawals
15 Average edit distance
16 Maximum edit distance
17 Inter-arrival time
18 Number of Interior Gateway Protocol (IGP) packets
19 Number of Exterior Gateway Protocol (EGP) packets
20 Number of incomplete packets
21 Packet size (B)


Link to the dataset: http://www.sfu.ca/~ljilja/cnl/projects/BGP_datasets/index.html
![image](https://github.com/Celestius29/BGP-_anomaly_detect/assets/60284629/3b49a3fe-212b-409e-86a9-ad42be07a69b)
