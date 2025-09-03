

[AWS CDK Crash Course for Beginners](https://www.youtube.com/watch?v=D4Asp5g4fp8)  
Note: I went through the above crash course, and during the interview, it will help as a quick refresher and reference. Hope it is not a content violation 

<img width="1190" height="452" alt="image" src="https://github.com/user-attachments/assets/baa381da-34d5-407e-993c-91bcb08a0c49" />  

<img width="1114" height="616" alt="image" src="https://github.com/user-attachments/assets/1b5ff2d0-dfbc-4428-b81e-fda882c8a530" />  


<img width="772" height="517" alt="image" src="https://github.com/user-attachments/assets/ce7b41b3-06f4-4610-920f-f8db060bb173" />  

<img width="537" height="629" alt="image" src="https://github.com/user-attachments/assets/43180583-89a6-4ef3-95a0-af7fe5586612" />  

<img width="1267" height="725" alt="image" src="https://github.com/user-attachments/assets/86bd29f6-184b-4c1d-92b0-45ee78a8e11a" />  


<img width="1200" height="685" alt="image" src="https://github.com/user-attachments/assets/82203b6b-9217-4c7a-8408-af5dae3b15e2" />


<img width="1223" height="645" alt="image" src="https://github.com/user-attachments/assets/473c8948-ae30-4388-982b-b4ff73706bed" />

<img width="1249" height="630" alt="image" src="https://github.com/user-attachments/assets/24067abf-e749-406c-97ff-2e678ddbea09" />  

<img width="1246" height="649" alt="image" src="https://github.com/user-attachments/assets/747a1d1a-e386-410d-b111-0bd31d662387" />


<img width="1243" height="808" alt="image" src="https://github.com/user-attachments/assets/c1a2dda2-b5c8-4845-bcd6-e28cd4c91d28" />


<img width="1249" height="713" alt="image" src="https://github.com/user-attachments/assets/99d3b028-b07f-4481-809d-3f2c5794867d" />

<img width="1197" height="658" alt="image" src="https://github.com/user-attachments/assets/7cf42125-32d3-428f-abde-93db8d394fbd" />

<img width="1291" height="768" alt="image" src="https://github.com/user-attachments/assets/b6ba04d4-3df2-4c39-ade6-8a8edba2d6b6" />  

<img width="1204" height="692" alt="image" src="https://github.com/user-attachments/assets/bffa704b-2b8a-4066-bc01-9dbe7a917098" />

CDK Watch
CDK Migrate

<img width="1225" height="233" alt="image" src="https://github.com/user-attachments/assets/749b9f15-2cb8-4563-ba53-57d32426b670" />


<img width="1236" height="615" alt="image" src="https://github.com/user-attachments/assets/a22d5c58-34c3-4248-829d-e686bf6dec1b" />

[Warp Tool](https://www.warp.dev/)
<img width="1230" height="635" alt="image" src="https://github.com/user-attachments/assets/3a2ece76-d7e0-4441-a70e-b77c1649206d" />


Create Folder, Project, Initiate the CDK Project

<img width="969" height="641" alt="image" src="https://github.com/user-attachments/assets/e6024a72-7a9e-4994-a0cf-439d021e8bec" />

CDK.json - CDK Configuration, Specification for CDK

<img width="1230" height="643" alt="image" src="https://github.com/user-attachments/assets/e61520af-a0d8-4dea-868c-c18b3afee2aa" />

<img width="1217" height="636" alt="image" src="https://github.com/user-attachments/assets/4ee64174-cf90-484c-b507-4c92e7535132" />

CDK Unit Testcases - Generates the CloudFormation Template and Testcases, and verifies if the corresponding property is available within the generated CloudFormation template
<img width="1227" height="649" alt="image" src="https://github.com/user-attachments/assets/a261b27e-05ce-4fab-b0e0-fee56f7e114b" />

Bin contains your app, and lib contains your stacks
<img width="1223" height="637" alt="image" src="https://github.com/user-attachments/assets/c655b1c3-80fd-48d8-a55c-c8fcf850b351" />


One Project can only have one app, but one project can have multiple stacks within the project.

<img width="1226" height="638" alt="image" src="https://github.com/user-attachments/assets/577bfc87-cdac-45eb-b25f-aa21bbd6d68d" />
The The 
Main Stack that one has to build will be part of the stack under the lib folder.
<img width="1225" height="696" alt="image" src="https://github.com/user-attachments/assets/d0723efc-6938-4492-b489-0570b47b8e6d" />
Important CDK Commands

CDK List Stack
CDK BootStack - which bootstraps
CDK Deploy - It will deploy all the resources

<img width="1219" height="614" alt="image" src="https://github.com/user-attachments/assets/7ac31dcb-dd83-4dc2-914f-4b04d1c78f66" />

### CDK Help

The image shows the output of the `cdk help` command, which lists all available AWS CDK (Cloud Development Kit) CLI commands. Here's a breakdown of the key commands and their purposes:

---

### **AWS CDK CLI Commands**

| Command | Description |
|--------|-------------|
| `cdk list [STACKS..]` | Lists all stacks in your CDK app. Alias: `ls`. |
| `cdk synthesize [STACKS..]` | Generates and prints the CloudFormation template for the specified stack(s). Alias: `synth`. |
| `cdk bootstrap [ENVIRONMENTS..]` | Deploys the CDK toolkit stack into an AWS environment (required before deploying stacks). |
| `cdk deploy [STACKS..]` | Deploys the specified stack(s) to your AWS account. |
| `cdk import [STACK]` | Imports existing AWS resources into a CDK stack. |
| `cdk watch [STACKS..]` | Shortcut for `deploy --watch`, automatically deploys changes when files are updated. |
| `cdk destroy [STACKS..]` | Destroys the specified stack(s) in AWS. |
| `cdk diff [STACKS..]` | Compares the local stack definition with the deployed version or a local template file. Returns exit code 1 if differences are found. |
| `cdk metadata [STACK]` | Retrieves metadata associated with a stack. |
| `cdk acknowledge [ID]` | Acknowledges a notice so it won’t appear again. Alias: `ack`. |
| `cdk notices` | Lists relevant notices or warnings from the CDK. |
| `cdk init [TEMPLATE]` | Creates a new, empty CDK project based on a template (e.g., `app`, `api`, etc.). |
| `cdk context` | Manages cached context values used during synthesis. |
| `cdk docs` | Opens the official CDK reference documentation in a browser. Alias: `doc`. |
| `cdk doctor` | Checks your CDK setup for potential issues and provides suggestions. |

---

### **Usage Tips**
- Use `cdk synth` to preview what will be deployed without modifying AWS.
- Use `cdk diff` to see changes between your current code and the deployed state.
- Always run `cdk bootstrap` once per AWS environment before deploying any stacks.
- Use `cdk watch` during development for faster iteration.

Let me know if you'd like examples or explanations for any specific command!



<img width="1220" height="643" alt="image" src="https://github.com/user-attachments/assets/b1f0664d-e2a1-410b-b0a4-0ab1d946990d" />











