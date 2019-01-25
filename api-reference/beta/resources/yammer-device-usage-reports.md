---
title: Verwendungsberichte für Yammer-Gerät
description: Die Verwendungsberichte für das Yammer-Gerät geben Aufschluss darüber, welche Geräte Ihre Benutzer für die Nutzung von Yammer verwenden. Sie können sich die Anzahl der Benutzer nach Gerätetyp für einen gewählten Zeitraum ansehen und Details für einzelne Benutzer anzeigen.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: f5b24d6d235a8719f5f4b7df0389b5e5971dd8cf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521866"
---
# <a name="yammer-device-usage-reports"></a><span data-ttu-id="46846-104">Verwendungsberichte für Yammer-Gerät</span><span class="sxs-lookup"><span data-stu-id="46846-104">Yammer device usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46846-105">Die Verwendungsberichte für das Yammer-Gerät geben Aufschluss darüber, welche Geräte Ihre Benutzer für die Nutzung von Yammer verwenden.</span><span class="sxs-lookup"><span data-stu-id="46846-105">The device usage reports for Yammer give you information about which devices your users utilize to engage on Yammer.</span></span> <span data-ttu-id="46846-106">Sie können sich die Anzahl der Benutzer nach Gerätetyp für einen gewählten Zeitraum ansehen und Details für einzelne Benutzer anzeigen.</span><span class="sxs-lookup"><span data-stu-id="46846-106">You can view the number of users by device type over a selected time period and view details by user.</span></span>

> <span data-ttu-id="46846-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Gerätenutzung](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="46846-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="reports"></a><span data-ttu-id="46846-108">Berichte</span><span class="sxs-lookup"><span data-stu-id="46846-108">Reports</span></span>

| <span data-ttu-id="46846-109">Funktion</span><span class="sxs-lookup"><span data-stu-id="46846-109">Function</span></span>                                 | <span data-ttu-id="46846-110">Rückgabetyp CSV</span><span class="sxs-lookup"><span data-stu-id="46846-110">CSV return type</span></span> | <span data-ttu-id="46846-111">Rückgabetyp JSON</span><span class="sxs-lookup"><span data-stu-id="46846-111">JSON return type</span></span>                         | <span data-ttu-id="46846-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46846-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="46846-113">Benutzerdetails abrufen</span><span class="sxs-lookup"><span data-stu-id="46846-113">Get user detail</span></span>](../api/reportroot-getyammerdeviceusageuserdetail.md) | <span data-ttu-id="46846-114">Stream</span><span class="sxs-lookup"><span data-stu-id="46846-114">Stream</span></span>          | [<span data-ttu-id="46846-115">yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="46846-115">yammerDeviceUsageUserDetail</span></span>](../resources/yammerdeviceusageuserdetail.md) | <span data-ttu-id="46846-116">Rufen Sie Details zur Yammer-Gerätenutzung nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="46846-116">Get details about Yammer device usage by user.</span></span> |
| [<span data-ttu-id="46846-117">Benutzeranzahl für Verteilung abrufen</span><span class="sxs-lookup"><span data-stu-id="46846-117">Get distribution user counts</span></span>](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="46846-118">Stream</span><span class="sxs-lookup"><span data-stu-id="46846-118">Stream</span></span>          | [<span data-ttu-id="46846-119">yammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="46846-119">yammerDeviceUsageDistributionUserCounts</span></span>](../resources/yammerdeviceusagedistributionusercounts.md) | <span data-ttu-id="46846-120">Erhalten Sie die Anzahl der Benutzer nach Gerätetyp.</span><span class="sxs-lookup"><span data-stu-id="46846-120">Get the number of users by device type.</span></span>  |
| [<span data-ttu-id="46846-121">Benutzeranzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="46846-121">Get user counts</span></span>](../api/reportroot-getyammerdeviceusageusercounts.md) | <span data-ttu-id="46846-122">Stream</span><span class="sxs-lookup"><span data-stu-id="46846-122">Stream</span></span>          | [<span data-ttu-id="46846-123">yammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="46846-123">yammerDeviceUsageUserCounts</span></span>](../resources/yammerdeviceusageusercounts.md) | <span data-ttu-id="46846-124">Erhalten Sie die Anzahl der täglichen Benutzer nach Gerätetyp.</span><span class="sxs-lookup"><span data-stu-id="46846-124">Get the number of daily users by device type.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-device-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
