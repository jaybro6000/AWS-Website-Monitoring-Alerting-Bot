# AWS Website Monitoring & Alerting Bot

Serverless **Website Watchdog** built with **AWS CloudWatch Synthetics** & **SNS**. Uses **Node.js/Puppeteer** canaries to monitor 24/7 uptime. Includes **CloudWatch Alarms** for instant email alerts via **SNS** upon failure. Proven via fault-injection testing with 100% detection accuracy. ✨

---

## 📸 Project Workflow

### 1. Designing the Trap
Shows the creation of the Amazon SNS topic `Website-Status-Alerts` to handle notification dispatching.

<img width="1920" height="858" alt="Project_The_Website_Up_Down_Alert_Bot_photo_2" src="https://github.com/user-attachments/assets/f205295b-204b-432f-afe0-d3e3deebbddf" />


### 2. Setting Up the Hook
Shows the Amazon SNS subscription confirmation, ensuring the email endpoint is verified to receive alerts.

<img width="1920" height="861" alt="Project_The_Website_Up_Down_Alert_Bot_photo_3" src="https://github.com/user-attachments/assets/6b0a3f0d-2c6a-4ab7-99da-0864c130b99a" />


### 3. Deploying the Canary
Shows the configuration of the CloudWatch Synthetic Canary (`website-watchdog`) utilizing the heartbeat monitoring blueprint.

<img width="1920" height="861" alt="Project_The_Website_Up_Down_Alert_Bot_photo_5" src="https://github.com/user-attachments/assets/ddcfb2e7-8658-4e71-8f13-80680517ceeb" />


### 4. Configuring the Watchdog
Shows attaching the CloudWatch Alarm and SNS topic to the canary to define the failure threshold.

<img width="1920" height="858" alt="Project_The_Website_Up_Down_Alert_Bot_photo_4" src="https://github.com/user-attachments/assets/e192f730-a867-4b0e-95b8-4c02c2d921ad" />


### 5. Verified Healthy State
Shows the Synthetics console indicating a 100% success rate while monitoring the target website.

<img width="1920" height="935" alt="Project_The_Website_Up_Down_Alert_Bot_photo_6" src="https://github.com/user-attachments/assets/4b157d45-443f-4830-8845-db6e28f66fcf" />


### 6. Simulating a Failure
Shows editing the canary script to point to a non-existent URL to force a failure scenario.

<img width="1920" height="863" alt="Project_The_Website_Up_Down_Alert_Bot_photo_8" src="https://github.com/user-attachments/assets/c80fce71-996a-4855-a2b8-ac5dd84c23ca" />

### 7. Detection of Downtime
Shows the canary run status changing to "Failed" in the CloudWatch console.

<img width="1920" height="843" alt="Project_The_Website_Up_Down_Alert_Bot_photo_9" src="https://github.com/user-attachments/assets/70e0f7bf-b0c2-48d5-b72c-528a3186a563" />


### 8. Real-time Alert Received
Shows the email alert received instantly in the inbox, proving the end-to-end integration works.

<img width="1531" height="770" alt="Project_The_Website_Up_Down_Alert_Bot_photo_7" src="https://github.com/user-attachments/assets/532a2217-cb83-48f6-9b12-4db7e17f242a" />
