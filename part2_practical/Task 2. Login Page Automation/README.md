# Login Page Automation with Testim.io

## Project Overview
Automated testing of [the-internet herokuapp login page](https://the-internet.herokuapp.com/login) using Testim.io's free tier.

## Full Report
[View the complete step-by-step details Here.](Login_test-allScreenShots-06-23-2025T08-32-56_A2.pdf)
[Go to Execution Result](https://app.testim.io//#/project/usw2KeHRsnnC6jn4ZzIMymWF/branch/master/test/OkFlJXE5MPVsXOvn?result-id=GAC0zaxmklTivHCn)

## Implementation Steps

### 1. Test Setup
- **Recorded test flow**:
  1. Navigated to login page
  2. Entered valid credentials:
     - Username: `tomsmith`
     - Password: `SuperSecretPassword!`
  3. Clicked Login button
  4. Verified Secure Area
  5. Logged out

- **Added assertions**:
  - Presence of "Secure Area" text (success case)
  - Visibility of Logout button
  - Error message for invalid attempts

### 2. Test Execution
- **Configuration**:
  - Browser: Chrome
  - Viewport: 1024x768 (manually set)
  - Run mode: Standard (non-headless)

- **Results obtained**:
  - 6/8 steps passed successfully
  - Full execution time: 42 seconds
  - [View detailed report](Login_test-allScreenShots-06-23-2025T08-32-56_A2.pdf)

### 3. Files Generated
/login_automation/
├── Login_Test.json # Testim export
├── Testim_Report_20240623.html # Execution summary
└── screenshots/
├── successful_login.png # Secure Area
└── logout_screen.png # Post-logout state

## How to Re-run
1. **Import test**:
   - Upload `Login_Test.json` to Testim dashboard
2. **Execute**:
   - Select test → Click "Run"
3. **View results**:
   - Screenshots auto-captured in `/screenshots`
   - HTML report generated post-execution

## Key Observations
- Testim successfully automated:
  - Form filling
  - Success/failure validations
  - Page transitions
- Free tier limitations encountered:
  - No CSV parameterization
  - Limited retry mechanisms

> Note: This implementation used workarounds for free tier constraints.