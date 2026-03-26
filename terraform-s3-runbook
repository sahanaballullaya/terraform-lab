# Terraform S3 Bucket Lab — Runbook

Author: Sahana  
Environment: AWS CloudShell  
Last Updated: 2026-03-26  

---

## Objective

Provision and destroy an AWS S3 bucket using Terraform and understand the full Infrastructure as Code (IaC) workflow.

---

## Prerequisites

- AWS account access  
- AWS CloudShell or local terminal  
- Terraform installed  

Verify Terraform:
terraform -version

---

## Project Setup

Step 1 — Create Working Directory

mkdir simple-tf
cd simple-tf

Step 2 — Create Terraform File

nano main.tf

Add:

provider "aws" {
  region = "us-east-1"
}

resource "aws_s3_bucket" "demo" {
  bucket = "sahana-simple-bucket-12345"

  tags = {
    Name = "terraform-lab"
    Env  = "test"
  }
}

---

## Terraform Workflow

terraform init
terraform fmt
terraform validate
terraform plan
terraform apply

Type yes

terraform output

---

## Verification

Check AWS S3 console for bucket.

---

## Cleanup

terraform destroy

Type yes

---

## Key Learnings

- init → plan → apply → destroy workflow
- Infrastructure as Code concept
- State management

---

## Interview Talking Point

I used Terraform to provision an AWS S3 bucket and executed the full lifecycle including init, plan, apply, and destroy.
