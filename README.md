# terraform-project-1

# 🌐 Terraform AWS S3 Static Website

This project demonstrates how to deploy a static website on AWS S3 using Terraform. It follows Infrastructure as Code (IaC) principles to automate the creation and configuration of cloud resources.

---

## 🚀 Features

* Creates an S3 bucket
* Enables static website hosting
* Configures public access
* Uploads HTML file automatically
* Outputs website URL after deployment

---

## 🛠️ Tech Stack

* Terraform
* AWS S3
* AWS CLI

---

## 📁 Project Structure

```
terraform-project-1/
│── main.tf
│── variables.tf
│── outputs.tf
│── terraform.tfvars
│── index.html
│── .gitignore
```

---

## ⚙️ Prerequisites

* AWS Account
* AWS CLI installed and configured
* Terraform installed

---

## 🚀 Deployment Steps

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/kunal015-P/terraform-project-1.git
cd terraform-project-1
```

---

### 2️⃣ Configure AWS Credentials

```bash
aws configure
```

Provide:

* AWS Access Key
* AWS Secret Key
* Region: ap-south-1

---

### 3️⃣ Add Terraform Variables

Create a file named `terraform.tfvars`:

```hcl
bucket_name = "your-unique-bucket-name"
```

> ⚠️ Bucket name must be globally unique

---

### 4️⃣ Initialize Terraform

```bash
terraform init
```

---

### 5️⃣ Review Plan

```bash
terraform plan
```

---

### 6️⃣ Apply Configuration

```bash
terraform apply
```

Type `yes` when prompted.

---

### 7️⃣ Access Website

After deployment, Terraform will output:

```
website_url = http://<your-bucket-name>.s3-website-ap-south-1.amazonaws.com
```

Open it in your browser 🌐

---

### 8️⃣ Destroy Resources (Cleanup)

```bash
terraform destroy
```

---

## 🧠 What You Learn

* Terraform basics (providers, resources, variables, outputs)
* AWS S3 configuration
* Static website hosting
* Infrastructure as Code workflow

---

## ⚠️ Important Notes

* Do NOT commit `.terraform/` folder
* Do NOT commit `terraform.tfvars`
* Always destroy resources to avoid AWS charges

---

## 💡 Future Improvements

* Add CloudFront (CDN)
* Enable HTTPS
* Use custom domain
* Convert into reusable Terraform modules

---

## 📌 Author

Kunal

---
