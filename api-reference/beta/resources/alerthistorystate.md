---
title: alertHistoryState-Ressourcentyp
description: Jedes Mal, wenn eine Warnung gepatcht wird, wird die Änderung in einem neuen alertHistoryState-Objekt gespeichert und als Teil der geänderten Warnung zurückgegeben.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: a5dda54101264ee2ec4d01a283f96a93f1d6e5e3
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366966"
---
# <a name="alerthistorystate-resource-type"></a><span data-ttu-id="b4c34-103">alertHistoryState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b4c34-103">alertHistoryState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4c34-104">Jedes Mal, wenn eine Warnung gepatcht wird, wird die Änderung in einem neuen alertHistoryState-Objekt gespeichert und als Teil der geänderten Warnung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b4c34-104">Each time an alert is patched, the change is saved in a new object of alertHistoryState, and will be returned as part of the modified alert.</span></span>

## <a name="properties"></a><span data-ttu-id="b4c34-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b4c34-105">Properties</span></span>

| <span data-ttu-id="b4c34-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b4c34-106">Property</span></span>     | <span data-ttu-id="b4c34-107">Typ</span><span class="sxs-lookup"><span data-stu-id="b4c34-107">Type</span></span>        | <span data-ttu-id="b4c34-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4c34-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b4c34-109">appId</span><span class="sxs-lookup"><span data-stu-id="b4c34-109">appId</span></span>|<span data-ttu-id="b4c34-110">String</span><span class="sxs-lookup"><span data-stu-id="b4c34-110">String</span></span>| <span data-ttu-id="b4c34-111">Die Anwendungs-ID der aufrufenden Anwendung, die ein Update (PATCH) an die Warnung übermittelt hat.</span><span class="sxs-lookup"><span data-stu-id="b4c34-111">The Application ID of the calling application that submitted an update (PATCH) to the alert.</span></span> <span data-ttu-id="b4c34-112">Die Anwendungs-ID sollte aus dem auth-Token extrahiert und nicht manuell von der aufrufenden Anwendung eingegeben werden.</span><span class="sxs-lookup"><span data-stu-id="b4c34-112">The appId should be extracted from the auth token and not entered manually by the calling application.</span></span> |
|<span data-ttu-id="b4c34-113">assignedTo</span><span class="sxs-lookup"><span data-stu-id="b4c34-113">assignedTo</span></span>|<span data-ttu-id="b4c34-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4c34-114">String</span></span>| <span data-ttu-id="b4c34-115">UPN des Benutzers, dem die Warnung zugewiesen wurde (Hinweis: Alert. ZugewiesenAn speichert nur den letzten Wert/UPN).</span><span class="sxs-lookup"><span data-stu-id="b4c34-115">UPN of user the alert was assigned to (note: alert.assignedTo only stores the last value/UPN).</span></span> |
|<span data-ttu-id="b4c34-116">comments</span><span class="sxs-lookup"><span data-stu-id="b4c34-116">comments</span></span>|<span data-ttu-id="b4c34-117">String collection</span><span class="sxs-lookup"><span data-stu-id="b4c34-117">String collection</span></span>|<span data-ttu-id="b4c34-118">Vom angemeldeten Benutzer eingegebene Kommentar.</span><span class="sxs-lookup"><span data-stu-id="b4c34-118">Comment entered by signed-in user.</span></span>|
|<span data-ttu-id="b4c34-119">Feedback</span><span class="sxs-lookup"><span data-stu-id="b4c34-119">feedback</span></span>|<span data-ttu-id="b4c34-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4c34-120">String</span></span>| <span data-ttu-id="b4c34-121">Analysten Feedback zu der Warnung in diesem Update.</span><span class="sxs-lookup"><span data-stu-id="b4c34-121">Analyst feedback on the alert in this update.</span></span> <span data-ttu-id="b4c34-122">Mögliche Werte: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span><span class="sxs-lookup"><span data-stu-id="b4c34-122">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="b4c34-123">status</span><span class="sxs-lookup"><span data-stu-id="b4c34-123">status</span></span>|<span data-ttu-id="b4c34-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4c34-124">String</span></span>| <span data-ttu-id="b4c34-125">Warnungsstatus Wert (falls aktualisiert).</span><span class="sxs-lookup"><span data-stu-id="b4c34-125">Alert status value (if updated).</span></span> <span data-ttu-id="b4c34-126">Mögliche Werte: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.</span><span class="sxs-lookup"><span data-stu-id="b4c34-126">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.</span></span>|
|<span data-ttu-id="b4c34-127">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4c34-127">updatedDateTime</span></span>|<span data-ttu-id="b4c34-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4c34-128">DateTimeOffset</span></span>| <span data-ttu-id="b4c34-129">Datum und Uhrzeit des Warnungs Updates.</span><span class="sxs-lookup"><span data-stu-id="b4c34-129">Date and time of the alert update.</span></span> <span data-ttu-id="b4c34-130">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="b4c34-130">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b4c34-131">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b4c34-131">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b4c34-132">user</span><span class="sxs-lookup"><span data-stu-id="b4c34-132">user</span></span>|<span data-ttu-id="b4c34-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4c34-133">String</span></span>| <span data-ttu-id="b4c34-134">UPN des angemeldeten Benutzers, der die Warnung aktualisiert hat (entnommen vom Bearer-Token, falls im Benutzer/Delegierten Authentifizierungsmodus).</span><span class="sxs-lookup"><span data-stu-id="b4c34-134">UPN of the signed-in user that updated the alert (taken from the bearer token - if in user/delegated auth mode).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b4c34-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b4c34-135">JSON representation</span></span>

<span data-ttu-id="b4c34-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b4c34-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertHistoryState",
  "baseType": null
}-->

```json
{
  "appId": "String",
  "assignedTo": "String",
  "comments": ["String"],
  "feedback": "String",
  "status": "String",
  "updatedDateTime": "String (timestamp)",
  "user": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertHistoryState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->