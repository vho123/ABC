# GHK Hospital AI Training
Module 4: 7 & 16 Oct 2026
Topic: Copilot Studio Workflows

1. Download required lab1.zip file
2. Unzip it to your OneDrive folder
<img width="310" height="119" alt="image" src="https://github.com/user-attachments/assets/e3e30726-d537-4b50-b3fe-8b6f284fc497" />
<img width="330" alt="image" src="https://github.com/user-attachments/assets/37704187-576c-4ec9-bb21-3ac39d2b5da0" />

2.1 Obtain the excel OneDrive file path,
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/bf1a9d2a-d425-45f6-adea-44e9ff320dc3" />

2.2 Obtain the "NewReport" OneDrive folder path,
<img width="1215" height="604" alt="image" src="https://github.com/user-attachments/assets/988e7266-df2e-461b-9468-8da7333ae39d" />

3. Create Agent - Lab Test Result Entry Agent
<img width="2000" height="937" alt="image" src="https://github.com/user-attachments/assets/6a89a2c8-86fb-41f8-8662-88535e840a44" />

3.1 Update the OneDrive path in skill.MD
<img width="1173" height="607" alt="image" src="https://github.com/user-attachments/assets/5dbe1441-6401-483c-919c-606965155dfd" />


4. Create Agent - Lab Test Result Comparison Agent
<img width="2000" height="651" alt="image" src="https://github.com/user-attachments/assets/ea3aae84-49ec-4faa-b552-2cce3548efa4" />

5. Create Workflow - GHK Lab Result Workflow
<img width="1590" height="381" alt="image" src="https://github.com/user-attachments/assets/290021e5-c237-4589-8632-eee386fabc9a" />

5.1 When a file is created in OneDrive

5.2 Execute Lab Test Result Entry Agent

5.3 Supervisor Review

5.4 If/else condition (Supervisor reviewed okay)

5.4.1 No, then send a team messgae.

5.4.2 Yes, Proceed to file movement and lab report comparison


6. List rows in excel
   
6.1 Execute Lab Test Result Comparison  Agent

6.2 Run Copilot  to generate a summary

6.3 If/else (has history to compare or not)

6.3.1 Has history, post message in Teams.
