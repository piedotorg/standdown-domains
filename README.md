
# Affiliate Network Rules

This repository contains a **JSON file** that defines rules for handling **affiliate network tracking links**. It includes patterns to identify various affiliate networks and specifies how they should be processed. We publish these rules to promote **transparency** in how we handle Stand-down, rather than pushing for a universal standard that everyone must adopt.

---

## **afsrc=1: The Preferred Industry Standard**

For over a decade, `afsrc=1` has served as a well-recognized standard in affiliate marketing. It offers a simple, universal way to signal the source of affiliate traffic, thereby ensuring accurate tracking and attribution. Ideally, **all advertisers and publishers** would consistently include `afsrc=1` in their affiliate links. Doing so eliminates the need for maintaining large, ever-changing lists of affiliate network rules.

- **Responsibility:** Publishers and advertisers should add `afsrc=1` to their links to clearly indicate affiliate sources.
- **Benefits:** When used universally, `afsrc=1` streamlines tracking, reduces confusion, and makes it easier for all parties to follow Stand-down policies.

However, because not all publishers follow this best practice, we continue to maintain and share our Stand-down rules for transparency.

---

## **What is Stand-down?**

Affiliate networks have long implemented policies—often referred to as **"standing down"**—to manage the complexities of last-click attribution and commission credit allocation. Over time, different networks have developed varied, often convoluted methods to address these challenges. In our approach, we’ve taken the most conservative stance possible to ensure a consistent experience across the board.

While the Stand-down policy itself is not new, its implementation can be inconsistent. That’s why we are pushing for **afsrc=1** as the industry standard for affiliate tracking. With afsrc=1, all parties benefit from a clear and streamlined system that simplifies attribution and reduces the need for maintaining complex Stand-down rules.

### **Why does it matter?**
When a shopper is already affiliated with a cash back provider, creator, or publisher, it's important that other extensions or publishers do not market additional offers. This universal Stand-down approach ensures that attribution works as expected for all parties, providing a consistent and transparent experience for both users and affiliate partners.

### **Example Scenario**
A user has two cash back browser extensions installed. If they activate cash back in the first extension, the second extension **must not**:  
- Show a pop-up or notification asking them to activate cash back  
- Display banners or other marketing to encourage activation  
- Attempt to overwrite the original affiliate tracking  

By **following Stand-down rules**, we ensure that **cash back tracking remains fair and transparent** for shoppers, affiliates, and publishers.

### **What does "marketing to" mean?**
- Displaying a **pop-up** to activate cash back  
- Showing **banners** or notifications promoting activation  
- Attempting to **overwrite the original cash back tracking**  

---

## **Why We Publish Our Stand-down Rules**

We believe that, ideally, **`afsrc=1`** should be universally adopted so that no Stand-down list is necessary. However, because not all affiliate networks or publishers implement it consistently, we maintain this **JSON file** to provide clarity on how we handle Stand-down events. This allows anyone—publishers, advertisers, or other developers—to see exactly how we process affiliate links in the absence of `afsrc=1`.

While we encourage the community to contribute to this file and use it as a resource, we see **`afsrc=1`** as the true, easy-to-use standard that already exists. Our hope is that more networks will **educate and enforce** its usage.

For more details on how we can streamline attribution, please check out our blog post [Embracing afsrc=1: A New Approach to Affiliate Tracking](https://www.pie.org/blog/embracing-afsrc-1). In the post, we focus on the need for stronger **`afsrc=1`** enforcement and explore ideas like first-click attribution. Our hope is that more networks will adopt and enforce **`afsrc=1`**, leading to a more consistent and transparent affiliate ecosystem.

---

## **Stand-down Types & Implementation Responsibility**

Stand-down enforcement can vary based on the level of restriction required by the affiliate network. There are two primary enforcement levels:

### **1️⃣ Notag**
- **Meaning:** The extension **cannot apply an affiliate tag** but may still display some functionality (e.g., coupons).  
- **Allowed:**  
  - Displaying coupons  
  - Showing non-affiliate-related functionality  
- **Not Allowed:**  
  - Overwriting an existing affiliate tag  

### **2️⃣ Stop**
- **Meaning:** The extension **must not show any functionality** related to cash back or rewards.  
- **Not Allowed:**  
  - Displaying cash back pop-ups or banners  
  - Allowing manual cash back activation  
  - Showing coupons or rewards  

### **🚨 Responsibility of Implementation**
Using this Stand-down file **does not automatically enforce compliance**.  
- **Implementers** (browser extensions, shopping tools, publishers, etc.) must ensure that their product **respects the appropriate Stand-down level**.  
- Failure to respect Stand-down rules may result in **violations of affiliate network agreements**.

---

## **Contribution Guidelines**

To maintain quality and accuracy, all contributions must follow these guidelines:

1. **Only submit verified affiliate network rules**  
   - All added rules must correspond to legitimate, known affiliate networks.
2. **No ad networks**  
   - This repository is strictly for **affiliate network tracking rules**, not general ad network behavior.

---

## 🚀 **How to Contribute**

We welcome contributions! If you’d like to propose changes or add new affiliate network rules, follow these steps:

1. **Fork** this repository.
2. Clone your fork: git clone https://github.com/your-username/repository-name.git
   cd repository-name
3. Open and edit Stand-down.json, ensuring valid JSON formatting.
4. Commit your changes: git commit -am "Added new affiliate rule for XYZ network"
5. Push your changes to your fork: git push origin your-branch-name
6. Submit a Pull Request (PR) to this repository with a clear description of your changes.

MIT License

Copyright (c) 2025 The People's Internet Experiment Inc.

Permission is hereby granted, free of charge, to any person obtaining a copy  
of this software and associated documentation files (the "Software"), to deal  
in the Software without restriction, including without limitation the rights  
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell  
copies of the Software, and to permit persons to whom the Software is  
furnished to do so, subject to the following conditions:  

The above copyright notice and this permission notice shall be included in all  
copies or substantial portions of the Software.  

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR  
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,  
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE  
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER  
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,  
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE  
SOFTWARE.
