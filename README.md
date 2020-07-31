# DOD-O365-OCE

The DoD Office 365 Connection Evaluator is tailored specifically for DoD environments to check client configuration, O365 connectivity via CAP (Cloud Access Points) and IAP (Internet Access Point) connections.

Resources:

O365 DoD Endpoints- https://docs.microsoft.com/en-us/office365/enterprise/office-365-u-s-government-dod-endpoints

O365 DoD CAs - https://docs.microsoft.com/en-us/microsoft-365/compliance/encryption-office-365-certificate-chains-itar?view=o365-worldwide

Notes:

Trusted Sites config check is a live check, it will pull the DoD Endpoints from the URL above each time it is ran to compare what is applied to trusted sites applied via group policy on the client. As new URLs are added, there may be a gap between the new URL being added and your GPO Management team adding the new site into Trusted Sites GPO. A Partial Failure will occur in this case.
