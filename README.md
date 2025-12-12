# COMP3010-BOTSv3-Incident-Analysis

Investigation and report on security incidents using the Boss of the SOC v3 (BOTSv3) dataset within Splunk





##### Introduction

-SOC Context Overview

-BOTSv3 Exercise

-Investigation Objectives

-Define Scope

-Define Assumptions



##### SOC Roles

SOC Tiers



SOC Responsibilities





SOC Analyst Method

-Security Alert

-Supporting Evidence

-Analysis

-Conclusion

-Next Steps



##### Incident Handling Reflection



Incident handling methodology

-prevention

-detection

-response

-recovery





##### Installation \& Data Preparation



Linux

splunk installation

dataset ingestion \& validation

tools used



Justify Decisions in context of SOC infrastructure

Evidence



##### AWS endpoint events



TEMPLATE

-Detailed Explanation with SOC Relevance

-Question

-Query

-Timestamp

-Screenshot

-Dashboards

-Answer

-Threat Intel Lookup





Question 1. IAM users that accessed an AWS service

-Detailed Explanation



Query: index=botsv3 sourcetype="aws:cloudtrail" userIdentity.type=IAMUser

| stats values(userIdentity.userName) as users

-Timestamp

-Screenshot

Answer: bstoll,btun,splunk\_access,web\_admin

-Threat Intel Lookup







###### Indicators of Compromise

###### 

###### Detection Methodology



###### Chronology of Events



TIMESTAMP HERE user 'bstoll' (Bud) logged in with Multi Factor Authenication



TIMESTAMP HERE S3 Bucket 'frothlywebcode' was made publicly accessible using (COMMAND HERE)



TIMESTAMP HERE Text file 'OPEN\_BUCKET\_PLEAE\_FIX.txt' was uploaded to the open bucket



TIMESTAMP HERE S3 Bucket 'frothlywebcode' was made private again





##### Conclusion



Findings

Key Lessons

SOC strategy implications

Improvements to be made to detection and response



References (IEEE style)







