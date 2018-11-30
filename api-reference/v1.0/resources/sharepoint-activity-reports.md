---
title: SharePoint-Aktivitätsberichte
description: Verwenden Sie die SharePoint-Aktivitätsberichte, um mehr über die Aktivität der für SharePoint lizenzierten Benutzer zu erfahren, indem Sie sich deren Interaktion mit Dateien ansehen. Sie können sich auch den Umfang der Zusammenarbeit basierend auf der Anzahl der freigegebenen Dateien ansehen.
ms.openlocfilehash: b180a098cdec6ef432ec2837c576192e7aa80b1c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016743"
---
# <a name="sharepoint-activity-reports"></a><span data-ttu-id="9ecab-104">SharePoint-Aktivitätsberichte</span><span class="sxs-lookup"><span data-stu-id="9ecab-104">SharePoint activity reports</span></span>

<span data-ttu-id="9ecab-105">Verwenden Sie die SharePoint-Aktivitätsberichte, um mehr über die Aktivität der für SharePoint lizenzierten Benutzer zu erfahren, indem Sie sich deren Interaktion mit Dateien ansehen.</span><span class="sxs-lookup"><span data-stu-id="9ecab-105">You can use the SharePoint activity reports to get the activity of every user licensed to use SharePoint by looking at their interaction with files.</span></span> <span data-ttu-id="9ecab-106">Sie können sich auch den Umfang der Zusammenarbeit basierend auf der Anzahl der freigegebenen Dateien ansehen.</span><span class="sxs-lookup"><span data-stu-id="9ecab-106">You can also look at the level of collaboration going on based on the number of files shared.</span></span>

> <span data-ttu-id="9ecab-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – SharePoint-Aktivität](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="9ecab-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="reports"></a><span data-ttu-id="9ecab-108">Berichte</span><span class="sxs-lookup"><span data-stu-id="9ecab-108">Reports</span></span>

| <span data-ttu-id="9ecab-109">Funktion</span><span class="sxs-lookup"><span data-stu-id="9ecab-109">Function</span></span>                                 | <span data-ttu-id="9ecab-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9ecab-110">Return Type</span></span> | <span data-ttu-id="9ecab-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ecab-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="9ecab-112">Benutzerdetails abrufen</span><span class="sxs-lookup"><span data-stu-id="9ecab-112">Get user detail</span></span>](../api/reportroot-getsharepointactivityuserdetail.md) | <span data-ttu-id="9ecab-113">Stream</span><span class="sxs-lookup"><span data-stu-id="9ecab-113">Stream</span></span>      | <span data-ttu-id="9ecab-114">Rufen Sie Details zu SharePoint-Aktivitäten nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="9ecab-114">Get details about SharePoint activity by user.</span></span> |
| [<span data-ttu-id="9ecab-115">Dateianzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="9ecab-115">Get file counts</span></span>](../api/reportroot-getsharepointactivityfilecounts.md) | <span data-ttu-id="9ecab-116">Stream</span><span class="sxs-lookup"><span data-stu-id="9ecab-116">Stream</span></span>      | <span data-ttu-id="9ecab-117">Erfahren Sie, wie viele eindeutige, lizenzierte Benutzer mit auf SharePoint-Websites gespeicherten Dateien interagiert haben.</span><span class="sxs-lookup"><span data-stu-id="9ecab-117">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span> |
| [<span data-ttu-id="9ecab-118">Benutzeranzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="9ecab-118">Get user counts</span></span>](../api/reportroot-getsharepointactivityusercounts.md) | <span data-ttu-id="9ecab-119">Stream</span><span class="sxs-lookup"><span data-stu-id="9ecab-119">Stream</span></span>      | <span data-ttu-id="9ecab-120">Rufen Sie die Anzahl der aktiven Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="9ecab-120">Get the trend in the number of active users.</span></span> <span data-ttu-id="9ecab-121">Ein Benutzer wird als aktiv betrachtet, wenn er innerhalb des angegebenen Zeitraums eine Dateiaktivität ausgeführt (speichern, synchronisieren, ändern oder freigeben) oder eine Seite besucht hat.</span><span class="sxs-lookup"><span data-stu-id="9ecab-121">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span> |
| [<span data-ttu-id="9ecab-122">Seiten abrufen</span><span class="sxs-lookup"><span data-stu-id="9ecab-122">Get pages</span></span>](../api/reportroot-getsharepointactivitypages.md) | <span data-ttu-id="9ecab-123">Stream</span><span class="sxs-lookup"><span data-stu-id="9ecab-123">Stream</span></span>      | <span data-ttu-id="9ecab-124">Rufen Sie die Anzahl der von Benutzern besuchten eindeutigen Seiten ab.</span><span class="sxs-lookup"><span data-stu-id="9ecab-124">Get the number of unique pages visited by users.</span></span> |