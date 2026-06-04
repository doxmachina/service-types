
# Service Types

This document intends to offer retailers a overview about what service types are, their role in the created and manifested orders and provide the reference list of the standard codes to use during order creation.

## Overview

Service types act as order parameters that define unique characteristics of the services offered by Paack: *time to delivery*, *time slot choice* (either fixed, defined by Paack or chosen by the customer) and its *duration*. 

Each retailer obtains the agreed service type from Commercial department as part of the relevant Service configurations.
Retailers, therefore, must only use the contracted service type when submitting new orders. 

Service types, along with parcels definition, customer and delivery/pick-up information are all integral parts of an order. 

> **Note**:  
During order creation, `service_type` is a mandatory field.  
After creating an order, it is not possible to change it.

The service type configured for the retailer account will be used within Paack ecosystem as part of the order processing, for:

+ Applying a default service type for orders manifested via "CSV upload" via CMS dashboard
+ Applying a default service type for individual orders, created manually via CMS dashboard
+ Applying a default service type for orders manifested via SFTP
+ Validating the service type for orders manifested via API 
    > **Note:**  
    These orders come with `service_type` defined in the body.

## How Service Types Are Constructed

Each service type is defined as a unique three-character code resulting from the combination of three single-character attributes for the following propositions:

1. Delivery date type; also indicates if Warehouse (**WH**) or Store / Ship from Store (**SFS**) model.
2. Time slot type
3. Available slot length

<!-- DYNAMIC CONTENT - DO NOT EDIT: START -->
<!-- Auto generated from .\schema\service-types.json on: 2026-06-03 18:46 -->

## Delivery Type

| Code | Description | 
|------|-------------|
|S| Same day delivery |
|N| Next day delivery |
|P| Precise day delivery |
|C| Two-day delivery |
|W| Any day delivery |
|X| Same day / express delivery |
|R| Return |


## Time Slot Type

| Code | Description | 
|------|-------------|
|T| time slot available |
|F| Fixed time slot |


## Slot Length

| Code | Description | 
|------|-------------|
|2| 2 hours |
|4| 4 hours |
|H| morning or evening slots |
|A| All day |
|Z| Other |


## Warehouse Models

| Code | Description | 
|------|-------------|
|WH| WH |
|SFS| SFS |
|both| WH & SFS |


## Legacy Codes

| Code | Description | 
|------|-------------|
|DDD| Defined day delivery  |
|ST3| Same day delivery - time slot available - 3 hours |
|UNK| Unknown |
|ND| Next day |
|SD| Same day |


## List of Service types

| Code | Description | Model |
|------|-------------|-------|
| ST2 | Same day delivery - time slot available - 2 hours | WH & SFS |
| ST4 | Same day delivery - time slot available - 4 hours | WH & SFS |
| STA | Same day delivery - time slot available - All day | WH & SFS |
| STZ | Same day delivery - time slot available - Other | WH & SFS |
| SF2 | Same day delivery - Fixed time slot - 2 hours | WH & SFS |
| SF4 | Same day delivery - Fixed time slot - 4 hours | WH & SFS |
| SFH | Same day delivery - Fixed time slot - morning or evening slots | WH & SFS |
| SFA | Same day delivery - Fixed time slot - All day | WH & SFS |
| SFZ | Same day delivery - Fixed time slot - Other | WH & SFS |
| NT2 | Next day delivery - time slot available - 2 hours | WH |
| NT4 | Next day delivery - time slot available - 4 hours | WH |
| NTH | Next day delivery - time slot available - morning or evening slots | WH |
| NTZ | Next day delivery - time slot available - Other | WH |
| NF2 | Next day delivery - Fixed time slot - 2 hours | WH |
| NF4 | Next day delivery - Fixed time slot - 4 hours | WH |
| NFA | Next day delivery - Fixed time slot - All day | WH |
| PT2 | Precise day delivery - time slot available - 2 hours | WH |
| PT4 | Precise day delivery - time slot available - 4 hours | WH |
| PTH | Precise day delivery - time slot available - morning or evening slots | WH |
| PTA | Precise day delivery - time slot available - All day | WH |
| PTZ | Precise day delivery - time slot available - Other | WH |
| PF2 | Precise day delivery - Fixed time slot - 2 hours | WH |
| PF4 | Precise day delivery - Fixed time slot - 4 hours | WH |
| PFA | Precise day delivery - Fixed time slot - All day | WH |
| CT2 | Two-day delivery - time slot available - 2 hours | WH |
| CT4 | Two-day delivery - time slot available - 4 hours | WH |
| CTH | Two-day delivery - time slot available - morning or evening slots | WH |
| CTZ | Two-day delivery - time slot available - Other | WH |
| CF2 | Two-day delivery - Fixed time slot - 2 hours | WH |
| CF4 | Two-day delivery - Fixed time slot - 4 hours | WH |
| CFA | Two-day delivery - Fixed time slot - All day | WH |
| CFZ | Two-day delivery - Fixed time slot - Other | WH |
| WT2 | Any day delivery - time slot available - 2 hours | WH |
| WT4 | Any day delivery - time slot available - 4 hours | WH |
| WTH | Any day delivery - time slot available - morning or evening slots | WH |
| WTZ | Any day delivery - time slot available - Other | WH |
| WF2 | Any day delivery - Fixed time slot - 2 hours | WH |
| WF4 | Any day delivery - Fixed time slot - 4 hours | WH |
| WFH | Any day delivery - Fixed time slot - morning or evening slots | WH |
| WFA | Any day delivery - Fixed time slot - All day | WH |
| WFZ | Any day delivery - Fixed time slot - Other | WH |
| XTZ | Same day / express delivery - time slot available - Other | SFS |
| XFA | Same day / express delivery - Fixed time slot - All day | SFS |
| XFZ | Same day / express delivery - Fixed time slot - Other | SFS |
| RT2 | Return - time slot available - 2 hours | WH |
| RFA | Return - Fixed time slot - All day | WH |

<!-- DYNAMIC CONTENT - DO NOT EDIT: END -->

> **Note:**  
Legacy service types above are still used by some retailers. 

The time slots of these legacy service types vary and align to certain combinations of the standard list, depending on the geographical location they are based on (e.g. **DDD** is equivalent to **P** delivery type and its time slots may coincide to the ones defined in **NFA** in some countries).


















