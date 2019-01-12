---
title: Ressourcentyp office365ActiveUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 2eaeccb1fa3b67c6b3e1d2d7c88a1dfad4e40e88
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959125"
---
# <a name="office365activeusercounts-resource-type"></a><span data-ttu-id="13914-103">Ressourcentyp office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="13914-103">office365ActiveUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="13914-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="13914-104">Properties</span></span>

| <span data-ttu-id="13914-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="13914-105">Property</span></span>          | <span data-ttu-id="13914-106">Typ</span><span class="sxs-lookup"><span data-stu-id="13914-106">Type</span></span>   | <span data-ttu-id="13914-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13914-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="13914-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="13914-108">reportRefreshDate</span></span> | <span data-ttu-id="13914-109">Datum</span><span class="sxs-lookup"><span data-stu-id="13914-109">Date</span></span>   | <span data-ttu-id="13914-110">Das aktuelle Datum des Inhalts.</span><span class="sxs-lookup"><span data-stu-id="13914-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="13914-111">Office365</span><span class="sxs-lookup"><span data-stu-id="13914-111">office365</span></span>         | <span data-ttu-id="13914-112">Int64</span><span class="sxs-lookup"><span data-stu-id="13914-112">Int64</span></span>  | <span data-ttu-id="13914-113">Die Anzahl von aktiven Benutzern in Office 365.</span><span class="sxs-lookup"><span data-stu-id="13914-113">The number of active users in Office 365.</span></span> <span data-ttu-id="13914-114">Dieser Wert schließt alle aktiven Benutzer in Exchange, OneDrive, SharePoint, Skype für Unternehmen, Yammer und Microsoft-Teams.</span><span class="sxs-lookup"><span data-stu-id="13914-114">This number includes all the active users in Exchange, OneDrive, SharePoint, Skype For Business, Yammer, and Microsoft Teams.</span></span> <span data-ttu-id="13914-115">Für jedes Produkt in der entsprechenden eigenschaftsbeschreibung finden Sie die Definition der aktiven Benutzer.</span><span class="sxs-lookup"><span data-stu-id="13914-115">You can find the definition of active user for each product in the respective property description.</span></span> |
| <span data-ttu-id="13914-116">Exchange</span><span class="sxs-lookup"><span data-stu-id="13914-116">exchange</span></span>          | <span data-ttu-id="13914-117">Int64</span><span class="sxs-lookup"><span data-stu-id="13914-117">Int64</span></span>  | <span data-ttu-id="13914-118">Die Anzahl von aktiven Benutzern in Exchange.</span><span class="sxs-lookup"><span data-stu-id="13914-118">The number of active users in Exchange.</span></span> <span data-ttu-id="13914-119">Jeder Benutzer, der lesen und e-Mail senden kann, wird einen aktiven Benutzer betrachtet.</span><span class="sxs-lookup"><span data-stu-id="13914-119">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="13914-120">oneDrive</span><span class="sxs-lookup"><span data-stu-id="13914-120">oneDrive</span></span>          | <span data-ttu-id="13914-121">Int64</span><span class="sxs-lookup"><span data-stu-id="13914-121">Int64</span></span>  | <span data-ttu-id="13914-122">Die Anzahl von aktiven Benutzern in OneDrive.</span><span class="sxs-lookup"><span data-stu-id="13914-122">The number of active users in OneDrive.</span></span> <span data-ttu-id="13914-123">Jeder Benutzer, der angezeigt oder bearbeitet Dateien, freigegebenen Dateien intern oder extern oder Dateien synchronisiert wird einen aktiven Benutzer betrachtet.</span><span class="sxs-lookup"><span data-stu-id="13914-123">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="13914-124">sharePoint</span><span class="sxs-lookup"><span data-stu-id="13914-124">sharePoint</span></span>        | <span data-ttu-id="13914-125">Int64</span><span class="sxs-lookup"><span data-stu-id="13914-125">Int64</span></span>  | <span data-ttu-id="13914-126">Die Anzahl von aktiven Benutzern in SharePoint.</span><span class="sxs-lookup"><span data-stu-id="13914-126">The number of active users in SharePoint.</span></span> <span data-ttu-id="13914-127">Jeder Benutzer, der angezeigt oder bearbeitet Dateien, gemeinsam genutzte Dateien intern oder extern, synchronisiert Dateien oder SharePoint-Seiten angezeigt wird einen aktiven Benutzer betrachtet.</span><span class="sxs-lookup"><span data-stu-id="13914-127">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="13914-128">skypeForBusiness</span><span class="sxs-lookup"><span data-stu-id="13914-128">skypeForBusiness</span></span>  | <span data-ttu-id="13914-129">Int64</span><span class="sxs-lookup"><span data-stu-id="13914-129">Int64</span></span>  | <span data-ttu-id="13914-130">Die Anzahl von aktiven Benutzern in Skype für Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="13914-130">The number of active users in Skype For Business.</span></span> <span data-ttu-id="13914-131">Jeder Benutzer, die organisiert oder in Konferenzen teilgenommen Peer-zu-Peer-Sitzungen verbunden wird einen aktiven Benutzer betrachtet.</span><span class="sxs-lookup"><span data-stu-id="13914-131">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="13914-132">Yammer</span><span class="sxs-lookup"><span data-stu-id="13914-132">yammer</span></span>            | <span data-ttu-id="13914-133">Int64</span><span class="sxs-lookup"><span data-stu-id="13914-133">Int64</span></span>  | <span data-ttu-id="13914-134">Die Anzahl von aktiven Benutzern in Yammer.</span><span class="sxs-lookup"><span data-stu-id="13914-134">The number of active users in Yammer.</span></span> <span data-ttu-id="13914-135">Jeder Benutzer kann buchen, lesen oder like Nachrichten wird einen aktiven Benutzer betrachtet.</span><span class="sxs-lookup"><span data-stu-id="13914-135">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="13914-136">Teams</span><span class="sxs-lookup"><span data-stu-id="13914-136">teams</span></span>             | <span data-ttu-id="13914-137">Int64</span><span class="sxs-lookup"><span data-stu-id="13914-137">Int64</span></span>  | <span data-ttu-id="13914-138">Die Anzahl der aktiven Benutzer in Microsoft-Teams.</span><span class="sxs-lookup"><span data-stu-id="13914-138">The number of active users in Microsoft Teams.</span></span> <span data-ttu-id="13914-139">Jeder Benutzer, die Nachrichten im Team Kanäle gebucht, gesendete Nachrichten in privaten chatten oder Besprechungen oder Anrufe beteiligt ist einen aktiven Benutzer betrachtet.</span><span class="sxs-lookup"><span data-stu-id="13914-139">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="13914-140">reportDate</span><span class="sxs-lookup"><span data-stu-id="13914-140">reportDate</span></span>        | <span data-ttu-id="13914-141">Datum</span><span class="sxs-lookup"><span data-stu-id="13914-141">Date</span></span>   | <span data-ttu-id="13914-142">Das Datum, an dem eine Anzahl von Benutzern aktiv waren.</span><span class="sxs-lookup"><span data-stu-id="13914-142">The date on which a number of users were active.</span></span> |
| <span data-ttu-id="13914-143">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="13914-143">reportPeriod</span></span>      | <span data-ttu-id="13914-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13914-144">String</span></span> | <span data-ttu-id="13914-145">Die Anzahl der Tage, die der Bericht wird behandelt.</span><span class="sxs-lookup"><span data-stu-id="13914-145">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="13914-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="13914-146">JSON representation</span></span>

<span data-ttu-id="13914-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="13914-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActiveUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "office365": 1024, 
  "exchange": 1024, 
  "oneDrive": 1024, 
  "sharePoint": 1024, 
  "skypeForBusiness": 1024, 
  "yammer": 1024, 
  "teams": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
