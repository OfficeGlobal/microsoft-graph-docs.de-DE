---
title: Ressourcentyp onPremisesExtensionAttributes
description: Die **OnPremisesExtensionAttributes** -Eigenschaft der Benutzerentität enthält fünfzehn Eigenschaften der benutzerdefinierten Erweiterung-Attribut. Diese Gruppe von Eigenschaften ist für einen Benutzer **OnPremisesSyncEnabled** im lokalen Active Directory gesteuert und Azure AD synchronisiert und ist schreibgeschützt. Für einen nur-Cloud-Benutzer (wobei **OnPremisesSyncEnabled** ist false), können diese Eigenschaften festgelegt werden, während der Erstellung oder zu aktualisieren.
ms.openlocfilehash: e5a56b5a846cf48cfc819b6d884689be10d6992e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018252"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="35fe7-105">Ressourcentyp onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="35fe7-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="35fe7-106">Die **OnPremisesExtensionAttributes** -Eigenschaft der [Benutzer](user.md) Entität enthält fünfzehn Eigenschaften der benutzerdefinierten Erweiterung-Attribut.</span><span class="sxs-lookup"><span data-stu-id="35fe7-106">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="35fe7-107">Diese Gruppe von Eigenschaften ist für einen Benutzer **OnPremisesSyncEnabled** im lokalen Active Directory gesteuert und Azure AD synchronisiert und ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="35fe7-107">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="35fe7-108">Für einen nur-Cloud-Benutzer (wobei **OnPremisesSyncEnabled** ist false), können diese Eigenschaften festgelegt werden, während der Erstellung oder zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="35fe7-108">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="35fe7-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="35fe7-109">Properties</span></span>
| <span data-ttu-id="35fe7-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="35fe7-110">Property</span></span>     | <span data-ttu-id="35fe7-111">Typ</span><span class="sxs-lookup"><span data-stu-id="35fe7-111">Type</span></span>   |<span data-ttu-id="35fe7-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="35fe7-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35fe7-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="35fe7-113">extensionAttribute1</span></span>|<span data-ttu-id="35fe7-114">String</span><span class="sxs-lookup"><span data-stu-id="35fe7-114">String</span></span>| <span data-ttu-id="35fe7-115">Erste anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="35fe7-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="35fe7-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="35fe7-116">extensionAttribute2</span></span>|<span data-ttu-id="35fe7-117">String</span><span class="sxs-lookup"><span data-stu-id="35fe7-117">String</span></span>| <span data-ttu-id="35fe7-118">Zweite anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="35fe7-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="35fe7-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="35fe7-119">extensionAttribute3</span></span>|<span data-ttu-id="35fe7-120">String</span><span class="sxs-lookup"><span data-stu-id="35fe7-120">String</span></span>| <span data-ttu-id="35fe7-121">Dritte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="35fe7-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="35fe7-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="35fe7-122">extensionAttribute4</span></span>|<span data-ttu-id="35fe7-123">String</span><span class="sxs-lookup"><span data-stu-id="35fe7-123">String</span></span>| <span data-ttu-id="35fe7-124">Vierte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="35fe7-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="35fe7-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="35fe7-125">extensionAttribute5</span></span>|<span data-ttu-id="35fe7-126">String</span><span class="sxs-lookup"><span data-stu-id="35fe7-126">String</span></span>| <span data-ttu-id="35fe7-127">Fünfte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="35fe7-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="35fe7-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="35fe7-128">extensionAttribute6</span></span>|<span data-ttu-id="35fe7-129">String</span><span class="sxs-lookup"><span data-stu-id="35fe7-129">String</span></span>| <span data-ttu-id="35fe7-130">Sechste anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="35fe7-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="35fe7-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="35fe7-131">extensionAttribute7</span></span>|<span data-ttu-id="35fe7-132">String</span><span class="sxs-lookup"><span data-stu-id="35fe7-132">String</span></span>| <span data-ttu-id="35fe7-133">Siebte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="35fe7-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="35fe7-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="35fe7-134">extensionAttribute8</span></span>|<span data-ttu-id="35fe7-135">String</span><span class="sxs-lookup"><span data-stu-id="35fe7-135">String</span></span>| <span data-ttu-id="35fe7-136">Achte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="35fe7-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="35fe7-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="35fe7-137">extensionAttribute9</span></span>|<span data-ttu-id="35fe7-138">String</span><span class="sxs-lookup"><span data-stu-id="35fe7-138">String</span></span>| <span data-ttu-id="35fe7-139">Neunte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="35fe7-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="35fe7-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="35fe7-140">extensionAttribute10</span></span>|<span data-ttu-id="35fe7-141">String</span><span class="sxs-lookup"><span data-stu-id="35fe7-141">String</span></span>| <span data-ttu-id="35fe7-142">Zehnte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="35fe7-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="35fe7-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="35fe7-143">extensionAttribute11</span></span>|<span data-ttu-id="35fe7-144">String</span><span class="sxs-lookup"><span data-stu-id="35fe7-144">String</span></span>| <span data-ttu-id="35fe7-145">Elfte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="35fe7-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="35fe7-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="35fe7-146">extensionAttribute12</span></span>|<span data-ttu-id="35fe7-147">String</span><span class="sxs-lookup"><span data-stu-id="35fe7-147">String</span></span>| <span data-ttu-id="35fe7-148">Zwölfte anpassbarer Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="35fe7-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="35fe7-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="35fe7-149">extensionAttribute13</span></span>|<span data-ttu-id="35fe7-150">String</span><span class="sxs-lookup"><span data-stu-id="35fe7-150">String</span></span>| <span data-ttu-id="35fe7-151">Dreizehnte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="35fe7-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="35fe7-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="35fe7-152">extensionAttribute14</span></span>|<span data-ttu-id="35fe7-153">String</span><span class="sxs-lookup"><span data-stu-id="35fe7-153">String</span></span>| <span data-ttu-id="35fe7-154">Vierzehnte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="35fe7-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="35fe7-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="35fe7-155">extensionAttribute15</span></span>|<span data-ttu-id="35fe7-156">String</span><span class="sxs-lookup"><span data-stu-id="35fe7-156">String</span></span>| <span data-ttu-id="35fe7-157">Fünfzehnte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="35fe7-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="35fe7-158">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="35fe7-158">JSON representation</span></span>

<span data-ttu-id="35fe7-159">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="35fe7-159">Here is a JSON representation of the resource</span></span>

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