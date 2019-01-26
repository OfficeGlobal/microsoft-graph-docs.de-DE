---
title: Microsoft Teams-Gerätenutzungsberichte
description: 'Verwenden Sie die Berichte zur Verwendung der Microsoft-Teams, Gerät, um Einblicke in die Microsoft-Teams Gerät Verwendung in Ihrer Organisation abzurufen. '
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d19df5132a67ac5862535a329eadbdff7044798c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576640"
---
# <a name="microsoft-teams-device-usage-reports"></a><span data-ttu-id="d11d7-103">Microsoft Teams-Gerätenutzungsberichte</span><span class="sxs-lookup"><span data-stu-id="d11d7-103">Microsoft Teams device usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d11d7-104">Verwenden Sie die Berichte zur Verwendung der Microsoft-Teams, Gerät, um Einblicke in die Microsoft-Teams Gerät Verwendung in Ihrer Organisation abzurufen.</span><span class="sxs-lookup"><span data-stu-id="d11d7-104">Use the Microsoft Teams device usage reports to get insights into the Microsoft Teams device usage in your organization.</span></span> 

## <a name="methods"></a><span data-ttu-id="d11d7-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="d11d7-105">Methods</span></span>

| <span data-ttu-id="d11d7-106">Methode</span><span class="sxs-lookup"><span data-stu-id="d11d7-106">Method</span></span>                                   | <span data-ttu-id="d11d7-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d11d7-107">Return Type</span></span>                              | <span data-ttu-id="d11d7-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d11d7-108">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="d11d7-109">Benutzerdetails abrufen</span><span class="sxs-lookup"><span data-stu-id="d11d7-109">Get user detail</span></span>](../api/reportroot-getteamsdeviceusageuserdetail.md) | [<span data-ttu-id="d11d7-110">teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="d11d7-110">teamsDeviceUsageUserDetail</span></span>](../resources/teamsdeviceusageuserdetail.md) | <span data-ttu-id="d11d7-111">Abrufen von Details zur Microsoft Teams-Gerätenutzung nach Benutzer.</span><span class="sxs-lookup"><span data-stu-id="d11d7-111">Get details about Microsoft Teams device usage by user.</span></span> |
| [<span data-ttu-id="d11d7-112">Benutzeranzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="d11d7-112">Get user counts</span></span>](../api/reportroot-getteamsdeviceusageusercounts.md) | [<span data-ttu-id="d11d7-113">teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="d11d7-113">teamsDeviceUsageUserCounts</span></span>](../resources/teamsdeviceusageusercounts.md) | <span data-ttu-id="d11d7-114">Abrufen der Anzahl der täglichen eindeutigen Benutzer nach Gerätetyp.</span><span class="sxs-lookup"><span data-stu-id="d11d7-114">Get the number of daily unique users by device type.</span></span> |
| [<span data-ttu-id="d11d7-115">Benutzeranzahl für Verteilung abrufen</span><span class="sxs-lookup"><span data-stu-id="d11d7-115">Get distribution user counts</span></span>](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [<span data-ttu-id="d11d7-116">teamsDeviceUsagedistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="d11d7-116">teamsDeviceUsagedistributionUserCounts</span></span>](../resources/teamsdeviceusagedistributionusercounts.md) | <span data-ttu-id="d11d7-117">Abrufen der Anzahl der eindeutigen Benutzer nach Gerätetyp im ausgewählten Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="d11d7-117">Get the number of unique users by device type over the selected time period.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/microsoft-teams-device-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
