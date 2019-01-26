---
title: Berichte über aktive Office 365-Benutzer
description: Sie können den Office 365 aktive Benutzer Bericht verwenden, um zu ermitteln, wie viele Lizenzen von Personen in Ihrer Organisation verwendet werden und Ausführen eines Drilldowns Informationen darüber, welche Benutzer welche Produkte verwenden. In diesem Bericht hilft Administratoren nicht ausgelastete Produkte oder Benutzer, die möglicherweise zusätzliche Schulungen oder Informationen zu identifizieren.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 638550fbc44acd0154a2dab5c062e2061fa9c582
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571765"
---
# <a name="office-365-active-users-reports"></a><span data-ttu-id="44aae-104">Berichte über aktive Office 365-Benutzer</span><span class="sxs-lookup"><span data-stu-id="44aae-104">Office 365 active users reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44aae-105">Sie können den Office 365 aktive Benutzer Bericht verwenden, um zu ermitteln, wie viele Lizenzen von Personen in Ihrer Organisation verwendet werden und Ausführen eines Drilldowns Informationen darüber, welche Benutzer welche Produkte verwenden.</span><span class="sxs-lookup"><span data-stu-id="44aae-105">You can use the Office 365 active users report to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="44aae-106">In diesem Bericht hilft Administratoren nicht ausgelastete Produkte oder Benutzer, die möglicherweise zusätzliche Schulungen oder Informationen zu identifizieren.</span><span class="sxs-lookup"><span data-stu-id="44aae-106">This report can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="44aae-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Aktive Benutzer](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="44aae-107">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="44aae-108">Berichte</span><span class="sxs-lookup"><span data-stu-id="44aae-108">Reports</span></span>
| <span data-ttu-id="44aae-109">Function</span><span class="sxs-lookup"><span data-stu-id="44aae-109">Function</span></span>                                 | <span data-ttu-id="44aae-110">Rückgabetyp CSV</span><span class="sxs-lookup"><span data-stu-id="44aae-110">CSV return type</span></span> | <span data-ttu-id="44aae-111">Rückgabetyp JSON</span><span class="sxs-lookup"><span data-stu-id="44aae-111">JSON return type</span></span>                         | <span data-ttu-id="44aae-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="44aae-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="44aae-113">Benutzerdetails abrufen</span><span class="sxs-lookup"><span data-stu-id="44aae-113">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="44aae-114">Stream</span><span class="sxs-lookup"><span data-stu-id="44aae-114">Stream</span></span>          | [<span data-ttu-id="44aae-115">office365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="44aae-115">office365ActiveUserDetail</span></span>](../resources/office365activeuserdetail.md) | <span data-ttu-id="44aae-116">Rufen Sie Details zu aktiven Office 365-Benutzern ab.</span><span class="sxs-lookup"><span data-stu-id="44aae-116">Get details about Office 365 active users.</span></span> |
| [<span data-ttu-id="44aae-117">Benutzeranzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="44aae-117">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="44aae-118">Stream</span><span class="sxs-lookup"><span data-stu-id="44aae-118">Stream</span></span>          | [<span data-ttu-id="44aae-119">office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="44aae-119">office365ActiveUserCounts</span></span>](../resources/office365activeusercounts.md) | <span data-ttu-id="44aae-120">Rufen Sie die Anzahl der im Berichtszeitraum täglich aktiven Benutzer nach Produkt ab.</span><span class="sxs-lookup"><span data-stu-id="44aae-120">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="44aae-121">Benutzeranzahl für Dienste abrufen</span><span class="sxs-lookup"><span data-stu-id="44aae-121">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="44aae-122">Stream</span><span class="sxs-lookup"><span data-stu-id="44aae-122">Stream</span></span>          | [<span data-ttu-id="44aae-123">office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="44aae-123">office365ServicesUserCounts</span></span>](../resources/office365servicesusercounts.md) | <span data-ttu-id="44aae-124">Rufen Sie die Anzahl der Benutzer nach Aktivitätstyp und Dienst ab.</span><span class="sxs-lookup"><span data-stu-id="44aae-124">Get the count of users by activity type and service.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-active-users-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
