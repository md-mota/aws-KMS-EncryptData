# Encrypting DynamoDB Data with AWS KMS 🔑
Secure Data Encryption • IAM Access Control • Key Policy Management

---

## Project Description  
This project walks through how to **encrypt a DynamoDB table using a customer‑managed AWS KMS key** and verify that encryption is enforced through IAM permissions. Instead of simply enabling encryption, the project focuses on **how AWS handles decryption access**, how unauthorized users are blocked, and how key policies determine who can read encrypted data.

To make the workflow clear and practical, the project includes:

- **Creating a symmetric KMS key** to encrypt DynamoDB data  
- **Applying the key to a DynamoDB table** to enable encryption at rest  
- **Adding data** and observing how DynamoDB decrypts it for authorized users  
- **Creating a test IAM user** with DynamoDB access but *no* KMS permissions  
- **Testing access** to show how AWS blocks decryption without key permissions  
- **Updating the KMS key policy** to grant controlled decrypt access  
- **Re‑testing access** to confirm the policy change works  

Overall, this project demonstrates how AWS KMS, DynamoDB, and IAM work together to secure data, enforce least‑privilege access, and protect encrypted resources at the key level.

---

## Workflow Diagrams

**Part 1:** Creating the encryption key and adding admins and users.  
<img src="workflow-diagram1.png" width="500">

**Part 2:** Creating the DynamoDB and encrypting it with KMS.  
<img src="workflow-diagram2.png" width="500">

**Part 3:** Creating test user and giving full access to only DynamoDB.  
<img src="workflow-diagram3.png" width="500">

**Part 4:** Failing to view the table as the test user.  
<img src="workflow-diagram4.png" width="500">

**Part 5:** Modifying the key's policy and granting the test user to decrypt the data.  
<img src="workflow-diagram5.png" width="500">

**Part 6:** Final Diagram for project overview.  
<img src="workflow-diagram6.png" width="500">

---