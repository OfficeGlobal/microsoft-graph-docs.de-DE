---
title: E-Mail-App-Verwendungsbericht
description: Sie können sehen, wie viele e-Mail-apps für die Verbindung zu Exchange Online verwendet werden. Sie können auch nachsehen, welche Versionen von Outlook-Apps verwendet werden, sodass Sie Benutzer informieren können, die auf unterstützte Outlook-Versionen upgraden sollten.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: 7f332359af9a6147894bb69e6d12532a83394bb5
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573746"
---
# <a name="email-app-usage-reports"></a><span data-ttu-id="7a689-104">E-Mail-App-Verwendungsbericht</span><span class="sxs-lookup"><span data-stu-id="7a689-104">Email app usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a689-105">Sie können sehen, wie viele e-Mail-apps für die Verbindung zu Exchange Online verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="7a689-105">You can see how many email apps are used to connect to Exchange Online.</span></span> <span data-ttu-id="7a689-106">Sie können auch nachsehen, welche Versionen von Outlook-Apps verwendet werden, sodass Sie Benutzer informieren können, die auf unterstützte Outlook-Versionen upgraden sollten.</span><span class="sxs-lookup"><span data-stu-id="7a689-106">You can also see which versions of Outlook apps are used which will enable you to follow up with users who should upgrade to supported Outlook versions.</span></span>

> <span data-ttu-id="7a689-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Nutzung von E-Mail-Apps](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="7a689-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="reports"></a><span data-ttu-id="7a689-108">Berichte</span><span class="sxs-lookup"><span data-stu-id="7a689-108">Reports</span></span>

| <span data-ttu-id="7a689-109">Function</span><span class="sxs-lookup"><span data-stu-id="7a689-109">Function</span></span>                                 | <span data-ttu-id="7a689-110">Rückgabetyp CSV</span><span class="sxs-lookup"><span data-stu-id="7a689-110">CSV return type</span></span> | <span data-ttu-id="7a689-111">Rückgabetyp JSON</span><span class="sxs-lookup"><span data-stu-id="7a689-111">JSON return type</span></span>                         | <span data-ttu-id="7a689-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7a689-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="7a689-113">Benutzerdetails abrufen</span><span class="sxs-lookup"><span data-stu-id="7a689-113">Get user detail</span></span>](../api/reportroot-getemailappusageuserdetail.md) | <span data-ttu-id="7a689-114">Stream</span><span class="sxs-lookup"><span data-stu-id="7a689-114">Stream</span></span>          | [<span data-ttu-id="7a689-115">emailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="7a689-115">emailAppUsageUserDetail</span></span>](../resources/emailappusageuserdetail.md) | <span data-ttu-id="7a689-116">Erhalten Sie detaillierte Informationen darüber, welche Aktivitäten Benutzer mit den verschiedenen E-Mail-Apps ausgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="7a689-116">Get details about which activities users performed on the various email apps.</span></span> |
| [<span data-ttu-id="7a689-117">Benutzeranzahl für Apps abrufen</span><span class="sxs-lookup"><span data-stu-id="7a689-117">Get apps user counts</span></span>](../api/reportroot-getemailappusageappsusercounts.md) | <span data-ttu-id="7a689-118">Stream</span><span class="sxs-lookup"><span data-stu-id="7a689-118">Stream</span></span>          | [<span data-ttu-id="7a689-119">emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="7a689-119">emailAppUsageAppsUserCounts</span></span>](../resources/emailappusageappsusercounts.md) | <span data-ttu-id="7a689-120">Rufen Sie die Anzahl der eindeutigen Benutzer pro E-Mail-App ab.</span><span class="sxs-lookup"><span data-stu-id="7a689-120">Get the count of unique users per email app.</span></span> |
| [<span data-ttu-id="7a689-121">Benutzeranzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="7a689-121">Get user counts</span></span>](../api/reportroot-getemailappusageusercounts.md) | <span data-ttu-id="7a689-122">Stream</span><span class="sxs-lookup"><span data-stu-id="7a689-122">Stream</span></span>          | [<span data-ttu-id="7a689-123">emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="7a689-123">emailAppUsageUserCounts</span></span>](../resources/emailappusageusercounts.md) | <span data-ttu-id="7a689-124">Rufen Sie die Anzahl der eindeutigen Benutzer ab, die über eine E-Mail-App mit Exchange Online verbunden sind.</span><span class="sxs-lookup"><span data-stu-id="7a689-124">Get the count of unique users that connected to Exchange Online using any email app.</span></span> |
| [<span data-ttu-id="7a689-125">Benutzeranzahl für Versionen abrufen</span><span class="sxs-lookup"><span data-stu-id="7a689-125">Get versions user counts</span></span>](../api/reportroot-getemailappusageversionsusercounts.md) | <span data-ttu-id="7a689-126">Stream</span><span class="sxs-lookup"><span data-stu-id="7a689-126">Stream</span></span>          | [<span data-ttu-id="7a689-127">emailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="7a689-127">emailAppUsageVersionsUserCounts</span></span>](../resources/emailappusageversionsusercounts.md) | <span data-ttu-id="7a689-128">Rufen Sie die Anzahl der eindeutigen Benutzer der Desktopversion von Outlook ab.</span><span class="sxs-lookup"><span data-stu-id="7a689-128">Get the count of unique users by Outlook desktop version.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/email-app-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
