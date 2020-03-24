# InavitasTask
This is a task which provided by a company for IIot section with kafka using  java

Write an application which reads data from CSV file and push the data to Kafka in JSON format below.
Requirements are like :
• CSV file includes columns are deviceId, timestamp and several dataNames. You should read CSV file and
parse the data to convert JSON file like below.
•
•
•
• Data should be produced into a topic name sample-data to Kafka.
All the data of each deviceId in file should be produced concurrently.
You should be careful about performance of application.
Source code of application should be provided in Github.
{
"deviceId":100001,
" dataTime ": 1584901399000,
"dataList":[
{
"dataName":”CurrentA”, // will be header of data is like CurrentA,CurrentB ..
},
{
" dataName ":”CurrentB”, // will be header of data is like CurrentA,CurrentB ..
"dataValue":123.456
}
]
}




Sample data:-

DeviceID	DataTime	CurrentA	CurrentB	CurrentC	ActivePower	AppearentPower	ReactivePower	VoltageA	VoltageB	VoltageC
100628	2020-02-01 00:10:00	274.498	279.786	261.852	15.187	15.199	-0.582	18.652	18.657	18.651
100628	2020-02-01 00:20:00	267.839	271.889	254.033	14.792	14.807	-0.643	18.689	18.686	18.68
100628	2020-02-01 00:30:00	260.458	263.174	245.619	14.331	14.342	-0.531	18.69	18.683	18.666
100628	2020-02-01 00:40:00	256.191	259.734	241.034	14.124	14.131	-0.428	18.72	18.709	18.691
100628	2020-02-01 00:50:00	249.245	251.743	233.788	13.72	13.726	-0.387	18.738	18.724	18.707
100628	2020-02-01 01:00:00	240.835	243.497	225.858	13.307	13.309	-0.156	18.801	18.787	18.766
100628	2020-02-01 01:10:00	238.119	237.49	221.01	13.041	13.044	-0.285	18.795	18.775	18.745
100628	2020-02-01 01:20:00	232.518	231.765	215.565	12.706	12.716	-0.503	18.776	18.761	18.735
100628	2020-02-01 01:30:00	209.231	207.355	192.037	11.313	11.336	-0.705	18.709	18.69	18.658
100628	2020-02-01 01:40:00	186.531	184.977	169.265	10.055	10.078	-0.677	18.743	18.724	18.692
100628	2020-02-01 01:50:00	178.802	177.14	162.716	9.662	9.683	-0.643	18.786	18.768	18.738
100628	2020-02-01 02:00:00	183.453	183.807	169.171	10.031	10.041	-0.428	18.832	18.817	18.785
100628	2020-02-01 02:10:00	187.342	185.099	171.882	10.182	10.192	-0.432	18.843	18.832	18.802
100628	2020-02-01 02:20:00	186.575	184.128	171.605	10.134	10.15	-0.557	18.842	18.837	18.798
100628	2020-02-01 02:30:00	171.527	168.464	156.568	9.275	9.286	-0.438	18.858	18.852	18.813
100628	2020-02-01 02:40:00	165.869	164.05	151.442	8.995	8.999	-0.259	18.876	18.872	18.833
100628	2020-02-01 02:50:00	161.581	159.405	146.505	8.726	8.735	-0.381	18.876	18.869	18.825
100628	2020-02-01 03:00:00	180.475	177.786	167.046	9.828	9.839	-0.453	18.891	18.893	18.848
100628	2020-02-01 03:10:00	174.264	172.034	161.443	9.489	9.497	-0.372	18.905	18.906	18.863
100628	2020-02-01 03:20:00	172.845	171.359	160.525	9.438	9.446	-0.382	18.916	18.92	18.88
100628	2020-02-01 03:30:00	171.084	169.423	158.612	9.344	9.352	-0.393	18.922	18.924	18.883
100628	2020-02-01 03:40:00	166.423	164.179	153.242	9.05	9.06	-0.426	18.927	18.927	18.886
100628	2020-02-01 03:50:00	167.813	165.703	154.379	9.125	9.135	-0.44	18.935	18.931	18.891
100628	2020-02-01 04:00:00	185.411	183.305	172.042	10.134	10.148	-0.53	18.955	18.952	18.91
100628	2020-02-01 04:10:00	192.61	191.68	179.681	10.592	10.601	-0.425	18.961	18.959	18.919
100628	2020-02-01 04:20:00	176.248	175.36	163.348	9.669	9.672	-0.186	18.971	18.97	18.929

