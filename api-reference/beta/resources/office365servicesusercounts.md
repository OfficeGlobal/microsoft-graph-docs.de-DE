---
title: Ressourcentyp office365ServicesUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 36fd043be3cef36951f7651d625f4a93d3b5f8cc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573893"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="12f9f-103">Ressourcentyp office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="12f9f-103">office365ServicesUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="12f9f-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="12f9f-104">Properties</span></span>

| <span data-ttu-id="12f9f-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="12f9f-105">Property</span></span>                 | <span data-ttu-id="12f9f-106">Typ</span><span class="sxs-lookup"><span data-stu-id="12f9f-106">Type</span></span>   | <span data-ttu-id="12f9f-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="12f9f-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="12f9f-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="12f9f-108">reportRefreshDate</span></span>        | <span data-ttu-id="12f9f-109">Date</span><span class="sxs-lookup"><span data-stu-id="12f9f-109">Date</span></span>   | <span data-ttu-id="12f9f-110">Das aktuelle Datum des Inhalts.</span><span class="sxs-lookup"><span data-stu-id="12f9f-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="12f9f-111">exchangeActive</span><span class="sxs-lookup"><span data-stu-id="12f9f-111">exchangeActive</span></span>           | <span data-ttu-id="12f9f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="12f9f-112">Int64</span></span>  | <span data-ttu-id="12f9f-113">Die Anzahl von aktiven Benutzern auf Exchange.</span><span class="sxs-lookup"><span data-stu-id="12f9f-113">The number of active users on Exchange.</span></span> <span data-ttu-id="12f9f-114">Jeder Benutzer, der lesen und e-Mail senden kann, wird einen aktiven Benutzer betrachtet.</span><span class="sxs-lookup"><span data-stu-id="12f9f-114">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="12f9f-115">exchangeInactive</span><span class="sxs-lookup"><span data-stu-id="12f9f-115">exchangeInactive</span></span>         | <span data-ttu-id="12f9f-116">Int64</span><span class="sxs-lookup"><span data-stu-id="12f9f-116">Int64</span></span>  | <span data-ttu-id="12f9f-117">Die Anzahl der inaktive Benutzer auf Exchange.</span><span class="sxs-lookup"><span data-stu-id="12f9f-117">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="12f9f-118">oneDriveActive</span><span class="sxs-lookup"><span data-stu-id="12f9f-118">oneDriveActive</span></span>           | <span data-ttu-id="12f9f-119">Int64</span><span class="sxs-lookup"><span data-stu-id="12f9f-119">Int64</span></span>  | <span data-ttu-id="12f9f-120">Die Anzahl von aktiven Benutzern in OneDrive.</span><span class="sxs-lookup"><span data-stu-id="12f9f-120">The number of active users on OneDrive.</span></span> <span data-ttu-id="12f9f-121">Jeder Benutzer, der angezeigt oder bearbeitet Dateien, freigegebenen Dateien intern oder extern oder Dateien synchronisiert wird einen aktiven Benutzer betrachtet.</span><span class="sxs-lookup"><span data-stu-id="12f9f-121">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="12f9f-122">oneDriveInactive</span><span class="sxs-lookup"><span data-stu-id="12f9f-122">oneDriveInactive</span></span>         | <span data-ttu-id="12f9f-123">Int64</span><span class="sxs-lookup"><span data-stu-id="12f9f-123">Int64</span></span>  | <span data-ttu-id="12f9f-124">Die Anzahl der inaktive Benutzer in OneDrive.</span><span class="sxs-lookup"><span data-stu-id="12f9f-124">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="12f9f-125">sharePointActive</span><span class="sxs-lookup"><span data-stu-id="12f9f-125">sharePointActive</span></span>         | <span data-ttu-id="12f9f-126">Int64</span><span class="sxs-lookup"><span data-stu-id="12f9f-126">Int64</span></span>  | <span data-ttu-id="12f9f-127">Die Anzahl der aktive Benutzer in SharePoint.</span><span class="sxs-lookup"><span data-stu-id="12f9f-127">The number of active users on SharePoint.</span></span> <span data-ttu-id="12f9f-128">Jeder Benutzer, der angezeigt oder bearbeitet Dateien, gemeinsam genutzte Dateien intern oder extern, synchronisiert Dateien oder SharePoint-Seiten angezeigt wird einen aktiven Benutzer betrachtet.</span><span class="sxs-lookup"><span data-stu-id="12f9f-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="12f9f-129">sharePointInactive</span><span class="sxs-lookup"><span data-stu-id="12f9f-129">sharePointInactive</span></span>       | <span data-ttu-id="12f9f-130">Int64</span><span class="sxs-lookup"><span data-stu-id="12f9f-130">Int64</span></span>  | <span data-ttu-id="12f9f-131">Die Anzahl der inaktive Benutzer auf SharePoint.</span><span class="sxs-lookup"><span data-stu-id="12f9f-131">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="12f9f-132">skypeForBusinessActive</span><span class="sxs-lookup"><span data-stu-id="12f9f-132">skypeForBusinessActive</span></span>   | <span data-ttu-id="12f9f-133">Int64</span><span class="sxs-lookup"><span data-stu-id="12f9f-133">Int64</span></span>  | <span data-ttu-id="12f9f-134">Die Anzahl von aktiven Benutzern auf Skype für Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="12f9f-134">The number of active users on Skype For Business.</span></span> <span data-ttu-id="12f9f-135">Jeder Benutzer, die organisiert oder in Konferenzen teilgenommen Peer-zu-Peer-Sitzungen verbunden wird einen aktiven Benutzer betrachtet.</span><span class="sxs-lookup"><span data-stu-id="12f9f-135">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="12f9f-136">skypeForBusinessInactive</span><span class="sxs-lookup"><span data-stu-id="12f9f-136">skypeForBusinessInactive</span></span> | <span data-ttu-id="12f9f-137">Int64</span><span class="sxs-lookup"><span data-stu-id="12f9f-137">Int64</span></span>  | <span data-ttu-id="12f9f-138">Die Anzahl der inaktive Benutzer auf Skype für Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="12f9f-138">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="12f9f-139">yammerActive</span><span class="sxs-lookup"><span data-stu-id="12f9f-139">yammerActive</span></span>             | <span data-ttu-id="12f9f-140">Int64</span><span class="sxs-lookup"><span data-stu-id="12f9f-140">Int64</span></span>  | <span data-ttu-id="12f9f-141">Die Anzahl der aktive Benutzer in Yammer.</span><span class="sxs-lookup"><span data-stu-id="12f9f-141">The number of active users on Yammer.</span></span> <span data-ttu-id="12f9f-142">Jeder Benutzer kann buchen, lesen oder like Nachrichten wird einen aktiven Benutzer betrachtet.</span><span class="sxs-lookup"><span data-stu-id="12f9f-142">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="12f9f-143">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="12f9f-143">yammerInactive</span></span>           | <span data-ttu-id="12f9f-144">Int64</span><span class="sxs-lookup"><span data-stu-id="12f9f-144">Int64</span></span>  | <span data-ttu-id="12f9f-145">Die Anzahl der inaktive Benutzer auf Yammer.</span><span class="sxs-lookup"><span data-stu-id="12f9f-145">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="12f9f-146">teamsActive</span><span class="sxs-lookup"><span data-stu-id="12f9f-146">teamsActive</span></span>              | <span data-ttu-id="12f9f-147">Int64</span><span class="sxs-lookup"><span data-stu-id="12f9f-147">Int64</span></span>  | <span data-ttu-id="12f9f-148">Die Anzahl der aktive Benutzer in Microsoft-Teams.</span><span class="sxs-lookup"><span data-stu-id="12f9f-148">The number of active users on Microsoft Teams.</span></span> <span data-ttu-id="12f9f-149">Jeder Benutzer, die Nachrichten im Team Kanäle gebucht, gesendete Nachrichten in privaten chatten oder Besprechungen oder Anrufe beteiligt ist einen aktiven Benutzer betrachtet.</span><span class="sxs-lookup"><span data-stu-id="12f9f-149">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="12f9f-150">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="12f9f-150">teamsInactive</span></span>            | <span data-ttu-id="12f9f-151">Int64</span><span class="sxs-lookup"><span data-stu-id="12f9f-151">Int64</span></span>  | <span data-ttu-id="12f9f-152">Die Anzahl der inaktive Benutzer in Microsoft-Teams.</span><span class="sxs-lookup"><span data-stu-id="12f9f-152">The number of inactive users on Microsoft Teams.</span></span>     |
| <span data-ttu-id="12f9f-153">office365Active</span><span class="sxs-lookup"><span data-stu-id="12f9f-153">office365Active</span></span>          | <span data-ttu-id="12f9f-154">Int64</span><span class="sxs-lookup"><span data-stu-id="12f9f-154">Int64</span></span>  | <span data-ttu-id="12f9f-155">Die Anzahl von aktiven Benutzern in Office 365.</span><span class="sxs-lookup"><span data-stu-id="12f9f-155">The number of active users on Office 365.</span></span>   |
| <span data-ttu-id="12f9f-156">office365Inactive</span><span class="sxs-lookup"><span data-stu-id="12f9f-156">office365Inactive</span></span>        | <span data-ttu-id="12f9f-157">Int64</span><span class="sxs-lookup"><span data-stu-id="12f9f-157">Int64</span></span>  | <span data-ttu-id="12f9f-158">Die Anzahl der inaktive Benutzer in Office 365.</span><span class="sxs-lookup"><span data-stu-id="12f9f-158">The number of inactive users on Office 365.</span></span>     |
| <span data-ttu-id="12f9f-159">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="12f9f-159">reportPeriod</span></span>             | <span data-ttu-id="12f9f-160">String</span><span class="sxs-lookup"><span data-stu-id="12f9f-160">String</span></span> | <span data-ttu-id="12f9f-161">Die Anzahl der Tage, die der Bericht wird behandelt.</span><span class="sxs-lookup"><span data-stu-id="12f9f-161">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="12f9f-162">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="12f9f-162">JSON representation</span></span>

<span data-ttu-id="12f9f-163">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="12f9f-163">The following is a JSON representation of the resource.</span></span>

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
  "office365Active": 1024,
  "office365Inactive": 1024,
  "reportPeriod": "String"
}
```
