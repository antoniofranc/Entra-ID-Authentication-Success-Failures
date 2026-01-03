<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/49978ebf-884f-49bc-8780-50bc818117d0" />

# Azure Sentinel Attack Maps Project
A comprehensive guide to creating interactive attack maps in Microsoft Sentinel using KQL queries to visualize authentication activity, resource creation, and malicious traffic across your Azure environment.

## 📋 Project Overview
This project demonstrates how to build five different attack maps in Azure Sentinel to monitor and visualize security events:

1. Entra ID Authentication Successes - Successful login attempts across the tenant
2. Entra ID Authentication Failures - Failed login attempts from around the world
3. Azure Resource Creation - Geographic visualization of resource deployment activity
4. VM Authentication Failures - Failed RDP/SSH attempts from bad actors and bots
5. Malicious Network Traffic - Suspicious traffic entering your network

-----
## 📊 Attack Maps
## 1. Entra ID Authentication Success Map

Authentication Success (Json) https://github.com/joshmadakor1/lognpacific-public/blob/main/cyber-range/sentinel/Directory-Login-Successes.json

<img width="500" height="794" alt="image" src="https://github.com/user-attachments/assets/d28e8ffc-f2df-4228-a242-8f938c1b996b" />
<img width="1486" height="564" alt="image" src="https://github.com/user-attachments/assets/3e51312a-db0e-47a8-ab22-04807aacd599" />

Visualizes successful login attempts across your Azure tenant, showing:
- User identity and geographic location
- Login frequency by region
- Latitude/longitude coordinates for precise mapping

## 2. Entra ID Authentication Failures Map

Authentication Failures (Json) https://github.com/joshmadakor1/lognpacific-public/blob/main/cyber-range/sentinel/Directory-Login-Failures.json

<img width="500" height="769" alt="image" src="https://github.com/user-attachments/assets/054e57b9-6826-408e-b61e-e168ffe566c7" />
<img width="1715" height="543" alt="image" src="https://github.com/user-attachments/assets/fcc86e41-7735-4739-9931-37f26ab1c70e" />

Displays failed authentication attempts, helping identify:
- Potential brute force attacks
- Suspicious login patterns
- Geographic anomalies in access attempts

## 3. Azure Resource Creation / Deletions

Azure Resource Creation (Json): https://github.com/joshmadakor1/lognpacific-public/blob/main/cyber-range/sentinel/Azure-Resource-Creation.json

<img width="500" height="793" alt="image" src="https://github.com/user-attachments/assets/ed6c9c69-0612-4a5d-a21f-49bc4a0ada3c" />
<img width="1527" height="585" alt="image" src="https://github.com/user-attachments/assets/0e347566-d082-47bd-bd57-43544add55c8" />

Tracks where Azure resources are being deployed from:
- Resource creation locations
- Deployment patterns
- Organizational activity monitoring

## 4. VM Authentication Failures

VM Authentication Failures (Json): https://github.com/joshmadakor1/lognpacific-public/blob/main/cyber-range/sentinel/VM-Authentication-Failures.json

<img width="500" height="721" alt="image" src="https://github.com/user-attachments/assets/cf68ba0f-0e10-484c-8950-9ba0a55ca0e4" />
<img width="1225" height="538" alt="image" src="https://github.com/user-attachments/assets/623fcf1c-b14d-446e-ba9b-fcf022d5b09f" />

Captures failed login attempts to virtual machines:
- Bot and malicious actor activity
- RDP/SSH brute force attempts
- Student and legitimate user failures

## 5. Malicious Network Traffic - Suspicious traffic entering your network
       (Json): https://github.com/joshmadakor1/lognpacific-public/blob/main/cyber-range/sentinel/Allowed-Inbound-Malicious-Flows.json
<img width="500" height="808" alt="image" src="https://github.com/user-attachments/assets/a59b6bb4-cb33-49ed-ba85-1361ff0d3aaa" />
<img width="1120" height="531" alt="image" src="https://github.com/user-attachments/assets/e8057029-98ba-49e6-a679-966adb4f0e0e" />
