---
title: "Power Apps analytics   | MicrosoftDocs"
description: The admin reports provide a view into environment level usage, errors, service performance.
author: jimholtz
manager: kvivek
ms.service: power-platform
ms.component: pa-admin
ms.topic: conceptual
ms.date: 02/25/2020
ms.author: jimholtz
search.audienceType: 
  - admin
search.app: 
  - D365CE
  - PowerApps
  - Powerplatform
---
# Admin Analytics for Power Apps

Preview of analytics for the environment admin is available at the Power Platform Admin center. The admin reports provide a view into environment level usage, errors, service performance to drive governance, and change management services to users. To view reports, in the Power Platform Admin center menu expand **Analytics** and then select **PowerApps**.  

> [!div class="mx-imgBorder"] 
> ![Power Apps analytics menu](media/powerapps-analytics-menu.png "Power Apps analytics menu")

## Who can view these reports?
Admins with the following roles can view the reports in Power Apps Analytics:
- Environment Admins - can view reports for the environments that the admin has access to.
- Power Platform service admins – can view reports for all environments.
- Office 365 global admins – can view reports for all environments.
- Tenant Admin – can view reports for all environments.

## Where is my data stored? 

When a user first creates an environment from a region, the environment is always hosted in that region. The data is stored only in the region that an environment is hosted in. Data is stored for a maximum of 28 days. The data refresh cycle is about 3 hours and the last refresh time in UTC time standard is displayed on the upper-right corner of the page. 

## What are the available reports? 

The preview contains four reports for Power Apps admins. The last viewed environment is selected by default.  

**Usage** report is the default reports seen by the logged in environment admin. It provides total app launches and daily active users across all apps in the environment. Admins can filter the view with attributes like device platform, player version, country, state, and city.

> [!div class="mx-imgBorder"] 
> ![Power Apps analytics usage report](media/powerapps-analytics-usage.png "Power Apps analytics usage report")

**Location** report provides a map-based view of usage. It gives an insight into regional adoption and usage trends.  

> [!div class="mx-imgBorder"] 
> ![Power Apps analytics location report](media/powerapps-analytics-location.png "Power Apps analytics location report")

**Error** report provides insights into the toast error trends, types, and counts per app to help drive improvements in app quality. The toast errors are errors displayed to the end users of the app. 

> [!div class="mx-imgBorder"] 
> ![Power Apps analytics error report](media/powerapps-analytics-total-errors.png "Power Apps analytics error report")

**Service Performance** report provides details of all standard and custom connectors to understand performance bottlenecks and client versus service API issues. An environment admin will get insights into:  

- Connectors used in the environment. 
- Best and least performant service and the API service response times.  
- Success rates for each service to determine areas that need attention. 
- The 50th, 75th, and 90th percentile response times for each service. 
- The number of HTTP 500 error codes of connectors indicating issues around the server not responding to calls from the client. 
- The number of successful connection requests. 

All the service performance KPI’s can be filtered with attributes like a specific service or connector, device platform, player version, and country, state, or city to drill down into the specific API. 

> [!div class="mx-imgBorder"] 
> ![Power Apps analytics service performance report](media/powerapps-analytics-service-performance.png "Power Apps analytics service performance report")

## How can I download the reports? 

The reports are built on Power BI. To download a report, select the ellipsis (…) of the specific KPI and select **Export data**. 

> [!div class="mx-imgBorder"] 
> ![Power Apps analytics export data](media/powerapps-analytics-export-data.png "Power Apps analytics export data")

## How do I change environments? 

Select **Change Filter** or the **Filter** button (![](media/filters-button.png "Filter button")) in the upper-right corner of the page.

> [!div class="mx-imgBorder"] 
> ![Select Change Filter or Filter](media/powerapps-analytics-filter.png "Select Change Filter or Filter")

Select the environment and time period from the drop-down lists, and then select **Apply** to save the changes. All the Power Apps analytics reports will now use this selection.

> [!div class="mx-imgBorder"] 
> ![Power Apps analytics change environments](media/powerapps-analytics-change-environments.png "Power Apps analytics change environments")
