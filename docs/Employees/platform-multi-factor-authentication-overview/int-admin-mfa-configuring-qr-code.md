---
title: Configuring multi-factor authentication using an authenticator app
excerpt: >-
  You can choose to set up your multi-factor authentication using a QR code or
  SMS. To learn how to set it up using SMS, see Configuring multi-factor
  authentication using SMS.
hidden: false
metadata:
  description: >-
    You can choose to set up your multi-factor authentication using a QR code or
    SMS. To learn how to set it up using SMS, see Configuring multi-factor
    authentication using SMS.
---

You can choose to set up your multi-factor authentication using a QR code or SMS. To learn how to set it up using SMS, see [Configuring multi-factor authentication using SMS](https://doc.toasttab.com/doc/platformguide/intAdminMfaConfiguringSms.html).

**To use a QR code for multi-factor authentication**

1. From a browser, go to [https://pos.toasttab.com](https://pos.toasttab.com) and select **Login** to access the Toast Web login page.
2. Enter your username and password. Select **Continue**.
3. In the **Keep Your Account Safe** dialog, select **Google Authenticator or similar**.

   ![Example of the Keep Your Account Safe window.](https://doc.toasttab.com/doc/media/mfa_keep_your_account_safe.png)
4. Scan the QR code displayed in the **Secure Your Account** window using an authenticator app.
5. Enter the one-time code provided in the authenticator app in the edit field, then select **Continue**.

   ![Example of the Secure Your Account window.](https://doc.toasttab.com/doc/media/mfa_secure_your_account.png)

In the future, you will be prompted periodically to enter a 6-digit code from your authenticator app when you sign in to Toast Web.

![Example of the Verify Your Identity dialog where you enter the 6-digit-code.](https://doc.toasttab.com/doc/media/mfa_enter_code_screen.png)
