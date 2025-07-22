
# 🐞 Bug Report: Talent Accesses Recruiter Referral Dashboard

## 📌 Title
Talent user is redirected to Recruiter Referral Dashboard when clicking the “Referrals” tab

## 🧪 Bug ID
`BDX-BUG-001`

## 🧭 Environment
 **Platform**: Web Application (Chrome Browser and Microsoft Edge)  
 **URL**: https://bondex.app  
 **User Role**: Talent  
 **Browser**: Chrome v125.0.6422.113 (also confirmed on Firefox)  
 **OS**: Windows 10 / Android 12  
 **Device**: Laptop 

## 📅 Date Detected
23rd July 2025

## 🧵 Precondition
User is registered and logged in as a **Talent** user.

## ✅ Steps to Reproduce
1. Log in as a **Talent** user at [https://bondex.app](https://bondex.app).  
2. Navigate to the sidebar or navbar.  
3. Click on the **“Referrals”** tab/icon.  
4. Observe the redirection.

## ❌ Actual Result
Talent is redirected to `/recruiter/referrals`, which is the **Recruiter's referral dashboard**. The content includes referral links, referral earnings, and other recruiter-specific features not meant for Talent users.

## ✅ Expected Result
Talent should either:
- Be redirected to their own version of the **Referrals** page (if designed to exist),  
**OR**  
- See a **“Not Authorized”** or **404** page, indicating this route is restricted.

## ⚠️ Impact Level
**Critical**

## 🔐 Security Concern
This violates **role-based access control (RBAC)**, enabling unauthorized access to recruiter-exclusive features and possibly sensitive data (e.g. earnings, referrals).

## 🎯 Priority
**P1 - Immediate Fix Needed**

## 📸 Video Proof
[Watch the video proof](https://drive.google.com/file/d/1IfXnC1hpTIqnKJGZJe0_8iaDbnNyPakh/view?usp=sharing)

## 🧰 Suggested Fix
- Check the logic controlling access to the `/referrals` route.
- Add role checks:
  ```js
  if (user.role !== "recruiter") {
    return <Redirect to="/unauthorized" />;
  }
  ```
- Hide the “Referrals” tab from the Talent user interface altogether.
- Implement backend route protection as well, in case of manual URL entry.

## 📞 Reported By
Enaibre Emmanuel (QA Intern )
