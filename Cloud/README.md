## Introduction into Cloud 

## Important Links

[Virtual Machine](VM'S.md)

[Virtual Networks](VNET.md)

[Cloud Questions ](Questions.md)

# Cloud

Cloud computing means accessing IT resources (like servers, storage, databases, and software) over the internet instead of managing them yourself.

---

### **1. Resources in the Cloud**

- **Compute Power**: Virtual Machines (VMs) act like computers in the cloud. You can install operating systems and run applications on them.
- **Storage**: You can store data in the cloud instead of using physical hard drives. Types include:
    - **Object Storage**: For storing files like images, videos, or backups (e.g., Amazon S3).
    - **Block Storage**: For disks attached to VMs (like SSDs or HDDs).
    - **File Storage**: For shared storage, like a network drive.
- **Databases (DBs)**: Cloud databases handle your structured data (SQL databases like MySQL, PostgreSQL) or unstructured data (NoSQL databases like MongoDB).
- **Networking**:
    - **Virtual Networks (VNETs)**: Private networks in the cloud where VMs and other resources communicate securely.
    - **Load Balancers**: Distribute traffic evenly across multiple VMs or services.
    - **Firewalls and Security Groups**: Control who can access resources.

---

### **2. Capacity and Scalability**

One of the best features of the cloud is that you can increase or decrease your resources as needed:

- **Scaling Up**: Adding more power to an individual resource (e.g., upgrading a VM).
- **Scaling Out**: Adding more instances of a resource (e.g., creating more VMs).

You pay only for what you use, so you don’t need to invest in expensive hardware upfront.

---

### **3. Virtualization**

Cloud computing uses **virtualization** to divide physical hardware into smaller, independent units called **virtual machines (VMs)**. Each VM behaves like a standalone computer but runs on shared physical hardware.

---

### **4. Cloud Service Models**

There are three main types of services:

1. **Infrastructure as a Service (IaaS)**: Access raw computing resources like VMs, storage, and networking (e.g., AWS EC2, Azure VMs).
2. **Platform as a Service (PaaS)**: Provides tools to build and deploy applications without worrying about the underlying infrastructure (e.g., Google App Engine).
3. **Software as a Service (SaaS)**: Fully functional software delivered via the internet (e.g., Gmail, Dropbox).

---

### **5. Benefits of the Cloud**

- **Flexibility**: Access resources anywhere with the internet.
- **Cost Efficiency**: No need to buy or maintain physical hardware.
- **High Availability**: Resources are often distributed across data centers for reliability.
- **Security**: Major cloud providers implement strict security measures.

---

### **Example in Action**

Imagine you're building an app:

1. Use **VMs** in the cloud to host the app.
2. Store user files in **cloud storage**.
3. Save user data in a **cloud database**.
4. Secure everything using **VNETs** and **firewalls**.
5. Scale your resources up or down depending on how many users you have.

Cloud computing simplifies complex tasks, making it easier for individuals and businesses to focus on what they do best.