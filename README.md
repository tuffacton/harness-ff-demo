# harness-ff-demo

To use:

1) Create a Harness Feature Flag project
2) Create the following flags:
 - Type: Boolean, Name: Builds Module, ID: Builds_Module
 - Type: Boolean, Name: Feature Flag Module, ID: Feature_Flag_Module
 - Type: Boolean, Name: CCM Module, ID: CCM_Module
 - Type: Boolean, Name: CV Module, ID: CV_Module
 - Type: Multivariate, Name: Trial Length, ID: Trial_Length, Values: 7-Day Trial, 14-Day Trial, 30-Day Trial
 
3) Create an environment and SDK key
4) Access the site at http://hostname/index.html?sdkkey=[sdkkey]
5) On first access, you will be prompted to enter an email address. You can use this email address for feature targeting.

Use Cases:
 - Enable/disable the modules at the environment level
 - Enable/disable a module for a specific target
 - Create a Target Group with the rule: "If 'identifier' ends with '@harness.io'" and enable/disable a module for a group of users

