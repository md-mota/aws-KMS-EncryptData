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