---
title: Ressourcentyp office365ServicesUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 18282aaa8dcd176a6eaa3a8176154670bfd6da9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808015"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="3bc13-103">Ressourcentyp office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="3bc13-103">office365ServicesUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="3bc13-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3bc13-104">Properties</span></span>

| <span data-ttu-id="3bc13-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3bc13-105">Property</span></span>                 | <span data-ttu-id="3bc13-106">Typ</span><span class="sxs-lookup"><span data-stu-id="3bc13-106">Type</span></span>   | <span data-ttu-id="3bc13-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3bc13-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="3bc13-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="3bc13-108">reportRefreshDate</span></span>        | <span data-ttu-id="3bc13-109">Datum</span><span class="sxs-lookup"><span data-stu-id="3bc13-109">Date</span></span>   | <span data-ttu-id="3bc13-110">Das aktuelle Datum des Inhalts.</span><span class="sxs-lookup"><span data-stu-id="3bc13-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="3bc13-111">exchangeActive</span><span class="sxs-lookup"><span data-stu-id="3bc13-111">exchangeActive</span></span>           | <span data-ttu-id="3bc13-112">Int64</span><span class="sxs-lookup"><span data-stu-id="3bc13-112">Int64</span></span>  | <span data-ttu-id="3bc13-113">Die Anzahl von aktiven Benutzern auf Exchange.</span><span class="sxs-lookup"><span data-stu-id="3bc13-113">The number of active users on Exchange.</span></span> <span data-ttu-id="3bc13-114">Jeder Benutzer, der lesen und e-Mail senden kann, wird einen aktiven Benutzer betrachtet.</span><span class="sxs-lookup"><span data-stu-id="3bc13-114">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="3bc13-115">exchangeInactive</span><span class="sxs-lookup"><span data-stu-id="3bc13-115">exchangeInactive</span></span>         | <span data-ttu-id="3bc13-116">Int64</span><span class="sxs-lookup"><span data-stu-id="3bc13-116">Int64</span></span>  | <span data-ttu-id="3bc13-117">Die Anzahl der inaktive Benutzer auf Exchange.</span><span class="sxs-lookup"><span data-stu-id="3bc13-117">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="3bc13-118">oneDriveActive</span><span class="sxs-lookup"><span data-stu-id="3bc13-118">oneDriveActive</span></span>           | <span data-ttu-id="3bc13-119">Int64</span><span class="sxs-lookup"><span data-stu-id="3bc13-119">Int64</span></span>  | <span data-ttu-id="3bc13-120">Die Anzahl von aktiven Benutzern in OneDrive.</span><span class="sxs-lookup"><span data-stu-id="3bc13-120">The number of active users on OneDrive.</span></span> <span data-ttu-id="3bc13-121">Jeder Benutzer, der angezeigt oder bearbeitet Dateien, freigegebenen Dateien intern oder extern oder Dateien synchronisiert wird einen aktiven Benutzer betrachtet.</span><span class="sxs-lookup"><span data-stu-id="3bc13-121">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="3bc13-122">oneDriveInactive</span><span class="sxs-lookup"><span data-stu-id="3bc13-122">oneDriveInactive</span></span>         | <span data-ttu-id="3bc13-123">Int64</span><span class="sxs-lookup"><span data-stu-id="3bc13-123">Int64</span></span>  | <span data-ttu-id="3bc13-124">Die Anzahl der inaktive Benutzer in OneDrive.</span><span class="sxs-lookup"><span data-stu-id="3bc13-124">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="3bc13-125">sharePointActive</span><span class="sxs-lookup"><span data-stu-id="3bc13-125">sharePointActive</span></span>         | <span data-ttu-id="3bc13-126">Int64</span><span class="sxs-lookup"><span data-stu-id="3bc13-126">Int64</span></span>  | <span data-ttu-id="3bc13-127">Die Anzahl der aktive Benutzer in SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3bc13-127">The number of active users on SharePoint.</span></span> <span data-ttu-id="3bc13-128">Jeder Benutzer, der angezeigt oder bearbeitet Dateien, gemeinsam genutzte Dateien intern oder extern, synchronisiert Dateien oder SharePoint-Seiten angezeigt wird einen aktiven Benutzer betrachtet.</span><span class="sxs-lookup"><span data-stu-id="3bc13-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="3bc13-129">sharePointInactive</span><span class="sxs-lookup"><span data-stu-id="3bc13-129">sharePointInactive</span></span>       | <span data-ttu-id="3bc13-130">Int64</span><span class="sxs-lookup"><span data-stu-id="3bc13-130">Int64</span></span>  | <span data-ttu-id="3bc13-131">Die Anzahl der inaktive Benutzer auf SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3bc13-131">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="3bc13-132">skypeForBusinessActive</span><span class="sxs-lookup"><span data-stu-id="3bc13-132">skypeForBusinessActive</span></span>   | <span data-ttu-id="3bc13-133">Int64</span><span class="sxs-lookup"><span data-stu-id="3bc13-133">Int64</span></span>  | <span data-ttu-id="3bc13-134">Die Anzahl von aktiven Benutzern auf Skype für Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="3bc13-134">The number of active users on Skype For Business.</span></span> <span data-ttu-id="3bc13-135">Jeder Benutzer, die organisiert oder in Konferenzen teilgenommen Peer-zu-Peer-Sitzungen verbunden wird einen aktiven Benutzer betrachtet.</span><span class="sxs-lookup"><span data-stu-id="3bc13-135">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="3bc13-136">skypeForBusinessInactive</span><span class="sxs-lookup"><span data-stu-id="3bc13-136">skypeForBusinessInactive</span></span> | <span data-ttu-id="3bc13-137">Int64</span><span class="sxs-lookup"><span data-stu-id="3bc13-137">Int64</span></span>  | <span data-ttu-id="3bc13-138">Die Anzahl der inaktive Benutzer auf Skype für Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="3bc13-138">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="3bc13-139">yammerActive</span><span class="sxs-lookup"><span data-stu-id="3bc13-139">yammerActive</span></span>             | <span data-ttu-id="3bc13-140">Int64</span><span class="sxs-lookup"><span data-stu-id="3bc13-140">Int64</span></span>  | <span data-ttu-id="3bc13-141">Die Anzahl der aktive Benutzer in Yammer.</span><span class="sxs-lookup"><span data-stu-id="3bc13-141">The number of active users on Yammer.</span></span> <span data-ttu-id="3bc13-142">Jeder Benutzer kann buchen, lesen oder like Nachrichten wird einen aktiven Benutzer betrachtet.</span><span class="sxs-lookup"><span data-stu-id="3bc13-142">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="3bc13-143">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="3bc13-143">yammerInactive</span></span>           | <span data-ttu-id="3bc13-144">Int64</span><span class="sxs-lookup"><span data-stu-id="3bc13-144">Int64</span></span>  | <span data-ttu-id="3bc13-145">Die Anzahl der inaktive Benutzer auf Yammer.</span><span class="sxs-lookup"><span data-stu-id="3bc13-145">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="3bc13-146">teamsActive</span><span class="sxs-lookup"><span data-stu-id="3bc13-146">teamsActive</span></span>              | <span data-ttu-id="3bc13-147">Int64</span><span class="sxs-lookup"><span data-stu-id="3bc13-147">Int64</span></span>  | <span data-ttu-id="3bc13-148">Die Anzahl von aktiven Benutzern auf Teams.</span><span class="sxs-lookup"><span data-stu-id="3bc13-148">The number of active users on Teams.</span></span> <span data-ttu-id="3bc13-149">Jeder Benutzer, die Nachrichten im Team Kanäle gebucht, gesendete Nachrichten in privaten chatten oder Besprechungen oder Anrufe beteiligt ist einen aktiven Benutzer betrachtet.</span><span class="sxs-lookup"><span data-stu-id="3bc13-149">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="3bc13-150">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="3bc13-150">teamsInactive</span></span>            | <span data-ttu-id="3bc13-151">Int64</span><span class="sxs-lookup"><span data-stu-id="3bc13-151">Int64</span></span>  | <span data-ttu-id="3bc13-152">Die Anzahl von aktiven Benutzern auf Teams.</span><span class="sxs-lookup"><span data-stu-id="3bc13-152">The number of active users on Teams.</span></span>     |
| <span data-ttu-id="3bc13-153">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="3bc13-153">reportPeriod</span></span>             | <span data-ttu-id="3bc13-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3bc13-154">String</span></span> | <span data-ttu-id="3bc13-155">Die Anzahl der Tage, die der Bericht wird behandelt.</span><span class="sxs-lookup"><span data-stu-id="3bc13-155">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="3bc13-156">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3bc13-156">JSON representation</span></span>

<span data-ttu-id="3bc13-157">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3bc13-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ServicesUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "exchangeActive": 1024, 
  "exchangeInactive": 1024, 
  "oneDriveActive": 1024, 
  "oneDriveInactive": 1024, 
  "sharePointActive": 1024, 
  "sharePointInactive": 1024, 
  "skypeForBusinessActive": 1024, 
  "skypeForBusinessInactive": 1024, 
  "yammerActive": 1024, 
  "yammerInactive": 1024, 
  "teamsActive": 1024, 
  "teamsInactive": 1024, 
  "reportPeriod": "String"
}
```
