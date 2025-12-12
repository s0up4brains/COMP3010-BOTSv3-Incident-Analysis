# COMP3010-BOTSv3-Incident-Analysis

Investigation and report on security incidents using the Boss of the SOC v3 (BOTSv3) dataset within Splunk





##### Introduction





##### SOC Roles

SOC Analyst Method

-Security Alert

-Supporting Evidence

-Analysis

-Conclusion

-Next Steps



##### Incident Handling Reflection





##### Installation \& Data Preparation

tools used



##### AWS endpoint events



TEMPLATE

-Detailed Wxplanation

-Question

-Query

-Timestamp

-Screenshot

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





##### Conclusion

