# Dell Warranty Information Tool

## Overview
A PowerShell module that retrieves warranty information for Dell computers using Dell's API. This tool allows you to:

- Retrieve warranty details for Dell computers
- Store API keys
- Save warranty information to the Windows Registry

# Store API key as plain text
Get-DellWarranty -Api

# OR store API key securely (recommended)
Get-DellWarranty -Api -KeyStorage Secure

# Get warranty info for the current computer
Get-DellWarranty -Show

# Get warranty info for a specific Service Tag
Get-DellWarranty -ServiceTag "ABC123D" -Show

# Save warranty info to the registry (requires admin rights)
Get-DellWarranty -Brand

# Get warranty info as an object for further processing
$warrantyInfo = Get-DellWarranty
$warrantyInfo.WarrantyEndDate
