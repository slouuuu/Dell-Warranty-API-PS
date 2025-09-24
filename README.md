<h1 align="center">
  <b>Dell Warranty Info</b>
</h1>

<p align="center">
  A PowerShell function to retrieve warranty information for Dell devices using Dell's API.
</p>

<br>

<p align="center">
  <img src="https://img.shields.io/badge/-PowerShell-5391FE?style=for-the-badge&logo=powershell&logoColor=white&labelColor=5391FE">
  <img src="https://img.shields.io/badge/-Dell%20API-007DB8?style=for-the-badge&logo=dell&logoColor=white&labelColor=007DB8">
</p>

<br>

## Quick Start

Replace the placeholder API credentials in the function:

```powershell
$ApiKey = "your_actual_api_key"
$ApiSecret = "your_actual_api_secret"
```


## Usage

### Basic usage
```powershell
$warranty = Get-DellWarrantyInfo -ServiceTag "ABC1234"
```

## Output

The function returns a hashtable with the following properties:

<div align="center">

| Property | Type | Description |
|----------|------|-------------|
| `ServiceTag` | String | Dell service tag |
| `Model` | String | Device model |
| `WarrantyStart` | DateTime | Warranty start date |
| `WarrantyEnd` | DateTime | Warranty end date |
| `SupportLevel` | String | Support level description |
| `IsExpired` | Boolean | Whether warranty has expired |

</div>

## Requirements

<p align="center">
  <img src="https://img.shields.io/badge/PowerShell-3.0+-5391FE?style=flat-square&logo=powershell">
  <img src="https://img.shields.io/badge/Dell%20API-Credentials-blue?style=flat-square">

  
</p>

## Security Note

<div align="center">
  <b>Store API credentials securely in production environments instead of hardcoding them.</b>
</div>

------

<div align="center">
  Last Updated: September 2025
</div>
