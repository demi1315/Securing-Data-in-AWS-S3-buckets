# 🔐 Securing Data in AWS S3 Buckets

This repository documents a **cloud security lab focused on protecting data stored in Amazon S3** by applying **core security controls** that prevent unauthorized access, data exposure, and accidental data loss.

The project demonstrates how **S3 bucket misconfigurations can be mitigated** using access control, encryption, versioning, and logging — all implemented using a fresh AWS account and the AWS Management Console.

---

## 🎯 Project Objective

The objective of this project was to:

- Create an S3 bucket with **public access fully blocked**
- Enable **bucket versioning** to protect against accidental deletion or overwrite
- Enforce **server-side encryption using a customer-managed AWS KMS key**
- Apply a **least-privilege bucket policy** for controlled access
- Enable **S3 server access logging** for audit and visibility
- Understand how each control reduces real-world data exposure risk

This project focuses on **data protection and misconfiguration hardening**, not application development.

---

## 🧪 Environment Overview

| Component | Description |
|--------|-------------|
| Cloud Platform | Amazon Web Services (AWS) |
| Storage Service | Amazon S3 |
| Encryption | AWS KMS (customer-managed key) |
| Access Control | Bucket policies |
| Logging | S3 Server Access Logging |
| Account Type | Newly created AWS account |
| Configuration Method | AWS Management Console |

---

## 🧭 Security Controls Implemented

### 🔒 Public Access Restriction
- Created an S3 bucket with **Block All Public Access enabled**
- Prevented accidental public exposure via ACLs or policies

### 🗂️ Data Protection with Versioning
- Enabled bucket versioning
- Ensured recovery capability from accidental deletion or overwrite

### 🔐 Encryption at Rest
- Enabled default server-side encryption
- Used a **customer-managed AWS KMS key**
- Ensured all objects are encrypted automatically

### 👤 Controlled Access via Bucket Policy
- Applied a bucket policy granting `s3:GetObject` access
- Restricted access to a **specific IAM principal (example ARN)**
- Followed least-privilege access principles

### 📊 Audit & Visibility
- Enabled S3 server access logging
- Configured a dedicated log bucket to capture access events
- Improved visibility into object-level access activity

---

## 🧱 Threats Addressed

This project mitigates common S3-related risks such as:

- Public bucket exposure
- Unauthorized data access
- Accidental object deletion
- Lack of encryption at rest
- Missing access visibility and audit trails

---

## ⚠️ Ethical & Usage Notice

- All configurations were performed in a **personal lab AWS account**
- No production or third-party data was used
- Example names and ARNs are for demonstration only
- Project is intended strictly for **defensive cloud security learning**

---

📌 *This repository is part of my cybersecurity portfolio and demonstrates hands-on experience with securing cloud storage against misconfiguration-based data exposure.*


