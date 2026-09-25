# AWS-IAM-POLICIES
This repository demonstrates how AWS IAM policies work and how to configure them

First, log into your AWS portal
<img width="958" height="1079" alt="image" src="https://github.com/user-attachments/assets/ba82960c-2662-41e7-b1e1-9be8ddf8f434" />
In the search bar, type IAM and select the service
<img width="964" height="1030" alt="image" src="https://github.com/user-attachments/assets/f89f408d-ea1c-4b72-8d0e-895255703c6c" />
On the left navigation pane, under Access Management, select Policies
<img width="962" height="1033" alt="image" src="https://github.com/user-attachments/assets/da9573b4-2a75-4246-ac42-82995a98e09e" />
This page displays the Policies section of the AWS Identity and Access Management console. For this example, I will be selecting the AdministratorAccess policy
<img width="971" height="1078" alt="image" src="https://github.com/user-attachments/assets/1e743b40-2471-4a20-b190-71c8c46af9f9" />
Once you select the policy, it will display its details. IAM policies define allowed or denied AWS actions and grant permissions once attached to an IAM User, Group, or Role

In this scenario, we are working with AdministratorAccess so this allows access to all the services in AWS and the Access level is set to Full access
<img width="1920" height="874" alt="image" src="https://github.com/user-attachments/assets/f9661b30-91d0-4178-9bcb-32aadb0f75d3" />
You can see how this policy is defined by right-clicking the JSON tab
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/3ed44dd9-f9eb-4c1a-9c73-c850eaa7c9ba" />
Once the page has loaded, you will see the JSON format of this policy
<img width="1494" height="392" alt="image" src="https://github.com/user-attachments/assets/49c3959c-672f-4439-9b1d-92b2277f73f8" />
Version: Specifies the IAM policy language version. 2012-10-17 is the current standard version and enables advanced features like policy variables

Statement: The main container for the policy rules. This can hold multiple individual permission blocks inside an array []

Effect ("Allow"): Specifies whether permissions are granted or denied

Action ("asterick"): Defines the permitted actions, while the "asterick" grants access to all AWS actions)

Resource ("asterick"): Identifies the target AWS resources to which the actions apply. The "asterick" applies permissions to all resources


For comparison, I will use the IAMReadOnlyAccess policy, showing the allowed services, access level, and its defined JSON format

In this screenshot, you can see that there is only one allowed service and the access level is set to Full: List Limited: Read
<img width="1920" height="1038" alt="image" src="https://github.com/user-attachments/assets/f8f33616-55cf-43f0-a767-a999d3d4688e" />
