# AccessReview DataBridge

> Helps IT admins and IGA consultants seamlessly pipe external HR, ITSM, or IGA data into Microsoft Entra Access Reviews without writing brittle custom code.

## Overview

AccessReview DataBridge is a SaaS dashboard that manages the full lifecycle of customDataProvidedResourceUploadSession objects via Microsoft Graph — letting admins upload external reviewer recommendations, monitor session status, and get alerted on failures or expirations. It abstracts away the complex session orchestration, referenceId tracking, and isUploadDone PATCH sequencing into a clean UI with audit logs. MSPs and IGA consultants can white-label it to offer Access Review enrichment as a managed service to their clients.

## Problem This Solves

Manually orchestrating Graph Beta upload sessions — tracking session state, matching source names exactly, PATCHing isUploadDone at the right time, and handling expiry or unknown status failures — is error-prone, undocumented in plain terms, and breaks silently in production, causing Access Reviews to run without the external data they depend on.

## Target Audience

IT admins and IGA/identity governance consultants managing Entra ID Access Reviews at mid-to-large enterprises (500+ users) who rely on external HR or ITSM data to drive review recommendations

## Tech Stack

PHP, Microsoft Graph, PowerShell, OAuth2

## Quick Start

```powershell
# Clone the repository
git clone https://github.com/accessreview-databridge.git
cd accessreview-databridge

# One-click install & run
.\Install.ps1

# Or run the script directly
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
.\scripts\{accessreview-databridge}.ps1
```

## Usage



## Monetization Strategy

SaaS subscription: $39/month per tenant (solo IT admin tier) or $99/month for MSP multi-tenant tier with white-label branding and client dashboard; one-time PowerShell Source Code module also sold at $149 for teams that prefer self-hosted automation

| Metric | Value |
|--------|-------|
| Revenue Potential | HIGH |
| Estimated Effort  | 1-3months |

## About the Author