# <a name="location-resource-type"></a><span data-ttu-id="88df5-101">Location-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="88df5-101">Location resource type</span></span>

<span data-ttu-id="88df5-102">Stellt Standortinformationen eines [Ereignisses](event.md) dar.</span><span class="sxs-lookup"><span data-stu-id="88df5-102">Represents location information of an event.</span></span>

<span data-ttu-id="88df5-103">Es gibt mehrere Methoden zum Erstellen von Ereignissen in einem Kalender, z. B. über eine App mithilfe der REST-API [Ereignis erstellen](../api/user_post_events.md) oder manuell mithilfe der Outlook-Benutzeroberfläche.</span><span class="sxs-lookup"><span data-stu-id="88df5-103">There are multiple ways to create events in a calendar, for example, through an app using the [create event](../api/user_post_events.md) REST API, or manually using the Outlook user interface.</span></span> <span data-ttu-id="88df5-104">Wenn Sie ein Ereignis über die Benutzeroberfläche erstellen, können Sie den Ort als Nur-Text angeben (z. B. „Harrys Bar“) oder aus der in Outlook bereitgestellten Raumliste, [Bing-Vorschlagssuche](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/) oder [lokale Bing-Suche](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span><span class="sxs-lookup"><span data-stu-id="88df5-104">When you create an event using the user interface, you can specify the location as plain text (for example, "Harry's Bar"), or from the rooms list provided by Outlook, [Bing Autosuggest](https://blogs.bing.com/search/2013/02/20/a-look-at-autosuggest/), or [Bing local search](https://blogs.bing.com/search/2010/08/17/local-search-on-m-bing-com/).</span></span> 

<span data-ttu-id="88df5-105">Je nachdem, wie ein Ereignis erstellt wurde, wird die schreibgeschützte **locationType**-Eigenschaft anders festgelegt.</span><span class="sxs-lookup"><span data-stu-id="88df5-105">Depending on how an event is created, expect Outlook to set the read-only **locationType** property differently.</span></span> 

| <span data-ttu-id="88df5-106">Wie ein Ereignis erstellt wurde</span><span class="sxs-lookup"><span data-stu-id="88df5-106">How event was created</span></span>  | <span data-ttu-id="88df5-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="88df5-107">Property</span></span>   | <span data-ttu-id="88df5-108">Erwarteter Wert</span><span class="sxs-lookup"><span data-stu-id="88df5-108">Expected value</span></span> |
|:----------|:-------|:--------------------------------|
| <span data-ttu-id="88df5-109">REST-API [Ereignis erstellen](../api/user_post_events.md) </span><span class="sxs-lookup"><span data-stu-id="88df5-109">[create event](../api/user_post_events.md) REST API</span></span> | <span data-ttu-id="88df5-110">**locationType**</span><span class="sxs-lookup"><span data-stu-id="88df5-110">**locationType**</span></span> | `default` |
| <span data-ttu-id="88df5-111">Benutzeroberfläche in Outlook</span><span class="sxs-lookup"><span data-stu-id="88df5-111">User interface in Outlook</span></span> | <span data-ttu-id="88df5-112">**locationType**</span><span class="sxs-lookup"><span data-stu-id="88df5-112">**locationType**</span></span> | <span data-ttu-id="88df5-113">Eine der folgenden Varianten:</span><span class="sxs-lookup"><span data-stu-id="88df5-113">One of the following:</span></span> <ul><li><span data-ttu-id="88df5-114">`default` für einen Ort, der als Nur-Text eingegeben wird.</span><span class="sxs-lookup"><span data-stu-id="88df5-114">`default` for a location entered as plain text.</span></span></li><li><span data-ttu-id="88df5-115">`conferenceRoom` für einen Raum, der von der Outlook-Raumliste bereitgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="88df5-115">`conferenceRoom` for a room provided by the Outlook rooms list.</span></span></li><li><span data-ttu-id="88df5-116">Oder eine der folgenden Listen – `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` – für einen Ort aus der Bing-Vorschlagssuche oder der lokalen Bing-Suche.</span><span class="sxs-lookup"><span data-stu-id="88df5-116">Or, any of this list - `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress` - for a location from Bing Autosuggest or Bing local search.</span></span></li></ul> |

## <a name="properties"></a><span data-ttu-id="88df5-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="88df5-117">Properties</span></span>
| <span data-ttu-id="88df5-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="88df5-118">Property</span></span>  | <span data-ttu-id="88df5-119">Typ</span><span class="sxs-lookup"><span data-stu-id="88df5-119">Type</span></span>   | <span data-ttu-id="88df5-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88df5-120">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="88df5-121">address</span><span class="sxs-lookup"><span data-stu-id="88df5-121">address</span></span> | [<span data-ttu-id="88df5-122">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="88df5-122">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="88df5-123">Die Adresse des Orts.</span><span class="sxs-lookup"><span data-stu-id="88df5-123">The street address of the location.</span></span> |
| <span data-ttu-id="88df5-124">Koordinaten</span><span class="sxs-lookup"><span data-stu-id="88df5-124">Coordinates</span></span> | [<span data-ttu-id="88df5-125">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="88df5-125">outlookGeoCoordinates</span></span>](outlookGeoCoordinates.md) | <span data-ttu-id="88df5-126">Die geografischen Koordinaten und die Erhebung des Orts.</span><span class="sxs-lookup"><span data-stu-id="88df5-126">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="88df5-127">displayName</span><span class="sxs-lookup"><span data-stu-id="88df5-127">displayName</span></span>  | <span data-ttu-id="88df5-128">String</span><span class="sxs-lookup"><span data-stu-id="88df5-128">String</span></span> | <span data-ttu-id="88df5-129">Der Name, der mit dem Ort verknüpft ist</span><span class="sxs-lookup"><span data-stu-id="88df5-129">The name associated with the location.</span></span>                       |
| <span data-ttu-id="88df5-130">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="88df5-130">locationEmailAddress</span></span> | <span data-ttu-id="88df5-131">String</span><span class="sxs-lookup"><span data-stu-id="88df5-131">String</span></span> | <span data-ttu-id="88df5-132">Optionale E-Mail-Adresse des Orts.</span><span class="sxs-lookup"><span data-stu-id="88df5-132">Optional email address of the location.</span></span>              |
| <span data-ttu-id="88df5-133">locationUri</span><span class="sxs-lookup"><span data-stu-id="88df5-133">locationUri</span></span> | <span data-ttu-id="88df5-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="88df5-134">String</span></span> | <span data-ttu-id="88df5-135">Optionaler URI, der den Ort darstellt.</span><span class="sxs-lookup"><span data-stu-id="88df5-135">Optional URI representing the location.</span></span> |
| <span data-ttu-id="88df5-136">locationType</span><span class="sxs-lookup"><span data-stu-id="88df5-136">locationType</span></span> | <span data-ttu-id="88df5-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="88df5-137">String</span></span> | <span data-ttu-id="88df5-138">Der Typ des Orts.</span><span class="sxs-lookup"><span data-stu-id="88df5-138">The type of the location to go to. Required.</span></span> <span data-ttu-id="88df5-139">Mögliche Werte sind: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`,`geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.</span><span class="sxs-lookup"><span data-stu-id="88df5-139">Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`, `geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`.</span></span> <span data-ttu-id="88df5-140">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="88df5-140">Read-only.</span></span>|
| <span data-ttu-id="88df5-141">uniqueId</span><span class="sxs-lookup"><span data-stu-id="88df5-141">UniqueId</span></span> | <span data-ttu-id="88df5-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="88df5-142">String</span></span> | <span data-ttu-id="88df5-143">Nur für internen Gebrauch.</span><span class="sxs-lookup"><span data-stu-id="88df5-143">For internal use only.</span></span>|
| <span data-ttu-id="88df5-144">uniqueIdType</span><span class="sxs-lookup"><span data-stu-id="88df5-144">uniqueIdType</span></span> | <span data-ttu-id="88df5-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="88df5-145">String</span></span> | <span data-ttu-id="88df5-146">Nur für internen Gebrauch.</span><span class="sxs-lookup"><span data-stu-id="88df5-146">For internal use only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="88df5-147">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="88df5-147">JSON representation</span></span>

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
