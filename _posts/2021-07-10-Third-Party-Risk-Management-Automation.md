---
excerpt: "Start Automation Third Party Risk."
author_profile: false
title:  "Third-Party Risk Management Automation"
search: True
categories: 
  - Third-Party
  - Risk Management
  - Automation
  - Risk
---

# Third-Party Risk Management Automation Why❓

## Literature
In 2019, Gartner  conducted a cross-functional third-party risk management survey of 11 functions. These were compliance, enterprise risk management, finance and accounting, IS, IT, internal audit, legal, privacy, purchasing and procurement, supply chain/distribution and logistics, and dedicated third-party risk management functions or offices. They studied the changing nature of third-party profiles and the impact of a broad range of third-party risk management activities, from due diligence to monitoring. Here, they report on aggregate, observed findings on the 11 functions.

State of the Third-Party Network
Third parties continue to expand into an extensive fourth and “*n*th” party network.
According to Gartner, 76% of organizations anticipate an increase in the number of third parties within their network over the next three years. Third parties continue to perform new-in-kind services and services outside the core business model, suggesting they are key to future growth. At the same time, the third-party network continues to expand to include a number of fourth and fifth or “*n*th” parties. Sixty-six percent of organizations anticipate an increase in the number of fourth and fifth parties in their third-party networks over the next three years (see Figure 1).

Figure 1. Forecast Changes for the Third-Party Network

![Figure 1. Forecast Changes for the Third-Party Network.](/assets/images/Figure-1--Forecast-Changes-for-the-Third-Party-Networkcontent.png "Figure 1. Forecast Changes for the Third-Party Network.")

## Conclusion

Yes, Conclusion Gartner research demonstrates thid-party networks continue to expand and what are you doing?

## Here is what I have done before

### Assumptions

1. There is already a contractual relationship between the parties and they have agreed to the exchange of data and to be subject of external audit.

1. You have access to the relevant data from your organization (ERP Invoice Records, Authorized Sales Territories, Promotions Periods, etc.)

1. Additional data may be required to enable other audit features; in the case of sales to Parent or Subsidiaries the auditor will required to research such metadata.

### Audit Overview

First lets understand the Audit Scope; we want to validate that our *Third-Party* is in alligment with your company policies, ethics and that they are following up contractual obligations. 

### Data Gathering

To start working we will need to get some data, such can come from several sources. 

#### Audit Metadata

|Field Name|Field Data Type|
|------------- |:-------------:|
|v_AP_Start_Date|date, datetime|
|v_AP_End_Date|date, datetime|
|Region|text|

#### Sales Data ERP Invoice Records (Local Clients, External Third-Party Vendor and/or Supply Chain Management Solutions)

|Field Reference|Field Name|Field Data Type|
| ------------- |:-------------:|:-------------:|
|R.1| Client (Parent or Subsidiaries)|text|
|R.2| Transaction Type (examples: sale, credite note, return, debit memo)|text,number with table reference.|
|R.3*| **_Invoice Date_**| date, datetime|
|R.4| Invoice Number or Credit Note Number|number, text, unique|
|R.5| For Returns: Original Invoice Number|number, text, unique|
|R.6| For Returns: Reason for Return (return code, etc.)|number, text, unique|
|R.7| Transaction Number if different from Invoice Number|number, text, unique|
|R.8| Sales Order Id|number, text, unique|
|R.9| Ship Date|date, datetime|
|R.10*|	**_Customer Purchase Order PO NUmber_**|number, text, unique|
|R.11*|	**_Customer Bill To Name_**|text|
|R.12|	Customer Bill To Address Street|text|
|R.13|	Customer Bill To Address State|text|
|R.14|	Customer Bill To Address Zip|number|
|R.15|	Customer Bill To Address Country|text|
|R.16|	Customer Ship To Name|text|
|R.17|	Customer Ship To Address Street|text|
|R.18|	Customer Ship To Address State|text|
|R.19|	Customer Ship To Address Zip|text|
|R.20|	Customer Ship To Address Country|text|
|R.21*|	**_End User Name_**|text|
|R.22*|	**_End User Address Street_**|text|
|R.23*|	**_End User Address State_**|text|
|R.24*|	**_End User Address Zip_**|text|
|R.25*|	**_End User Address Country_**|text|
|R.26*|	**_Quantity Ordered_**|number|
|R.27*|	**_Quantity Invoiced_**|number|
|R.28*|	**_Distributor Sku Code_**|number, text|,unique|
|R.29|	Distributor Sku Description|text|
|R.30|	Client Sku Code|number, text|,unique|
|R.31|	Brand Product Desciption|text|
|R.32|	Serial Number|number|

Bold * are mandatory fields to perform initial analysis.

We have perpare the following test cases that will help you to start your audit:

* Be subject to audit (this need to be clear as this is the key to data request)
