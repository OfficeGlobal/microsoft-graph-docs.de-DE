---
title: Location-Ressourcentyp
description: Stellt Standortinformationen eines Ereignisses dar.
localization_priority: Normal
ms.openlocfilehash: 6e3c61bcf8f22a20bf41053c2310dc51f5b800a7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508608"
---
# <a name="location-resource-type"></a><span data-ttu-id="5d863-103">Location-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5d863-103">Location resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d863-104">Stellt Standortinformationen eines [Ereignisses](event.md) dar.</span><span class="sxs-lookup"><span data-stu-id="5d863-104">Represents location information of an [event](event.md).</span></span>

<span data-ttu-id="5d863-105">Es gibt mehrere Methoden zum Erstellen von Ereignissen in einem Kalender, z. B. über eine App mithilfe der REST-API [Ereignis erstellen](../api/user-post-events.md) oder manuell mithilfe der Outlook-Benutzeroberfläche.</span><span class="sxs-lookup"><span data-stu-id="5d863-105">There are multiple ways to create events in a calendar, for example, through an app using the [create event](../api/user-post-events.md) REST API, or manually using the Outlook user interface.</span></span> <span data-ttu-id="5d863-106">Wenn Sie ein Ereignis über die Benutzeroberfläche erstellen, können Sie den Ort als Nur-Text angeben (z. B. „Harrys Bar“) oder aus der in Outlook bereitgestellten Raumliste, [Bing-Vorschlagssuche](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/) oder [lokale Bing-Suche](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span><span class="sxs-lookup"><span data-stu-id="5d863-106">When you create an event using the user interface, you can specify the location as plain text (for example, "Harry's Bar"), or from the rooms list provided by Outlook, [Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/), or [Bing local search](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span></span> 

<span data-ttu-id="5d863-107">Je nachdem, wie ein Ereignis erstellt wurde, wird die schreibgeschützte **locationType**-Eigenschaft anders festgelegt.</span><span class="sxs-lookup"><span data-stu-id="5d863-107">Depending on how an event is created, expect Outlook to set the read-only **locationType** property differently.</span></span> 

| <span data-ttu-id="5d863-108">Wie ein Ereignis erstellt wurde</span><span class="sxs-lookup"><span data-stu-id="5d863-108">How event was created</span></span>  | <span data-ttu-id="5d863-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5d863-109">Property</span></span>   | <span data-ttu-id="5d863-110">Erwarteter Wert</span><span class="sxs-lookup"><span data-stu-id="5d863-110">Expected value</span></span> |
|:----------|:-------|:--------------------------------|
| <span data-ttu-id="5d863-111">REST-API [Ereignis erstellen](../api/user-post-events.md) </span><span class="sxs-lookup"><span data-stu-id="5d863-111">[create event](../api/user-post-events.md) REST API</span></span> | <span data-ttu-id="5d863-112">**locationType**</span><span class="sxs-lookup"><span data-stu-id="5d863-112">**locationType**</span></span> | `default` |
| <span data-ttu-id="5d863-113">Benutzeroberfläche in Outlook</span><span class="sxs-lookup"><span data-stu-id="5d863-113">User interface in Outlook</span></span> | <span data-ttu-id="5d863-114">**locationType**</span><span class="sxs-lookup"><span data-stu-id="5d863-114">**locationType**</span></span> | <span data-ttu-id="5d863-115">Eine der folgenden Varianten:</span><span class="sxs-lookup"><span data-stu-id="5d863-115">One of the following:</span></span> <ul><li><span data-ttu-id="5d863-116">`default` für einen Ort, der als Nur-Text eingegeben wird.</span><span class="sxs-lookup"><span data-stu-id="5d863-116">`default` for a location entered as plain text.</span></span></li><li><span data-ttu-id="5d863-117">`conferenceRoom` für einen Raum, der von der Outlook-Raumliste bereitgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="5d863-117">`conferenceRoom` for a room provided by the Outlook rooms list.</span></span></li><li><span data-ttu-id="5d863-118">Oder eine der folgenden Listen – `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` – für einen Ort aus der Bing-Vorschlagssuche oder der lokalen Bing-Suche.</span><span class="sxs-lookup"><span data-stu-id="5d863-118">Or, any of this list - `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` - for a location from Bing Autosuggest or Bing local search.</span></span></li></ul> |




## <a name="properties"></a><span data-ttu-id="5d863-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5d863-119">Properties</span></span>
| <span data-ttu-id="5d863-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5d863-120">Property</span></span>  | <span data-ttu-id="5d863-121">Typ</span><span class="sxs-lookup"><span data-stu-id="5d863-121">Type</span></span>   | <span data-ttu-id="5d863-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d863-122">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="5d863-123">address</span><span class="sxs-lookup"><span data-stu-id="5d863-123">address</span></span> | [<span data-ttu-id="5d863-124">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="5d863-124">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="5d863-125">Die Adresse des Orts.</span><span class="sxs-lookup"><span data-stu-id="5d863-125">The street address of the location.</span></span> |
| <span data-ttu-id="5d863-126">Koordinaten</span><span class="sxs-lookup"><span data-stu-id="5d863-126">coordinates</span></span> | [<span data-ttu-id="5d863-127">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="5d863-127">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="5d863-128">Die geografischen Koordinaten und die Erhebung des Orts.</span><span class="sxs-lookup"><span data-stu-id="5d863-128">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="5d863-129">displayName</span><span class="sxs-lookup"><span data-stu-id="5d863-129">displayName</span></span>  | <span data-ttu-id="5d863-130">String</span><span class="sxs-lookup"><span data-stu-id="5d863-130">String</span></span> | <span data-ttu-id="5d863-131">Der Name, der mit dem Ort verknüpft ist</span><span class="sxs-lookup"><span data-stu-id="5d863-131">The name associated with the location.</span></span>                       |
| <span data-ttu-id="5d863-132">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="5d863-132">locationEmailAddress</span></span> | <span data-ttu-id="5d863-133">String</span><span class="sxs-lookup"><span data-stu-id="5d863-133">String</span></span> | <span data-ttu-id="5d863-134">Optionale E-Mail-Adresse des Orts.</span><span class="sxs-lookup"><span data-stu-id="5d863-134">Optional email address of the location.</span></span> |
| <span data-ttu-id="5d863-135">locationUri</span><span class="sxs-lookup"><span data-stu-id="5d863-135">locationUri</span></span> | <span data-ttu-id="5d863-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5d863-136">String</span></span> | <span data-ttu-id="5d863-137">Optionaler URI, der den Ort darstellt.</span><span class="sxs-lookup"><span data-stu-id="5d863-137">Optional URI representing the location.</span></span> |
| <span data-ttu-id="5d863-138">locationType</span><span class="sxs-lookup"><span data-stu-id="5d863-138">locationType</span></span> | <span data-ttu-id="5d863-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5d863-139">String</span></span> | <span data-ttu-id="5d863-140">Der Typ des Orts.</span><span class="sxs-lookup"><span data-stu-id="5d863-140">The type of location.</span></span> <span data-ttu-id="5d863-141">Mögliche Werte sind: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span><span class="sxs-lookup"><span data-stu-id="5d863-141">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span></span> <span data-ttu-id="5d863-142">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5d863-142">Read-only.</span></span>|
| <span data-ttu-id="5d863-143">uniqueId</span><span class="sxs-lookup"><span data-stu-id="5d863-143">uniqueId</span></span> | <span data-ttu-id="5d863-144">String</span><span class="sxs-lookup"><span data-stu-id="5d863-144">String</span></span> | <span data-ttu-id="5d863-145">Nur für internen Gebrauch.</span><span class="sxs-lookup"><span data-stu-id="5d863-145">For internal use only.</span></span>|
| <span data-ttu-id="5d863-146">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="5d863-146">uniqueIdType</span></span> | <span data-ttu-id="5d863-147">String</span><span class="sxs-lookup"><span data-stu-id="5d863-147">String</span></span> | <span data-ttu-id="5d863-148">Nur für internen Gebrauch.</span><span class="sxs-lookup"><span data-stu-id="5d863-148">For internal use only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="5d863-149">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5d863-149">JSON representation</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/location.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
