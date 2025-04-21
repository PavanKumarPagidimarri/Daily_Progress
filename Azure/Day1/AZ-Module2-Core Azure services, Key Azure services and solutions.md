# Define cloud models

What are cloud models? The cloud models define the deployment type of cloud resources. The three main cloud models are: private, public, and hybrid.

### **Private Cloud**

- Delivers IT services over the internet but **used exclusively by a single organization**.
- Offers **greater control and customization** for the company and its IT team.
- Generally **more expensive** and has **fewer benefits** (like scalability) compared to public cloud.
    
- Can be:
    - Hosted **on-premises** in the organization's own data center.
    - Hosted **offsite in a dedicated data center**, possibly by a third party, but still exclusive to the organization.
        

---

### ☁️ **Public Cloud**

- **Built, owned, and managed by third-party** cloud service providers (e.g., AWS, Azure, GCP).
- **Open to the general public** – anyone can access and use services.
- Resources like storage and compute are **shared across multiple users**.
- Offers benefits like **cost-efficiency, scalability**, and **minimal maintenance responsibility**.
    

---

### ☁️ **Hybrid Cloud**

- A **combination of private and public cloud** environments working together.
- Allows **data and apps to move between** private and public clouds for **flexibility and optimization**.
- Can be used for:
    
    - **Handling spikes in demand** by using public cloud for overflow.
    - **Improving security** by keeping sensitive workloads in private cloud and others in public.
    - **Custom deployments** based on business requirements.


### Cloud service types:
### 💻 **1. Infrastructure as a Service (IaaS)**

> _“Virtualized computing resources delivered over the internet”_

- Provides **virtual machines**, storage, networks, and operating systems.
- Most control over the IT resources, like hardware and software.
- Great for **system admins, network architects**, and custom deployment.
- You manage: OS, applications, middleware, data.
- Cloud provider manages: virtualization, servers, storage, networking.

**Examples**: Microsoft Azure (VMs), Amazon EC2, Google Compute Engine

---

### 🧩 **2. Platform as a Service (PaaS)**

> _“Framework for developers to build applications without managing infrastructure”_

- Provides tools to develop, test, and deploy applications.
- No need to manage OS, storage, or infrastructure.
- Useful for **developers** to focus only on the application logic.
- Cloud provider manages everything except the application and data.
    

**Examples**: Azure App Services, Google App Engine, Heroku

---

### 🧑‍💼 **3. Software as a Service (SaaS)**

> _“Ready-to-use software delivered over the internet”_

- Fully managed applications delivered via the web.
- Users don’t worry about infrastructure, platform, or code.
- Accessible via browser – great for **end-users** and businesses.
- Cloud provider handles **everything** (app, data, runtime, OS, servers, etc.)
    
**Examples**: Microsoft 365, Gmail, Dropbox, Salesforce

### 🔐 **What is the Shared Responsibility Model?**

It defines **who is responsible** for securing what — based on the type of service you're using:

- **IaaS (Infrastructure as a Service)**
- **PaaS (Platform as a Service)**
- **SaaS (Software as a Service)**
    
### 📊 **Responsibility Breakdown:**

#### ✅ **Microsoft’s Responsibility (Cloud Provider):**

- **Physical data centers** (security, power, cooling, hardware)
- **Network infrastructure**
- **Host OS and virtualization layer**
- **Platform security** (in PaaS & SaaS)
- **Compliance with global standards**

#### ✅ **Your Responsibility (Customer):**

- **Data** (classification, encryption, backups)
- **Identity and access** (users, permissions, MFA)
- **Applications** (security, code, APIs)
- **Operating systems & updates** (in IaaS)
- **Network configuration** (NSGs, firewalls)


-----------------------------------
Cloud Model |    Microsoft Manages |    You Manage

IaaS | Hardware, networking, virtualization |  OS, apps, data, access, configs

PaaS | Infrastructure + OS, runtime |  App logic, data, access

SaaS | Everything (infra, app, runtime) |  Data, access, user management

