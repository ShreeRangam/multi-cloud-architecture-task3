# multi-cloud-architecture-task3
# 🌐 Multi-Cloud Architecture Project – Task 3

## 🚀 Project Overview

This project demonstrates a simple **multi-cloud architecture** using **Amazon Web Services (AWS)** and **Microsoft Azure**. The goal is to distribute services across two different cloud platforms and showcase how they can work together seamlessly.

---

## 🧱 Architecture

- **Frontend** (Static Website): Hosted on **AWS S3**
- **Backend API**: Hosted on **Azure Function App**

The frontend sends a request to the backend API hosted on another cloud provider and displays the result.

---

## 📌 Objectives

- ✅ Design a multi-cloud setup
- ✅ Deploy services across AWS and Azure
- ✅ Demonstrate interoperability (communication between services on different platforms)

---

## 🔧 Technologies Used

- **AWS S3** – for hosting the static website
- **Azure Function App** – for backend API
- **GitHub** – for version control and documentation

---

## 🖼️ Architecture Diagram

---
## 🛠 Setup Instructions

### ✅ Part 1: Deploy Frontend on AWS S3

1. Create an **S3 bucket**
2. Enable **static website hosting**
3. Upload your HTML
4. Make bucket public via **Bucket Policy**
5. Note the **S3 website endpoint**

### ✅ Part 2: Deploy API on Azure

1. Create an **Azure Function App**
2. Use a simple HTTP trigger to return:
   ```python
   return func.HttpResponse("Hello from Azure!", status_code=200)

