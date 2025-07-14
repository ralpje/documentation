# Local Admin Rights FAQ 
On this page, you can find some frequently asked questions about using [EPM]("Endpoint Privilige Management"). 

## Installing PowerShell modules

To install PowerShell modules on your system, it is not required to have administrative rights or use EPM. You can install PowerShell module for your current user, by using the `-Scope CurrentUser` parameter. 

``` powershell
    # Installing a module for the current user
    Install-Module AzureAD -Scope CurrentUser
```

## When to use what installation method
The workflow for installing an application is as follows:

``` mermaid
graph LR
    A[Need to install an app] --> B(Is app in company portal?);
    B -->|Yes| C[Install app via Company Portal];
    B -->|No| E[Use EPM to install the app];
```
