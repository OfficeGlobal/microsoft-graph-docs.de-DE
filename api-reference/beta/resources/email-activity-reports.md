---
title: E-Mail-Aktivitätsberichte
description: Sie können eine Ansicht der e-Mail-Verkehr auf oberster Ebene innerhalb Ihrer Organisation über die Seite Berichte abrufen. Sie können auch in der e-Mail-Aktivität-Widget zu verstehen, die Trends und Details pro Benutzer, der die e-Mail-Aktivität in Ihrer Organisation anzeigen.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: reports
ms.openlocfilehash: e11de43f197e520d653961af9b9090d06b085369
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528305"
---
# <a name="email-activity-reports"></a><span data-ttu-id="7846a-104">E-Mail-Aktivitätsberichte</span><span class="sxs-lookup"><span data-stu-id="7846a-104">Email activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7846a-105">Sie können eine Ansicht der e-Mail-Verkehr auf oberster Ebene innerhalb Ihrer Organisation über die Seite Berichte abrufen.</span><span class="sxs-lookup"><span data-stu-id="7846a-105">You can get a high level view of email traffic within your organization from the Reports page.</span></span> <span data-ttu-id="7846a-106">Sie können auch in der e-Mail-Aktivität-Widget zu verstehen, die Trends und Details pro Benutzer, der die e-Mail-Aktivität in Ihrer Organisation anzeigen.</span><span class="sxs-lookup"><span data-stu-id="7846a-106">You can also drill into the Email Activity widget to understand the trends and details per user of the email activity in your organization.</span></span>

> <span data-ttu-id="7846a-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – E-Mail-Aktivität](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="7846a-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="7846a-108">Berichte</span><span class="sxs-lookup"><span data-stu-id="7846a-108">Reports</span></span>

| <span data-ttu-id="7846a-109">Funktion</span><span class="sxs-lookup"><span data-stu-id="7846a-109">Function</span></span>                                 | <span data-ttu-id="7846a-110">Rückgabetyp CSV</span><span class="sxs-lookup"><span data-stu-id="7846a-110">CSV return type</span></span> | <span data-ttu-id="7846a-111">Rückgabetyp JSON</span><span class="sxs-lookup"><span data-stu-id="7846a-111">JSON return type</span></span>                         | <span data-ttu-id="7846a-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7846a-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="7846a-113">Benutzerdetails abrufen</span><span class="sxs-lookup"><span data-stu-id="7846a-113">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="7846a-114">Stream</span><span class="sxs-lookup"><span data-stu-id="7846a-114">Stream</span></span>          | [<span data-ttu-id="7846a-115">emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="7846a-115">emailActivityUserDetail</span></span>](../resources/emailactivityuserdetail.md) | <span data-ttu-id="7846a-116">Erhalten Sie detaillierte Informationen über die von Benutzern ausgeführten E-Mail-Aktivitäten.</span><span class="sxs-lookup"><span data-stu-id="7846a-116">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="7846a-117">Aktivitätsanzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="7846a-117">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="7846a-118">Stream</span><span class="sxs-lookup"><span data-stu-id="7846a-118">Stream</span></span>          | [<span data-ttu-id="7846a-119">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="7846a-119">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="7846a-120">Ermöglicht es Ihnen, einen Überblick über die E-Mail-Aktivitäten (z. B. wie viele E-Mails versendet, gelesen und empfangen wurden) in Ihrer Organisation zu gewinnen.</span><span class="sxs-lookup"><span data-stu-id="7846a-120">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="7846a-121">Benutzeranzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="7846a-121">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="7846a-122">Stream</span><span class="sxs-lookup"><span data-stu-id="7846a-122">Stream</span></span>          | [<span data-ttu-id="7846a-123">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="7846a-123">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="7846a-124">Ermöglicht es Ihnen, sich anhand der Anzahl eindeutiger Benutzer, die E-Mail-Aktivitäten wie Senden, Lesen und Empfangen ausführen, über Trends zu informieren.</span><span class="sxs-lookup"><span data-stu-id="7846a-124">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/email-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
