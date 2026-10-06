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

<img width="700" height="647" alt="image" src="https://github.com/user-attachments/assets/16db01ca-574d-47ca-b574-c993542c74e7" />

5.2 Execute Lab Test Result Entry Agent

<img width="752" height="529" alt="image" src="https://github.com/user-attachments/assets/abfe578f-a163-4932-b98f-ce5824046890" />

5.3 Supervisor Review

<img width="660" height="725" alt="image" src="https://github.com/user-attachments/assets/09c6a331-1f6a-44f6-90c1-2dd094ce2e1d" />

5.4 If/else condition (Supervisor reviewed okay)

<img width="648" height="498" alt="image" src="https://github.com/user-attachments/assets/ac5c2e1c-0149-44fc-a680-23f4179af2b2" />

5.4.1 No, then send a team messgae.

<img width="643" height="478" alt="image" src="https://github.com/user-attachments/assets/8a83d825-cd3f-44e1-8828-b50196f76bd9" />

5.4.2 Yes, Proceed to file movement and lab report comparison


6. List rows in excel

<img width="634" height="815" alt="image" src="https://github.com/user-attachments/assets/b8c8ac71-0940-4fa9-836d-86bf376e9983" />

6.1 Execute Lab Test Result Comparison  Agent

<img width="711" height="550" alt="image" src="https://github.com/user-attachments/assets/3294f31a-1e78-4826-84cb-1450b9cf4b17" />
<img width="698" height="736" alt="image" src="https://github.com/user-attachments/assets/ecb029b1-081d-4f1d-b959-5e39f1945477" />

6.2 Run Copilot  to generate a summary

<img width="652" height="791" alt="image" src="https://github.com/user-attachments/assets/1592681d-d3ca-4959-bd6a-9eb344c62ebc" />

6.3 If/else (has history to compare or not)

<img width="660" height="467" alt="image" src="https://github.com/user-attachments/assets/209c4611-2939-445c-9015-1ae8bb10e226" />

6.3.1 Has history, post message in Teams.

<img width="704" height="439" alt="image" src="https://github.com/user-attachments/assets/00081a7b-e107-4f44-96b3-2570a4659c76" />

7. File Movement
7.1 Update a row
   
<img width="707" height="715" alt="image" src="https://github.com/user-attachments/assets/df5a8411-d7b0-428e-bb38-422f504812d6" />
<img width="722" height="801" alt="image" src="https://github.com/user-attachments/assets/cbed25db-e24e-4c9b-8c3c-2a8ab7beeeec" />

7.2 List files in OneDrive folder (Processed)

<img width="708" height="465" alt="image" src="https://github.com/user-attachments/assets/566f461f-6660-40c9-9c56-b1d723f3f7fd" />

7.3 Get file content

<img width="716" height="536" alt="image" src="https://github.com/user-attachments/assets/54eba274-46d0-4826-83ed-af4a58a93858" />

7.4 Create new file

<img width="642" height="534" alt="image" src="https://github.com/user-attachments/assets/a0f5de35-ffe5-446b-880a-c031ca57ec14" />

7.5 Delete file

<img width="659" height="363" alt="image" src="https://github.com/user-attachments/assets/4c895e61-5fa9-4ecf-931f-151392200236" />

8. Post a summary to Teams message

<img width="695" height="517" alt="image" src="https://github.com/user-attachments/assets/cc7ff98d-afd4-4ebc-949e-199051478652" />
<img width="693" height="496" alt="image" src="https://github.com/user-attachments/assets/e41af3ff-d94a-4d0e-ae06-1778f5663c88" />






