---
title: Ressourcentyp onPremisesExtensionAttributes
description: Die **OnPremisesExtensionAttributes** -Eigenschaft der Benutzerentität enthält fünfzehn Eigenschaften der benutzerdefinierten Erweiterung-Attribut. Diese Gruppe von Eigenschaften ist für einen Benutzer **OnPremisesSyncEnabled** im lokalen Active Directory gesteuert und Azure AD synchronisiert und ist schreibgeschützt. Für einen nur-Cloud-Benutzer (wobei **OnPremisesSyncEnabled** ist false), können diese Eigenschaften festgelegt werden, während der Erstellung oder zu aktualisieren.
localization_priority: Normal
ms.openlocfilehash: c0cb765efe9e94c8254e45eaa9d55bc16382f6d2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824745"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="ce9b9-105">Ressourcentyp onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="ce9b9-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="ce9b9-106">Die **OnPremisesExtensionAttributes** -Eigenschaft der [Benutzer](user.md) Entität enthält fünfzehn Eigenschaften der benutzerdefinierten Erweiterung-Attribut.</span><span class="sxs-lookup"><span data-stu-id="ce9b9-106">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="ce9b9-107">Diese Gruppe von Eigenschaften ist für einen Benutzer **OnPremisesSyncEnabled** im lokalen Active Directory gesteuert und Azure AD synchronisiert und ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="ce9b9-107">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="ce9b9-108">Für einen nur-Cloud-Benutzer (wobei **OnPremisesSyncEnabled** ist false), können diese Eigenschaften festgelegt werden, während der Erstellung oder zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="ce9b9-108">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="ce9b9-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ce9b9-109">Properties</span></span>
| <span data-ttu-id="ce9b9-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ce9b9-110">Property</span></span>     | <span data-ttu-id="ce9b9-111">Typ</span><span class="sxs-lookup"><span data-stu-id="ce9b9-111">Type</span></span>   |<span data-ttu-id="ce9b9-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ce9b9-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce9b9-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="ce9b9-113">extensionAttribute1</span></span>|<span data-ttu-id="ce9b9-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce9b9-114">String</span></span>| <span data-ttu-id="ce9b9-115">Erste anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="ce9b9-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="ce9b9-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="ce9b9-116">extensionAttribute2</span></span>|<span data-ttu-id="ce9b9-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce9b9-117">String</span></span>| <span data-ttu-id="ce9b9-118">Zweite anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="ce9b9-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="ce9b9-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="ce9b9-119">extensionAttribute3</span></span>|<span data-ttu-id="ce9b9-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce9b9-120">String</span></span>| <span data-ttu-id="ce9b9-121">Dritte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="ce9b9-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="ce9b9-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="ce9b9-122">extensionAttribute4</span></span>|<span data-ttu-id="ce9b9-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce9b9-123">String</span></span>| <span data-ttu-id="ce9b9-124">Vierte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="ce9b9-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="ce9b9-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="ce9b9-125">extensionAttribute5</span></span>|<span data-ttu-id="ce9b9-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce9b9-126">String</span></span>| <span data-ttu-id="ce9b9-127">Fünfte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="ce9b9-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="ce9b9-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="ce9b9-128">extensionAttribute6</span></span>|<span data-ttu-id="ce9b9-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce9b9-129">String</span></span>| <span data-ttu-id="ce9b9-130">Sechste anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="ce9b9-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="ce9b9-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="ce9b9-131">extensionAttribute7</span></span>|<span data-ttu-id="ce9b9-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce9b9-132">String</span></span>| <span data-ttu-id="ce9b9-133">Siebte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="ce9b9-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="ce9b9-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="ce9b9-134">extensionAttribute8</span></span>|<span data-ttu-id="ce9b9-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce9b9-135">String</span></span>| <span data-ttu-id="ce9b9-136">Achte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="ce9b9-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="ce9b9-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="ce9b9-137">extensionAttribute9</span></span>|<span data-ttu-id="ce9b9-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce9b9-138">String</span></span>| <span data-ttu-id="ce9b9-139">Neunte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="ce9b9-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="ce9b9-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="ce9b9-140">extensionAttribute10</span></span>|<span data-ttu-id="ce9b9-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce9b9-141">String</span></span>| <span data-ttu-id="ce9b9-142">Zehnte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="ce9b9-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="ce9b9-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="ce9b9-143">extensionAttribute11</span></span>|<span data-ttu-id="ce9b9-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce9b9-144">String</span></span>| <span data-ttu-id="ce9b9-145">Elfte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="ce9b9-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="ce9b9-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="ce9b9-146">extensionAttribute12</span></span>|<span data-ttu-id="ce9b9-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce9b9-147">String</span></span>| <span data-ttu-id="ce9b9-148">Zwölfte anpassbarer Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="ce9b9-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="ce9b9-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="ce9b9-149">extensionAttribute13</span></span>|<span data-ttu-id="ce9b9-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce9b9-150">String</span></span>| <span data-ttu-id="ce9b9-151">Dreizehnte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="ce9b9-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="ce9b9-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="ce9b9-152">extensionAttribute14</span></span>|<span data-ttu-id="ce9b9-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce9b9-153">String</span></span>| <span data-ttu-id="ce9b9-154">Vierzehnte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="ce9b9-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="ce9b9-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="ce9b9-155">extensionAttribute15</span></span>|<span data-ttu-id="ce9b9-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce9b9-156">String</span></span>| <span data-ttu-id="ce9b9-157">Fünfzehnte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="ce9b9-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ce9b9-158">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ce9b9-158">JSON representation</span></span>

<span data-ttu-id="ce9b9-159">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ce9b9-159">Here is a JSON representation of the resource</span></span>

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
