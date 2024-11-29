# NetlifyHelper Bot Integration Guide

This guide explains how to connect the **NetlifyHelper Bot** with your Netlify account for automated notifications.

---

## **Steps to Integrate NetlifyHelper Bot**

### **1. Generate Webhook Token**
1. Go to **Integrations → Webhook Token**.
2. Click **"Generate New Token"**.
3. Copy the generated token.
![image](https://github.com/user-attachments/assets/f2435777-8607-4a0b-ac90-64062a4a61a1)

---

### **2. Configure the Token URL**
1. Replace `{Token}` in the following URL with your copied token:
https://cliq.zoho.com/company/871740404/api/v2/bots/netlifyhelper/incoming?zapikey={Token}


This will be your **TokenURL**.

---

### **3. Configure Notifications in Netlify**
1. Go to [Netlify Notification Settings](https://app.netlify.com/sites/{your_site}/configuration/notifications#emails-and-webhooks).
2. Under **Deploy Notification**, choose **Add Notification**.
3. In the **Add Notification** window:
- Select **HTTP POST Request**.
- Add the **TokenURL** in the field **Url to notify**.
4. Choose the notification type you need and click **Save**.
![image](https://github.com/user-attachments/assets/e0bfd311-7fe2-4480-9a65-5cc6f75c29db)
![image](https://github.com/user-attachments/assets/b98e93fb-c60b-4bde-8a30-5bee2c39cf4a)

---

### **Example:**
Here’s an example URL for your webhook:
https://cliq.zoho.com/company/871740404/api/v2/bots/netlifyhelper/incoming?zapikey=YOUR_GENERATED_TOKEN

---

### **Need Help?**
If you encounter any issues, please reach out to the support team or consult the [Netlify Documentation](https://docs.netlify.com/).
