# cloud-task-4
# CLOUD COMPUTING 
**COMPANY**: CODTECH IT SOLUTIONS
**NAME**: PRINCE KUMAR 
**INTERN ID**: CT08DG546
**DOMAIN**:: Cloud Computing
**DURATION**: 8 WEEKS
**MENTOR**: NEELA SANTOSH

# Task 4 - Cloud Security Implementation
## Steps Completed:
1. Created IAM user with limited permissions.
2. Configured S3 bucket with Block Public Access.
3. Enabled Server Side Encryption.
4. Tested access permissions.
## Why Cloud Security?
- Prevents unauthorized access.
- Encryption keeps data safe at rest.
- IAM ensures only right users get access.

I focused on securing cloud resources — a very important topic in real-world cloud environments. I started by creating an IAM user in AWS instead of using the root account, which is a key security best practice. I attached the minimum required permissions to this user, following the principle of least privilege, which means only giving people or services the access they absolutely need.

Next, I revisited my S3 bucket from Task 1 and made sure Block Public Access was enabled so no accidental public exposure could happen. I then tested permissions to ensure that unauthorized users could not download objects without permission.

To secure the data further, I enabled Server Side Encryption (SSE) for the bucket. I chose SSE-S3, which uses AWS-managed keys, but I also learned how to use SSE-KMS for more control using customer-managed keys. Encryption ensures that even if someone gets unauthorized access to the physical storage, they cannot read the data without the keys.

I tested my configuration by trying to access objects without permissions (it failed) and with the IAM user (it succeeded). I took screenshots to demonstrate IAM user creation, encryption settings, and permission testing. Everything was documented and uploaded to GitHub with a clear README.md.

In an interview, I can explain how IAM, bucket policies, and encryption work together, what the shared responsibility model means, and how to audit cloud resources to maintain security. This task helped me understand practical cloud security measures every engineer should follow.
