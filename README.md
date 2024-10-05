<h1>Geo IP Data Ingestion and Log Analytics and Microsoft Sentinel (SIEM) Setup</h1>
This tutorial outlines the configuration of our Log Analytics Workspace and Microsoft Sentinel

<h2>Environments and Technologies Used</h2>

- <b>Microsoft Azure</b> 
- <b>Log Analytics Workspace</b>
- <b>Microsoft Sentinel</b>

<h2>Operating Systems</h2>

- <b>Windows 10</b>


<h2>Configuration Steps</h2>

- <b>Download this file onto your PC: https://github.com/joshmadakor1/Cyber-Course-v2/blob/main/Sentinel-Maps(JSON)/geoip-summarized.csv</b>

![image](https://github.com/user-attachments/assets/b057eca4-fad8-4301-8d8e-f41710d259fc)
- <b>Navigate to Log Analytics Workspace and click create</b>
- <b>Resource Group: RG-Cyber-Lab</b>
- <b>Name: LAW-Cyber-Lab-01</b>
- <b>Region: EAST US 2</b>

![image](https://github.com/user-attachments/assets/984d76f5-906b-45b1-a3ce-d1237e52c86e)
- <b>Navigate to Microsoft Sentinel and click "Create"</b>
- <b>Add Microsoft Sentinel to LAW-Cyber-Lab-01 workspace</b>

![image](https://github.com/user-attachments/assets/29ec2424-3768-48ce-aff8-355be63e3f33)
- <b>Click "Watchlist" and "New"</b>

![image](https://github.com/user-attachments/assets/150e0b62-a54f-4735-851a-abd11137fed1)
- <b>Name/Alias: geoip</b>
- <b>Source Type: Local File</b>
- <b>Number of lines before row: 0</b>
- Upload geoip summarized.csv file</b>
- <b>Search key: network</b>

![image](https://github.com/user-attachments/assets/24920579-c510-4f1d-b13b-35286f38970e)
- <b>55k Watchlist Items</b>

![image](https://github.com/user-attachments/assets/186d936a-097e-4b90-8a81-ddc4e4a7a377)
- <b>Navigate to Log Analytics Workspace and query _GetWatchlist("geoip")

![image](https://github.com/user-attachments/assets/4042ac65-bc1a-4afa-afaa-91514f3eb403)
- <b>Count results</b>



