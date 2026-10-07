# Foreign Trading Order Enhancement

**Role:** Business Analyst
**Industry:** FinTech
**Project Type:** Trading Application Enhancement
**Markets:** Hong Kong (HK) & United States (US)

---

## Project Overview

The **Foreign Trading Order Enhancement** project focused on expanding the available order types for the Hong Kong and United States markets within the trading application.

Before the enhancement, the available order types differed across markets:

| Market                 | Existing Order Types                   |
| ---------------------- | -------------------------------------- |
| **Malaysia (MY)**      | Market, Limit, Stop Market, Stop Limit |
| **Hong Kong (HK)**     | Limit                                  |
| **United States (US)** | Limit, RSP                             |

To provide a more consistent trading experience across markets, additional order types were introduced for the HK and US markets.

The enhancement reused the **existing order calculation logic and order placement workflow** already implemented in the system. Therefore, the main focus of my BA work was to ensure that the new order types were presented correctly in the UI while maintaining consistency with the existing system behaviour.

---

# Business Objective

The main objective was to expand the supported order types for foreign markets while maintaining the existing system logic and calculation methods.

The enhancement introduced:

* **Market Order**
* **Stop Market Order**
* **Stop Limit Order**

for the relevant HK and US trading scenarios.

Rather than creating new calculation or order-processing logic, the existing system behaviour was reused to support the additional order types.

This helped maintain consistency with the existing trading functionality and reduced unnecessary changes to the underlying workflow.

---

# My BA Contribution

My main responsibilities focused on **requirements documentation and UI/functional alignment**.

### 1. Requirements Analysis

I reviewed the existing order types and their corresponding system behaviour to understand how the new order types could be incorporated into the HK and US markets.

Since the calculation methods and order placement workflow already existed in the system, the requirement was primarily focused on extending the availability of these existing capabilities to the relevant foreign markets.

---

### 2. UI / UX Requirement

I worked closely with the UI/UX designer to determine how the additional order types should be presented within the existing Order Pad.

My focus was to ensure that:

* The new order types were displayed correctly
* The UI remained consistent with the existing Order Pad
* The new options followed the established user flow
* The presentation did not introduce unnecessary changes to the existing trading experience

I communicated the functional requirements and clarified how the existing system behaviour should be reflected in the new UI.

---

### 3. BRD Documentation

I documented the requirements and expected behaviour in the **Business Requirements Document (BRD)**.

The documentation covered areas such as:

* Supported order types by market
* UI requirements
* Existing calculation behaviour
* Existing order placement workflow
* Expected system behaviour
* Functional considerations for the enhancement

The key consideration was to ensure that the new order types followed the **same calculation and order-processing logic already established within the system**.

---

# Existing Logic Reuse

One of the key characteristics of this enhancement was that the underlying trading logic did not require major changes.

The existing system already supported the required calculation methods and order placement workflows for other markets.

Therefore, the enhancement followed this approach:

```text
Existing Order Type Logic
        ↓
Review Existing Calculation & Workflow
        ↓
Extend Availability to HK / US
        ↓
Define UI Presentation
        ↓
Document Requirements in BRD
        ↓
Development
        ↓
Validation / UAT
```

This allowed the enhancement to introduce additional trading capabilities while maintaining consistency with the existing system behaviour.

---

# BA Skills Demonstrated

### Business Analysis

* Requirements Analysis
* Functional Requirement Definition
* Existing System Analysis
* Requirements Documentation
* BRD Preparation
* Cross-Market Requirement Analysis
* Stakeholder Communication

### Application Analysis

* Trading Application Analysis
* Order Type Analysis
* UI / UX Requirement
* Functional Validation
* Existing Workflow Analysis

---

# Project Outcome

The enhancement expanded the available order types for the HK and US markets while maintaining the existing calculation methods and order placement workflows.

By reusing established system logic, the enhancement focused on extending existing capabilities rather than introducing new trading logic.

My contribution primarily covered **requirements analysis, UI/UX coordination, functional clarification, and BRD documentation**.

---

# Confidentiality

This portfolio case study has been generalized and anonymized for portfolio purposes.

It does not include:

* Internal company documents
* Actual BRD files
* Customer information
* Proprietary trading data
* Internal system screenshots
* Production data
* Confidential business rules
