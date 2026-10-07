# Testing & UAT Portfolio

## Overview

During my experience as a Business Analyst at Rakuten Trade, I was involved in User Acceptance Testing (UAT), functional testing, data validation, and application validation across several system initiatives.

My testing responsibilities focused on validating system behaviour against business rules, production behaviour, and expected results. I also identified inconsistencies and issues during testing and reported them for further investigation.

This portfolio presents three selected testing experiences:

1. **MFA Binding & Login Testing**
2. **ICE Market Data Migration Validation**
3. **iOS SDK Application Testing**

---

# 1. MFA Binding & Login Testing

## Project Overview

The Multi-Factor Authentication (MFA) initiative was designed to enhance account and data protection by controlling which devices and browser sessions could access a user's account.

The key concept tested was that an account could have **one bound mobile device and one active browser session**, with specific rules governing new device and browser login attempts.

My role focused on validating the functional behaviour of the MFA binding, login approval, and session management scenarios.

## Testing Scope

I tested different login and device-binding scenarios to ensure that the system behaved according to the defined business rules.

### Scenario 1 — First-Time Login / Device Binding

When a user logs in for the first time or the system detects that the device has not been bound:

* **Mobile login:** The mobile device is directly bound during the login process.
* **Browser login:** The user is required to use the provided QR code to download/access the mobile application and complete the device-binding process.

### Scenario 2 — Login from an Unbound Mobile Device

After a device has already been bound:

1. A new/unbound mobile device attempts to log in.
2. A login approval notification is sent to the originally bound mobile device.
3. If the bound device approves the request, the new device is successfully logged in.
4. The previously bound mobile device is automatically logged out.

### Scenario 3 — Browser Login

I also validated browser login behaviour:

1. The browser login request is sent to the bound mobile device for approval.
2. After approval, the browser can access the account.
3. The account is restricted to one active browser session/tab according to the defined MFA rules.
4. If another session replaces the existing session, the previous session is automatically logged out.

### Scenario 4 — Multiple Browsers

I validated that different browsers could be used simultaneously according to the defined rules.

For example:

* Google Chrome
* Microsoft Edge

This was tested to ensure that the system differentiated between permitted browser sessions and duplicate sessions within the same browser environment.

### Scenario 5 — MFA Exclusion

Users who do not require MFA can request an exclusion through Customer Service.

I validated that accounts with the appropriate MFA exclusion would bypass the relevant MFA detection and login flow.

## Sample Test Scenarios

The following examples represent the types of scenarios validated during testing. Sensitive production data and internal system information have been excluded.

| Test Scenario | Expected Result |
|---|---|
| First-time login from an unbound mobile device | Mobile device is successfully bound |
| Browser login from an unbound session | User is guided through the required binding process |
| Login from a new mobile device | Approval notification is sent to the bound device |
| Bound device approves new device login | New device is logged in and previous device is logged out |
| Browser login with an existing bound device | Login request is sent to the bound device for approval |
| Multiple sessions within the same browser | Previous session is logged out according to the defined rules |
| Login using different browsers | Chrome and Microsoft Edge can be used according to the defined session rules |
| Account with MFA exclusion | MFA validation is bypassed |

## Testing Approach

The testing focused on:

* Device binding and unbinding behaviour
* Login approval notifications
* Bound vs. unbound device behaviour
* Browser login behaviour
* Session management
* Automatic logout behaviour
* MFA exclusion behaviour
* Positive and negative test scenarios

---

# 2. ICE Market Data Migration Validation

## Project Overview

The ICE migration initiative involved validating market data provided by the ICE data provider against the production environment.

The primary objective of my testing was to ensure that the migrated market data remained **consistent, accurate, and timely** compared with the existing production data.

## Testing Scope

The validation covered market data across different stocks and markets.

Testing had to take into consideration the respective market opening times, as market data availability and updates could vary depending on the trading market.

I performed detailed checks to identify:

* Data inconsistencies
* Missing data
* Incorrect data
* Delayed data updates
* Differences between ICE-provided data and production data

## Market Timing Validation

Because different markets have different opening times, testing had to be performed according to the relevant market schedules.

The validation process involved checking whether market data became available and updated at the expected time.

## Sample Data Validation Scenarios

The following examples represent the validation approach used during testing. Actual market data and production information have been excluded.

| Validation Area | Expected Result |
|---|---|
| Market data availability | Data is available according to the expected market opening time |
| Market data value | ICE data matches the corresponding production data |
| Data update timing | Updates are reflected without unexpected delay |
| Data consistency | No unexpected differences between ICE and production data |
| Delayed update | Any unexpected delay is identified and reported for further investigation |

For example:

**Expected Market Data**

`Market Opens → Data Available → Data Updates`

**Validation**

`ICE Data → Compare with Production → Check Accuracy & Timing`

Any unexpected delay or discrepancy identified during testing had to be reported for further investigation.

## Testing Challenges

This testing required a high level of attention to detail because market data was continuously updated.

A single discrepancy or delayed update could affect the validation result, which meant that the data had to be checked carefully against the production environment.

The testing process was therefore highly time-sensitive and required repeated validation during market operating hours.

---

# 3. iOS SDK Application Testing

## Project Overview

I participated in testing an iOS SDK implementation to ensure that the application continued to behave consistently with the existing production application.

My responsibility focused on validating the application's functionality, UI behaviour, calculations, and order workflow.

## Testing Scope

The testing covered several key areas:

### Functional Validation

Verified that key application functions continued to work as expected after the SDK implementation.

### UI Validation

Compared the iOS application behaviour and visual presentation against the existing production application.

Areas checked included:

* UI behaviour
* Screen presentation
* Colours
* Display consistency

### Calculation Validation

Validated that relevant calculations produced the expected results and remained consistent with the existing application behaviour.

### Order Workflow Validation

Validated the order process to ensure that the workflow remained consistent with the existing production system.

This included checking that users could proceed through the expected order flow without unexpected behaviour.

## Sample Test Scenarios

The following examples represent the types of application behaviour validated during testing.

| Test Area | Expected Result |
|---|---|
| Application functionality | Functions behave consistently with the production application |
| UI presentation | UI behaviour, colours, and display remain consistent |
| Calculation | Calculation results match the expected production behaviour |
| Order workflow | Order process follows the existing production workflow |
| Screen behaviour | User interactions behave as expected |

## Testing Approach

The testing primarily involved comparing the new iOS implementation against the existing production application.

The key validation areas were:

**UI → Functionality → Calculation → Order Workflow → Production Consistency**

Any unexpected behaviour or inconsistency identified during testing was documented and reported for further investigation.

---

# Overall Testing Experience

Across these initiatives, my testing experience involved more than simply executing test cases.

I needed to understand the expected business behaviour, identify relevant scenarios, compare actual system behaviour against expected results, and identify inconsistencies when they occurred.

### Testing Areas

| Area | Experience |
|---|---|
| Functional Testing | MFA, iOS SDK, iSpeed 2.0 |
| UAT | MFA, iOS SDK |
| Data Validation | ICE Migration, iSpeed 2.0 |
| Production Comparison | ICE Migration, iOS SDK, iSpeed 2.0 |
| Business Rule Validation | MFA, iSpeed 2.0 |
| UI Validation | iOS SDK, iSpeed 2.0 |
| Workflow Validation | MFA, iOS SDK, iSpeed 2.0 |
| Calculation Validation | iOS SDK |
| Issue Identification | All testing activities |
| Consistency Checking | ICE Migration, iOS SDK, iSpeed 2.0 |

### Additional Testing Experience

In addition to the testing activities described above, I also participated in functionality and UI validation for the **iSpeed 2.0 Enhancement** project.

My testing involvement included:

- Validating enhanced order-related functionality
- Checking UI behaviour and screen consistency
- Verifying market data displayed within the application
- Comparing expected behaviour against the existing production application
- Identifying and reporting inconsistencies for further investigation

The detailed Business Analysis case study for this project is documented separately in the [iSpeed 2.0 Enhancement](../iSpeed%202.0%20Enhancement/README.md) case study.

## Key Takeaways

These experiences strengthened my ability to:

* Translate business rules into practical test scenarios
* Validate application functionality against expected behaviour
* Identify inconsistencies between environments
* Perform detailed data validation
* Validate UI and workflow behaviour
* Analyse unexpected system behaviour
* Communicate issues for further investigation

## Key Skills Demonstrated

- UAT & Functional Testing
- Business Rule Validation
- Test Scenario Design
- Data Validation & Migration Testing
- UI & Application Validation
- Workflow & Calculation Validation
- Production Comparison
- Defect / Issue Identification
- Requirement-based Testing
- Application Behaviour Analysis

Through these testing activities, I developed practical experience in **UAT, functional testing, data validation, application validation, and business rule analysis** as part of my Business Analyst role.
