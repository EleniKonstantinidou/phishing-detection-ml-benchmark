# phishing-detection-ml-benchmark
Benchmarking traditional classifiers, ensemble models (XGBoost, Random Forest), and deep learning (MLPs, Autoencoders) on the UCI Phishing Website dataset.


## **Overview**

Phishing is a widespread cyber threat where malicious entities impersonate legitimate websites to gain sensitive information (e.g., credentials, financial data). This project analyzes website properties and evaluates machine learning classification algorithms to automatically distinguish between legitimate and phishing URLs.

## Dataset Description

The dataset was obtained from the UC Irvine Machine Learning Repository and aggregates samples from sources including the PhishTank archive, MillerSmiles archive, and Google searching operators.

- **Total Instances:** 11,055
- **Total Attributes:** 31 (30 input features + 1 target variable)
- **Feature Data Types:** Integer
- **Missing Values:** 0 (verified with no missing values or unknown '?' symbol)
- **Target Variable (Result):** Binary classification where **1:** Legitimate website & **-1:** Phishing website


## Feature List and Mappings

*Below we outline in detail what each value of the dataset represents in each attribute column.*

**having_IP_Address**  { -1,1 } : -1 for phishing, 1 for legitimate

**URL_Length**   { 1,0,-1 } : 1 for legitimate (short), 0 for suspicious (medium), -1 for phishing (long)

**Shortining_Service** { 1,-1 } : -1 for phishing, 1 for legitimate

**having_At_Symbol**   { 1,-1 } ; -1 for phishing, 1 for legitimate

**double_slash_redirecting** { -1,1 } : -1 for phishing, 1 for legitimate

**Prefix_Suffix**  { -1,1 } : -1 for phishing, 1 for legitimate

**having_Sub_Domain** { -1,0,1 } : 1 for legitimate (no subdomains), 0 for suspicious (one subdomain), -1 for phishing (multiple subdomains)

**SSLfinal_State** { -1,1,0 } : 1 for legitimate, 0 for suspicious, -1 for phishing

**Domain_registeration_length** { -1,1 } : -1 for phishing (short period), 1 for legitimate (long period)

**Favicon** { 1,-1 } : -1 for phishing, 1 for legitimate

**port** { 1,-1 } : -1 for phishing (non-standard ports), 1 for legitimate

**HTTPS_token** { -1,1 } : -1 for phishing, 1 for legitimate

**Request_URL**  { 1,-1 } : -1 for phishing, 1 for legitimate

**URL_of_Anchor** { -1,0,1 } : 1 for legitimate, 0 for suspicious, -1 for phishing

**Links_in_tags** { 1,-1,0 } : 1 for legitimate, 0 for suspicious, -1 for phishing

**SFH**  { -1,1,0 } : 1 for legitimate, 0 for suspicious, -1 for phishing

**Submitting_to_email** { -1,1 } : -1 for phishing, 1 for legitimate

**Abnormal_URL** { -1,1 } : -1 for phishing, 1 for legitimate

**Redirect**  { 0,1 } : 0 for phishing (multiple redirects), 1 for legitimate (single or no redirect)

**on_mouseover**  { 1,-1 } : -1 for phishing, 1 for legitimate

**RightClick**  { 1,-1 } : -1 for phishing, 1 for legitimate

**popUpWidnow**  { 1,-1 } : -1 for phishing, 1 for legitimate

**Iframe** { 1,-1 } : -1 for phishing, 1 for legitimate

**age_of_domain**  { -1,1 } : -1 for phishing (young domain), 1 for legitimate (older domain)

**DNSRecord**   { -1,1 } : -1 for phishing (no record), 1 for legitimate

**web_traffic**  { -1,0,1 } : 1 for legitimate, 0 for suspicious, -1 for phishing

**Page_Rank** { -1,1 } : -1 for phishing, 1 for legitimate

**Google_Index** { 1,-1 } : -1 for phishing, 1 for legitimate

**Links_pointing_to_page** { 1,0,-1 } : 1 for legitimate, 0 for suspicious, -1 for phishing

**Statistical_report** { -1,1 } : -1 for phishing, 1 for legitimate

**Result**  { -1,1 } : -1 for phishing, 1 for legitimate

