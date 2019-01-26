---
title: Verwendungsberichte für Yammer-Gerät
description: Die Verwendungsberichte für das Yammer-Gerät geben Aufschluss darüber, welche Geräte Ihre Benutzer für die Nutzung von Yammer verwenden. Sie können sich die Anzahl der Benutzer nach Gerätetyp für einen gewählten Zeitraum ansehen und Details für einzelne Benutzer anzeigen.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 57dcba3a91b15b4980d9e76b7aad6251008f5966
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577431"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="ca32b-104">Verwendungsberichte für Yammer-Gerät</span><span class="sxs-lookup"><span data-stu-id="ca32b-104">Yammer device usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca32b-105">Die Verwendungsberichte für das Yammer-Gerät geben Aufschluss darüber, welche Geräte Ihre Benutzer für die Nutzung von Yammer verwenden.</span><span class="sxs-lookup"><span data-stu-id="ca32b-105">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="ca32b-106">Sie können sich die Anzahl der Benutzer nach Gerätetyp für einen gewählten Zeitraum ansehen und Details für einzelne Benutzer anzeigen.</span><span class="sxs-lookup"><span data-stu-id="ca32b-106">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="ca32b-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Gerätenutzung](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="ca32b-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="ca32b-108">Berichte</span><span class="sxs-lookup"><span data-stu-id="ca32b-108">Reports</span></span>

| <span data-ttu-id="ca32b-109">Function</span><span class="sxs-lookup"><span data-stu-id="ca32b-109">Function</span></span>                                 | <span data-ttu-id="ca32b-110">Rückgabetyp CSV</span><span class="sxs-lookup"><span data-stu-id="ca32b-110">CSV return type</span></span> | <span data-ttu-id="ca32b-111">Rückgabetyp JSON</span><span class="sxs-lookup"><span data-stu-id="ca32b-111">JSON return type</span></span>                         | <span data-ttu-id="ca32b-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ca32b-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="ca32b-113">Benutzerdetails abrufen</span><span class="sxs-lookup"><span data-stu-id="ca32b-113">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="ca32b-114">Stream</span><span class="sxs-lookup"><span data-stu-id="ca32b-114">Stream</span></span>          | [<span data-ttu-id="ca32b-115">yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="ca32b-115">yammerDeviceUsageUserDetail</span></span>](../resources/yammerdeviceusageuserdetail.md) | <span data-ttu-id="ca32b-116">Rufen Sie Details zur Yammer-Gerätenutzung nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="ca32b-116">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="ca32b-117">Benutzeranzahl für Verteilung abrufen</span><span class="sxs-lookup"><span data-stu-id="ca32b-117">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="ca32b-118">Stream</span><span class="sxs-lookup"><span data-stu-id="ca32b-118">Stream</span></span>          | [<span data-ttu-id="ca32b-119">yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="ca32b-119">yammerDeviceUsageDistributionUserCounts</span></span>](../resources/yammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="ca32b-120">Erhalten Sie die Anzahl der Benutzer nach Gerätetyp.</span><span class="sxs-lookup"><span data-stu-id="ca32b-120">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="ca32b-121">Benutzeranzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="ca32b-121">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="ca32b-122">Stream</span><span class="sxs-lookup"><span data-stu-id="ca32b-122">Stream</span></span>          | [<span data-ttu-id="ca32b-123">yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="ca32b-123">yammerDeviceUsageUserCounts</span></span>](../resources/yammerdeviceusageusercounts.md) | <span data-ttu-id="ca32b-124">Erhalten Sie die Anzahl der täglichen Benutzer nach Gerätetyp.</span><span class="sxs-lookup"><span data-stu-id="ca32b-124">Get the number of daily users by device type.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-device-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
