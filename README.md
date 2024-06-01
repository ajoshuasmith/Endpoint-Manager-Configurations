# Endpoint-Manager-Configurations

These are JSON files that can be imported into Microsoft 365 to automatically create these policies so you are not digging through the platform. These JSON files were exported out of Microsoft tenants and were utilized for rapid deployment across tenants to save labor time while also creating a baseline standard of what I used in tenants. Most of these JSON files will IMPROVE your Secure Score. I averaged around 700-800 with Business Premium Licensing. This does not account for all of the additional security features that are added NOT within Endpoint Manager such as Spam, Phishing, Malware, Safe Links, Safe Attachments, DKIM and much much more.

I strongly recommend you to utilize [cipp.app](https://cipp.app/) for this importing of JSON files as it is MUCH easier and you will get other Microsoft 365 management benefits. It costs less than $20 a month to run on Azure. 

If you do not have access to CIPP, there is a PowerShell method that is documented over at [https://github.com/microsoftgraph/powershell-intune-samples/tree/master/SettingsCatalog](https://github.com/microsoftgraph/powershell-intune-samples/tree/master)



References:
https://learn.microsoft.com/en-us/answers/questions/1259549/export-import-intune-tenant-settings-(windows-conf
You will need to connect to Microsoft 365 with a Global Administrator
Uninstall-Module -Name AzureAD (uninstall AzureAD if you previously had it installed)
Install-Module -Name AzureAD -RequiredVersion 2.0.2.140 (this version fixes the errors)

