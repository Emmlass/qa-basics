
# Talent User - Manual Test Cases

## Test Case 1: Talent Navigation After Signup
 **Test Case ID:** TC-T-001  
 **Title:** Verify talent is redirected to the applications page after signup  
 **Steps:**  
  1. Sign up as a talent user  
  2. Click “Continue”  
 **Expected Result:**  
  Talent is redirected to `https://bondex.app/talent/applications`  
 **Actual Result:**  
  Redirect is successful  
 **Status:** ✅ Pass  

## Test Case 2: Talent Navigation Items
 **Test Case ID:** TC-T-002  
 **Title:** Verify presence and function of navbar items for talent  
 **Steps:**  
  1. Login as talent user  
  2. Inspect navbar  
  3. Click on each of the 7 items: Bondex logo, Jobs Portal, Applications, Referrals, Profile, Notifications, Profile Dropdown  
 **Expected Result:**  
  All items present and redirect appropriately  
 **Actual Result:**  
  All items available and functional  
 **Status:** ✅ Pass  

## Test Case 3: Talent Referral Link Behavior
 **Test Case ID:** TC-T-003  
 **Title:** Verify talent referral link redirects to recruiter page  
 **Steps:**  
  1. Click “Referrals” in talent navbar  
  2. Observe the URL and redirection  
 **Expected Result:**  
  Redirects to recruiter referral dashboard  
 **Actual Result:**  
  Talent is redirected to `https://bondex.app/recruiter/referrals`  
 **Status:** ⚠️ Pass (but potential UX concern)  

## Test Case 4: Talent Profile Dropdown Options
 **Test Case ID:** TC-T-004  
 **Title:** Verify talent profile dropdown contains expected menu items  
 **Steps:**  
  1. Click circular profile icon (top-right)  
  2. Check for: Job Alerts, Account Settings, Help Center, Logout  
 **Expected Result:**  
  All items visible and clickable  
 **Actual Result:**  
  Working as expected  
 **Status:** ✅ Pass  

## Test Case 5: Talent Account Settings - Account Details
 **Test Case ID:** TC-T-005  
 **Title:** Verify correct email and account type shown for talent  
 **Steps:**  
  1. Go to `Account Settings > Account Details`  
 **Expected Result:**  
  Shows email and account type as “Talent”  
 **Actual Result:**  
  Working correctly  
 **Status:** ✅ Pass  

## Test Case 6: Talent Account Settings - Wallet
 **Test Case ID:** TC-T-006  
 **Title:** Verify wallet page and connect external wallet button  
 **Steps:**  
  1. Go to `Account Settings > Wallet`  
 **Expected Result:**  
  Page loads with “connect external wallet” button  
 **Actual Result:**  
  As expected  
 **Status:** ✅ Pass  

## Test Case 7: Talent Account Settings - Job Alerts
 **Test Case ID:** TC-T-007  
 **Title:** Verify job alert page for talent  
 **Steps:**  
  1. Go to `Account Settings > Job Alerts`  
 **Expected Result:**  
  Loads `https://bondex.app/talent/account/job-alerts`  
 **Actual Result:**  
  Working correctly  
 **Status:** ✅ Pass  
