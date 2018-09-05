# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="64bb4-101">Ressourcentyp onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="64bb4-101">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="64bb4-102">Die Eigenschaft **onPremisesExtensionAttribute** der [Benutzer](user.md)-Entität enthält fünfzehn benutzerdefinierte Erweiterungsattributseigenschaften.</span><span class="sxs-lookup"><span data-stu-id="64bb4-102">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="64bb4-103">Für einen **onPremisesSyncEnabled**-Benutzer wird diese Eigenschaftengruppe auf dem lokalen Active Directory gemastert und mit Azure AD synchronisiert. Sie ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="64bb4-103">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="64bb4-104">Für einen Nur-Cloud-Benutzer (wobei **onPremisesSyncEnabled** falsch ist) können diese Eigenschaften während der Erstellung oder der Aktualisierung festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="64bb4-104">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="64bb4-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="64bb4-105">Properties</span></span>
| <span data-ttu-id="64bb4-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="64bb4-106">Property</span></span>     | <span data-ttu-id="64bb4-107">Typ</span><span class="sxs-lookup"><span data-stu-id="64bb4-107">Type</span></span>   |<span data-ttu-id="64bb4-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="64bb4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64bb4-109">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="64bb4-109">extensionAttribute1</span></span>|<span data-ttu-id="64bb4-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="64bb4-110">String</span></span>| <span data-ttu-id="64bb4-111">Erste anpassbares Erweiterungsattribut.</span><span class="sxs-lookup"><span data-stu-id="64bb4-111">First customizable extension attribute.</span></span> |
|<span data-ttu-id="64bb4-112">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="64bb4-112">extensionAttribute2</span></span>|<span data-ttu-id="64bb4-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="64bb4-113">String</span></span>| <span data-ttu-id="64bb4-114">Zweites anpassbares Erweiterungsattribut.</span><span class="sxs-lookup"><span data-stu-id="64bb4-114">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="64bb4-115">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="64bb4-115">extensionAttribute3</span></span>|<span data-ttu-id="64bb4-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="64bb4-116">String</span></span>| <span data-ttu-id="64bb4-117">Drittes anpassbares Erweiterungsattribut.</span><span class="sxs-lookup"><span data-stu-id="64bb4-117">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="64bb4-118">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="64bb4-118">extensionAttribute4</span></span>|<span data-ttu-id="64bb4-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="64bb4-119">String</span></span>| <span data-ttu-id="64bb4-120">Viertes anpassbares Erweiterungsattribut.</span><span class="sxs-lookup"><span data-stu-id="64bb4-120">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="64bb4-121">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="64bb4-121">extensionAttribute5</span></span>|<span data-ttu-id="64bb4-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="64bb4-122">String</span></span>| <span data-ttu-id="64bb4-123">Fünftes anpassbares Erweiterungsattribut.</span><span class="sxs-lookup"><span data-stu-id="64bb4-123">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="64bb4-124">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="64bb4-124">extensionAttribute6</span></span>|<span data-ttu-id="64bb4-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="64bb4-125">String</span></span>| <span data-ttu-id="64bb4-126">Sechstes anpassbares Erweiterungsattribut.</span><span class="sxs-lookup"><span data-stu-id="64bb4-126">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="64bb4-127">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="64bb4-127">extensionAttribute7</span></span>|<span data-ttu-id="64bb4-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="64bb4-128">String</span></span>| <span data-ttu-id="64bb4-129">Siebtes anpassbares Erweiterungsattribut.</span><span class="sxs-lookup"><span data-stu-id="64bb4-129">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="64bb4-130">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="64bb4-130">extensionAttribute8</span></span>|<span data-ttu-id="64bb4-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="64bb4-131">String</span></span>| <span data-ttu-id="64bb4-132">Achtes anpassbares Erweiterungsattribut.</span><span class="sxs-lookup"><span data-stu-id="64bb4-132">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="64bb4-133">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="64bb4-133">extensionAttribute9</span></span>|<span data-ttu-id="64bb4-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="64bb4-134">String</span></span>| <span data-ttu-id="64bb4-135">Neuntes anpassbares Erweiterungsattribut.</span><span class="sxs-lookup"><span data-stu-id="64bb4-135">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="64bb4-136">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="64bb4-136">extensionAttribute10</span></span>|<span data-ttu-id="64bb4-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="64bb4-137">String</span></span>| <span data-ttu-id="64bb4-138">Zehntes anpassbares Erweierungsattribut.</span><span class="sxs-lookup"><span data-stu-id="64bb4-138">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="64bb4-139">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="64bb4-139">extensionAttribute11</span></span>|<span data-ttu-id="64bb4-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="64bb4-140">String</span></span>| <span data-ttu-id="64bb4-141">Elftes anpassbares Erweiterungsattribut.</span><span class="sxs-lookup"><span data-stu-id="64bb4-141">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="64bb4-142">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="64bb4-142">extensionAttribute12</span></span>|<span data-ttu-id="64bb4-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="64bb4-143">String</span></span>| <span data-ttu-id="64bb4-144">Zwölftes anpassbares Erweiterungsattribut.</span><span class="sxs-lookup"><span data-stu-id="64bb4-144">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="64bb4-145">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="64bb4-145">extensionAttribute13</span></span>|<span data-ttu-id="64bb4-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="64bb4-146">String</span></span>| <span data-ttu-id="64bb4-147">Dreizehntes anpassbares Erweiterungsattribut.</span><span class="sxs-lookup"><span data-stu-id="64bb4-147">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="64bb4-148">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="64bb4-148">extensionAttribute14</span></span>|<span data-ttu-id="64bb4-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="64bb4-149">String</span></span>| <span data-ttu-id="64bb4-150">Vierzehntes anpassbares Erweiterungsattribut.</span><span class="sxs-lookup"><span data-stu-id="64bb4-150">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="64bb4-151">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="64bb4-151">extensionAttribute15</span></span>|<span data-ttu-id="64bb4-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="64bb4-152">String</span></span>| <span data-ttu-id="64bb4-153">Fünfzehntes anpassbares Erweiterungsattribut.</span><span class="sxs-lookup"><span data-stu-id="64bb4-153">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="64bb4-154">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="64bb4-154">JSON representation</span></span>

<span data-ttu-id="64bb4-155">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="64bb4-155">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
}-->


```json
{
      "extensionAttribute1": "string",
      "extensionAttribute2": "string",
      "extensionAttribute3": "string",
      "extensionAttribute4": "string",
      "extensionAttribute5": "string",
      "extensionAttribute6": "string",
      "extensionAttribute7": "string",
      "extensionAttribute8": "string",
      "extensionAttribute9": "string",
      "extensionAttribute10": "string",
      "extensionAttribute11": "string",
      "extensionAttribute12": "string",
      "extensionAttribute13": "string",
      "extensionAttribute14": "string",
      "extensionAttribute15": "string"
  }

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->