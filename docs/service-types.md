
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
<!-- DYNAMIC CONTENT - DO NOT EDIT: END -->

> **Note:**  
Legacy service types above are still used by some retailers. 

The time slots of these legacy service types vary and align to certain combinations of the standard list, depending on the geographical location they are based on (e.g. **DDD** is equivalent to **P** delivery type and its time slots may coincide to the ones defined in **NFA** in some countries).


















