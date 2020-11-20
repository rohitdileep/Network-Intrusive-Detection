# Network-Intrusive-Detection

BUSINESS CONTEXT:  

With the enormous growth of computer networks usage and the huge increase in the number of
applications running on top of it, network security is becoming increasingly more important. All
the computer systems suffer from security vulnerabilities which are both technically difficult and
economically costly to be solved by the manufacturers. Therefore, the role of Intrusion Detection
Systems (IDSs), as special-purpose devices to detect anomalies and attacks in the network, is
becoming more important.
The research in the intrusion detection field has been mostly focused on anomaly-based and
misusebased detection techniques for a long time. While misuse-based detection is generally
favored in commercial products due to its predictability and high accuracy, in academic research
anomaly detection is typically conceived as a more powerful method due to its theoretical
potential for addressing novel attacks.
Conducting a thorough analysis of the recent research trend in anomaly detection, one will
encounter several machine learning methods reported to have a very high detection rate of 98%
while keeping the false alarm rate at 1%. However, when we look at the state of the art IDS
solutions and commercial tools, there is no evidence of using anomaly detection approaches, and
practitioners still think that it is an immature technology. To find the reason of this contrast, lots
of research was done done in anomaly detection and considered various aspects such as learning
and detection approaches, training data sets, testing data sets, and evaluation methods.

BUSINESS PROBLEM:

Your task to build network intrusion detection system to detect anamolies and attacks in the
network. There are two problems.
1. Binomial Classification: Activity is normal or attack
2. Multinomial classification: Activity is normal or DOS or PROBE or R2L or U2R
Please note that, currently the dependent variable (target variable) is not definied explicitly.
However, you can use attack variable to define the target variable as required.

LIST OF COLUMNS FOR THE DATA SET:
["duration","protocol_type","service","flag","src_bytes","dst_bytes","land",
"wrong_fragment","urgent","hot","num_failed_logins","logged_in",
"num_compromised","root_shell","su_attempted","num_root","num_file_creations",
"num_shells","num_access_files","num_outbound_cmds","is_host_login",
"is_guest_login","count","srv_count","serror_rate", "srv_serror_rate",
"rerror_rate","srv_rerror_rate","same_srv_rate", "diff_srv_rate", 
"srv_diff_host_rate","dst_host_count","dst_host_srv_count","dst_host_same_srv_rate",
"dst_host_diff_srv_rate","dst_host_same_src_port_rate",
"dst_host_srv_diff_host_rate","dst_host_serror_rate","dst_host_srv_serror_rate",
"dst_host_rerror_rate","dst_host_srv_rerror_rate","attack", "last_flag"]


Type Features:
Nominal: Protocol_type(2), Service(3), Flag(4)
Binary: Land(7), logged_in(12), root_shell(14), su_attempted(15), is_host_login(21),, is_guest_login(22)
Numeric:Duration(1), src_bytes(5), dst_bytes(6), wrong_fragment(8), urgent(9), hot(10),
num_failed_logins(11), num_compromised(13), num_root(16), num_file_creations(17),
num_shells(18), num_access_files(19), num_outbound_cmds(20), count(23), srv_count(24), error_rate(25),
srv_serror_rate(26), rerror_rate(27),srv_rerror_rate(28), same_srv_rate(29),diff_srv_rate(30),
srv_diff_host_rate(31), dst_host_count(32), dst_host_srv_count(33), dst_host_same_srv_rate(34),
dst_host_diff_srv_rate(35), dst_host_same_src_port_rate(36), dst_host_srv_diff_host_rate(37),
dst_host_serror_rate(38), dst_host_srv_serror_rate(39), dst_host_rerror_rate(40),
dst_host_srv_rerror_rate(41)

Attack Class:

DOS : Black,Land,Neptune,Smurf,Teardrop,Apache,Storm,Processatable,Worm
Probe : Satan,Ipsweep,Nmap,Portsweep,Mscan,Saint
R2L : Guess_Password,Ftp_write,Imap,Phf,Multihop,Warezmaster,Warezclient,Spy,Xlock,Xspnoon,Snpmguess,Snpmgetattack,Htttunnel,Sendmail,Named
U2R : Buffer_overflow,Loadmodule,Rootkit,Perl,SQLattack,Stem.
