# NetlifyHelper Bot Integration Guide

This guide explains how to connect the **NetlifyHelper Bot** with your Netlify account for automated notifications.

---

## **Steps to Integrate NetlifyHelper Bot**

### **1. Generate Webhook Token**
1. Go to **Integrations → Webhook Token**.
2. Click **"Generate New Token"**.
3. Copy the generated token.
![Screenshot 2024-11-29 191311](https://github.com/user-attachments/assets/f5a22305-b58f-46f3-8b30-a5e09e1918de)

---

### **2. Obtain the Token URL**
1. Click the generated token.
2. Click **get Webhook URL**.
3. Set the **Module** as **Bot** and **Bot** as **Netlify_Helper**.
4. The **Incoming endpoint** will be your **TokenURL**.
![ntfly1](https://github.com/user-attachments/assets/ae7eb035-34e9-42b2-bcd9-e8f92dc18e7c)

![ntfly2](https://github.com/user-attachments/assets/e19b97af-f1ac-49f0-bae7-e1c0f67037a0)

---

### **3. Configure Notifications in Netlify**
1. Go to [Netlify Notification Settings](https://app.netlify.com/sites/{your_site}/configuration/notifications#emails-and-webhooks).
2. Under **Deploy Notification**, choose **Add Notification**.
3. In the **Add Notification** window:
- Select **HTTP POST Request**.
- Add the **TokenURL** in the field **Url to notify**.
4. Choose the notification type you need and click **Save**.
![Screenshot 2024-11-29 191610](https://github.com/user-attachments/assets/678f4363-9f63-4400-9ef6-bcbc216f0246)

![Screenshot 2024-11-29 191650](https://github.com/user-attachments/assets/9d66a501-4587-45bf-ab67-34774b077587)
