# ***Virtual Private Cloud (VPC)***

**Author:** Jadon Scott  
**Date:** 07/01/26 

---

# **Project Overview**

### **Project Summary**

In this project, you’re going to build a VPC with the purpose of being able to showcase a secure, isolated, and scalable environment you’ll build from scratch.

---

**Initial Questioning**

* What is the project called? \- Virtual Cloud Cloud.  
* Why did you choose this project? \- To learn & practice an aspect of networking that’s viable in the IT / Cybersecurity Industry.

---

# **Requirements**

### **Business Requirements**

* What did the user or client need? \- Google Gemini API Key, Cursor, and Python.  
* What constraints existed? \- No constraints existed.

### **Technical Requirements**

* Operating system \- Windows 11  
* Network requirements \- Stable Connection  
* Software dependencies \- Amazon Web Services (AWS)

---

# **Project Scope**

**Questions to Answer**

* What assumptions were made? \- That the project mostly be configurations rather than coding.  
* What limitations existed? \- No limitations existed. 

---

# **Pre \- Download Requirements & Configurations**

- Create an account with [AWS](https://signin.aws.amazon.com/signin?redirect_uri=https%3A%2F%2Fconsole.aws.amazon.com%2Fconsole%2Fhome%3FhashArgs%3D%2523%26isauthcode%3Dtrue%26state%3DhashArgsFromTB_ap-southeast-2_fffdf5be4bb1a27e&client_id=arn%3Aaws%3Asignin%3A%3A%3Aconsole%2Fcanvas&forceMobileApp=0&code_challenge=m-aiqeB2UZeXTGXNyugMP8L64zd_AGUxJl4HLnA-X1o&code_challenge_method=SHA-256)

---

# 

# Phase \#1 \- Creating the VPC

* In the **AWS Management Console** search field, type VPC.  
* Select from the drop down menu.

* In the left navigation pane, choose **Your VPCs**.  
* {Note \- Make sure you're in the region that's closest to you. Use the dropdown on the top right hand corner to switch Regions.}

![][image1]

<img width="941" height="734" alt="InstructionFlick#1" src="https://github.com/user-attachments/assets/a377d2e4-d99f-425a-99f1-65625a16b81d" />
   \#1

* You'll notice that there is already a VPC in your account; that VPC is the default & serves as a form of example. It can be ignored.

* Choose **Create VPC**.  
* Choose **VPC Only** & input the following below.

**Name tag:** Test VPC

**IPv4 CIDR:** 10.0.0.0/16

![][image2]

<img width="921" height="757" alt="InstructionFlick#2" src="https://github.com/user-attachments/assets/c88a2cc9-63ac-4e66-aba7-da8123458023" />
  \#2

---

# 

# Phase \#2 \- Creating Subnets

The next step is to divide this large space into subdivisions called subnets. This part helps you start planning where different resources will stay and operate.

* In the **VPC Dashboard**, under **Virtual Private Cloud**, choose **Subnets**.  
* Choose **Create subnet**.


![][image3]

<img width="1099" height="773" alt="InstructionFlick#3" src="https://github.com/user-attachments/assets/567dd397-dfcd-4229-a440-4e4fb94c071c" />
  \#3

* Again, you'll notice that there are already Subnets in your account. They come as default along with the default VPC. They are pre-defined for each availability of a region. They can be ignored.

Configure your subnet settings:

* **VPC ID:** Test VPC  
* **Subnet name:** Public 1  
* **Availability Zone:** Pick the first Availability Zone on the list.  
* **IPv4 VPC CIDR block:** 10.0.0.0/16  
* **IPv4 subnet CIDR block:** 10.0.0.0/24

![][image4]

<img width="1092" height="586" alt="InstructionFlick#4" src="https://github.com/user-attachments/assets/4426306d-e123-41e0-9093-83463da9bbcb" />
  \#4

* Choose **Create subnet.**  
* Select the checkbox next to **Public 1**.  
* In the **Actions** menu, select **Edit subnet settings.**

**![][image5]**

<img width="1089" height="756" alt="Instruction Flick#5" src="https://github.com/user-attachments/assets/6e40c0d0-3500-48a2-9f77-120c73286618" />
  \#5

* Check the box next to **Enable auto-assign public IPv4 address.**  
* Choose **Save.**

---

# 

# Phase \#3 \- Creating the Internet Gateway

Now, for the final step, connect your VPC with an internet gateway. Think of it as building a transit system that links your private city to the outside world.

* In the left navigation pane, choose **Internet gateways**.

* Last time, you'll notice that there is already an existing Internet Gateway similar to existing Subnet n’ VPC’s from earlier. It can also be ignored.

![][image6]

<img width="1086" height="877" alt="InstructionFlick#6" src="https://github.com/user-attachments/assets/e0d9699b-053a-483e-bfff-2e2c68a63c64" />
  \#6

* Choose **Create internet gateway**.  
* Configure your internet gateway settings:  
  * **Name tag:** Test IG  
* Choose **Create internet gateway**.

* Select your newly created internet gateway and choose **Actions**, then **Attach to VPC**.
