---
title: Berichte über aktive Office 365-Benutzer
description: Sie können den Office 365 aktive Benutzer Bericht verwenden, um zu ermitteln, wie viele Lizenzen von Personen in Ihrer Organisation verwendet werden und Ausführen eines Drilldowns Informationen darüber, welche Benutzer welche Produkte verwenden. In diesem Bericht hilft Administratoren nicht ausgelastete Produkte oder Benutzer, die möglicherweise zusätzliche Schulungen oder Informationen zu identifizieren.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: e85924b7066dde92f0db5fd0b3f1f83dd32fd0c1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516210"
---
# <a name="office-365-active-users-reports"></a><span data-ttu-id="0e298-104">Berichte über aktive Office 365-Benutzer</span><span class="sxs-lookup"><span data-stu-id="0e298-104">Office 365 active users reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e298-105">Sie können den Office 365 aktive Benutzer Bericht verwenden, um zu ermitteln, wie viele Lizenzen von Personen in Ihrer Organisation verwendet werden und Ausführen eines Drilldowns Informationen darüber, welche Benutzer welche Produkte verwenden.</span><span class="sxs-lookup"><span data-stu-id="0e298-105">You can use the Office 365 active users report to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="0e298-106">In diesem Bericht hilft Administratoren nicht ausgelastete Produkte oder Benutzer, die möglicherweise zusätzliche Schulungen oder Informationen zu identifizieren.</span><span class="sxs-lookup"><span data-stu-id="0e298-106">This report can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="0e298-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Aktive Benutzer](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="0e298-107">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="0e298-108">Berichte</span><span class="sxs-lookup"><span data-stu-id="0e298-108">Reports</span></span>
| <span data-ttu-id="0e298-109">Funktion</span><span class="sxs-lookup"><span data-stu-id="0e298-109">Function</span></span>                                 | <span data-ttu-id="0e298-110">Rückgabetyp CSV</span><span class="sxs-lookup"><span data-stu-id="0e298-110">CSV return type</span></span> | <span data-ttu-id="0e298-111">Rückgabetyp JSON</span><span class="sxs-lookup"><span data-stu-id="0e298-111">JSON return type</span></span>                         | <span data-ttu-id="0e298-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e298-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="0e298-113">Benutzerdetails abrufen</span><span class="sxs-lookup"><span data-stu-id="0e298-113">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="0e298-114">Stream</span><span class="sxs-lookup"><span data-stu-id="0e298-114">Stream</span></span>          | [<span data-ttu-id="0e298-115">office365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="0e298-115">office365ActiveUserDetail</span></span>](../resources/office365activeuserdetail.md) | <span data-ttu-id="0e298-116">Rufen Sie Details zu aktiven Office 365-Benutzern ab.</span><span class="sxs-lookup"><span data-stu-id="0e298-116">Get details about Office 365 active users.</span></span> |
| [<span data-ttu-id="0e298-117">Benutzeranzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="0e298-117">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="0e298-118">Stream</span><span class="sxs-lookup"><span data-stu-id="0e298-118">Stream</span></span>          | [<span data-ttu-id="0e298-119">office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="0e298-119">office365ActiveUserCounts</span></span>](../resources/office365activeusercounts.md) | <span data-ttu-id="0e298-120">Rufen Sie die Anzahl der im Berichtszeitraum täglich aktiven Benutzer nach Produkt ab.</span><span class="sxs-lookup"><span data-stu-id="0e298-120">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="0e298-121">Benutzeranzahl für Dienste abrufen</span><span class="sxs-lookup"><span data-stu-id="0e298-121">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="0e298-122">Stream</span><span class="sxs-lookup"><span data-stu-id="0e298-122">Stream</span></span>          | [<span data-ttu-id="0e298-123">office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="0e298-123">office365ServicesUserCounts</span></span>](../resources/office365servicesusercounts.md) | <span data-ttu-id="0e298-124">Rufen Sie die Anzahl der Benutzer nach Aktivitätstyp und Dienst ab.</span><span class="sxs-lookup"><span data-stu-id="0e298-124">Get the count of users by activity type and service.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-active-users-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
