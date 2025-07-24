
# Recruiter User - Manual Test Cases

## Test Case 1: Recruiter Navigation After Signup
- **Test Case ID:** TC-R-001  
- **Title:** Verify recruiter is redirected to the referrals page after signup  
- **Steps:**  
  1. Sign up as a recruiter user  
  2. Click “Continue”  
- **Expected Result:**  
  Recruiter is redirected to `https://bondex.app/recruiter/referrals`  
- **Actual Result:**  
  Redirect is successful  
- **Status:** ✅ Pass  

## Test Case 2: Recruiter Navigation Items
- **Test Case ID:** TC-R-002  
- **Title:** Verify presence and function of navbar items for recruiter  
- **Steps:**  
  1. Login as recruiter user  
  2. Inspect navbar  
  3. Click on each of the 7 items: Jobs Portal, Applications, Referrals, Profile, Notifications, Account Settings, Logout  
- **Expected Result:**  
  All items present and redirect appropriately  
- **Actual Result:**  
  All items available and functional  
- **Status:** ✅ Pass  

## Test Case 3: Post a Job Button Visibility
- **Test Case ID:** TC-R-003  
- **Title:** Ensure recruiter has no “Post a Job” button visible  
- **Steps:**  
  1. Navigate to any page as recruiter  
  2. Look for “Post a Job” button  
- **Expected Result:**  
  Button should not exist for recruiter  
- **Actual Result:**  
  No button found  
- **Status:** ✅ Pass  

## Test Case 4: Recruiter Account Settings - Wallet Tab
- **Test Case ID:** TC-R-004  
- **Title:** Check external wallet connection feature  
- **Steps:**  
  1. Go to `Account Settings > Wallet`  
- **Expected Result:**  
  “Connect External Wallet” button should be present  
- **Actual Result:**  
  Button is present  
- **Status:** ✅ Pass  

## Test Case 5: Recruiter Account Settings - Job Alerts
- **Test Case ID:** TC-R-005  
- **Title:** Validate recruiter can view and configure job alerts  
- **Steps:**  
  1. Go to `Account Settings > Job Alerts`  
- **Expected Result:**  
  Job alert configuration page appears  
- **Actual Result:**  
  Working as expected  
- **Status:** ✅ Pass  
