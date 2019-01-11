---
title: Location-Ressourcentyp
description: Stellt Standortinformationen eines Ereignisses dar.
localization_priority: Normal
ms.openlocfilehash: 650876596e2cf9336054957cfd4c95bf4dad16b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879401"
---
# <a name="location-resource-type"></a><span data-ttu-id="d4748-103">Location-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d4748-103">Location resource type</span></span>

> <span data-ttu-id="d4748-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d4748-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4748-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d4748-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d4748-106">Stellt Standortinformationen eines [Ereignisses](event.md) dar.</span><span class="sxs-lookup"><span data-stu-id="d4748-106">Represents location information of an [event](event.md).</span></span>

<span data-ttu-id="d4748-107">Es gibt mehrere Methoden zum Erstellen von Ereignissen in einem Kalender, z. B. über eine App mithilfe der REST-API [Ereignis erstellen](../api/user-post-events.md) oder manuell mithilfe der Outlook-Benutzeroberfläche.</span><span class="sxs-lookup"><span data-stu-id="d4748-107">There are multiple ways to create events in a calendar, for example, through an app using the [create event](../api/user-post-events.md) REST API, or manually using the Outlook user interface.</span></span> <span data-ttu-id="d4748-108">Wenn Sie ein Ereignis über die Benutzeroberfläche erstellen, können Sie den Ort als Nur-Text angeben (z. B. „Harrys Bar“) oder aus der in Outlook bereitgestellten Raumliste, [Bing-Vorschlagssuche](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/) oder [lokale Bing-Suche](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span><span class="sxs-lookup"><span data-stu-id="d4748-108">When you create an event using the user interface, you can specify the location as plain text (for example, "Harry's Bar"), or from the rooms list provided by Outlook, [Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/), or [Bing local search](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span></span> 

<span data-ttu-id="d4748-109">Je nachdem, wie ein Ereignis erstellt wurde, wird die schreibgeschützte **locationType**-Eigenschaft anders festgelegt.</span><span class="sxs-lookup"><span data-stu-id="d4748-109">Depending on how an event is created, expect Outlook to set the read-only **locationType** property differently.</span></span> 

| <span data-ttu-id="d4748-110">Wie ein Ereignis erstellt wurde</span><span class="sxs-lookup"><span data-stu-id="d4748-110">How event was created</span></span>  | <span data-ttu-id="d4748-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d4748-111">Property</span></span>   | <span data-ttu-id="d4748-112">Erwarteter Wert</span><span class="sxs-lookup"><span data-stu-id="d4748-112">Expected value</span></span> |
|:----------|:-------|:--------------------------------|
| <span data-ttu-id="d4748-113">REST-API [Ereignis erstellen](../api/user-post-events.md) </span><span class="sxs-lookup"><span data-stu-id="d4748-113">[create event](../api/user-post-events.md) REST API</span></span> | <span data-ttu-id="d4748-114">**locationType**</span><span class="sxs-lookup"><span data-stu-id="d4748-114">**locationType**</span></span> | `default` |
| <span data-ttu-id="d4748-115">Benutzeroberfläche in Outlook</span><span class="sxs-lookup"><span data-stu-id="d4748-115">User interface in Outlook</span></span> | <span data-ttu-id="d4748-116">**locationType**</span><span class="sxs-lookup"><span data-stu-id="d4748-116">**locationType**</span></span> | <span data-ttu-id="d4748-117">Eine der folgenden Varianten:</span><span class="sxs-lookup"><span data-stu-id="d4748-117">One of the following:</span></span> <ul><li><span data-ttu-id="d4748-118">`default` für einen Ort, der als Nur-Text eingegeben wird.</span><span class="sxs-lookup"><span data-stu-id="d4748-118">`default` for a location entered as plain text.</span></span></li><li><span data-ttu-id="d4748-119">`conferenceRoom` für einen Raum, der von der Outlook-Raumliste bereitgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="d4748-119">`conferenceRoom` for a room provided by the Outlook rooms list.</span></span></li><li><span data-ttu-id="d4748-120">Oder eine der folgenden Listen – `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` – für einen Ort aus der Bing-Vorschlagssuche oder der lokalen Bing-Suche.</span><span class="sxs-lookup"><span data-stu-id="d4748-120">Or, any of this list - `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` - for a location from Bing Autosuggest or Bing local search.</span></span></li></ul> |




## <a name="properties"></a><span data-ttu-id="d4748-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d4748-121">Properties</span></span>
| <span data-ttu-id="d4748-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d4748-122">Property</span></span>  | <span data-ttu-id="d4748-123">Typ</span><span class="sxs-lookup"><span data-stu-id="d4748-123">Type</span></span>   | <span data-ttu-id="d4748-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4748-124">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="d4748-125">address</span><span class="sxs-lookup"><span data-stu-id="d4748-125">address</span></span> | [<span data-ttu-id="d4748-126">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="d4748-126">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="d4748-127">Die Adresse des Orts.</span><span class="sxs-lookup"><span data-stu-id="d4748-127">The street address of the location.</span></span> |
| <span data-ttu-id="d4748-128">Koordinaten</span><span class="sxs-lookup"><span data-stu-id="d4748-128">coordinates</span></span> | [<span data-ttu-id="d4748-129">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="d4748-129">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="d4748-130">Die geografischen Koordinaten und die Erhebung des Orts.</span><span class="sxs-lookup"><span data-stu-id="d4748-130">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="d4748-131">displayName</span><span class="sxs-lookup"><span data-stu-id="d4748-131">displayName</span></span>  | <span data-ttu-id="d4748-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4748-132">String</span></span> | <span data-ttu-id="d4748-133">Der Name, der mit dem Ort verknüpft ist</span><span class="sxs-lookup"><span data-stu-id="d4748-133">The name associated with the location.</span></span>                       |
| <span data-ttu-id="d4748-134">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="d4748-134">locationEmailAddress</span></span> | <span data-ttu-id="d4748-135">String</span><span class="sxs-lookup"><span data-stu-id="d4748-135">String</span></span> | <span data-ttu-id="d4748-136">Optionale E-Mail-Adresse des Orts.</span><span class="sxs-lookup"><span data-stu-id="d4748-136">Optional email address of the location.</span></span> |
| <span data-ttu-id="d4748-137">locationUri</span><span class="sxs-lookup"><span data-stu-id="d4748-137">locationUri</span></span> | <span data-ttu-id="d4748-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4748-138">String</span></span> | <span data-ttu-id="d4748-139">Optionaler URI, der den Ort darstellt.</span><span class="sxs-lookup"><span data-stu-id="d4748-139">Optional URI representing the location.</span></span> |
| <span data-ttu-id="d4748-140">locationType</span><span class="sxs-lookup"><span data-stu-id="d4748-140">locationType</span></span> | <span data-ttu-id="d4748-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4748-141">String</span></span> | <span data-ttu-id="d4748-142">Der Typ des Orts.</span><span class="sxs-lookup"><span data-stu-id="d4748-142">The type of location.</span></span> <span data-ttu-id="d4748-143">Mögliche Werte sind: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span><span class="sxs-lookup"><span data-stu-id="d4748-143">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="d4748-144">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d4748-144">Read-only.</span></span>|
| <span data-ttu-id="d4748-145">uniqueId</span><span class="sxs-lookup"><span data-stu-id="d4748-145">uniqueId</span></span> | <span data-ttu-id="d4748-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4748-146">String</span></span> | <span data-ttu-id="d4748-147">Nur für internen Gebrauch.</span><span class="sxs-lookup"><span data-stu-id="d4748-147">For internal use only.</span></span>|
| <span data-ttu-id="d4748-148">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="d4748-148">uniqueIdType</span></span> | <span data-ttu-id="d4748-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4748-149">String</span></span> | <span data-ttu-id="d4748-150">Nur für internen Gebrauch.</span><span class="sxs-lookup"><span data-stu-id="d4748-150">For internal use only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="d4748-151">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d4748-151">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.location"
}-->
```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "coordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "displayName": "string",
  "locationEmailAddress": "string",
  "locationUri": "string",
  "locationType": "string",
  "uniqueId": "string",
  "uniqueIdType": "string"
}

```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
