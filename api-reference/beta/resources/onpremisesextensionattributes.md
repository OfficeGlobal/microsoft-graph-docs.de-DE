---
title: Ressourcentyp onPremisesExtensionAttributes
description: Die **OnPremisesExtensionAttributes** -Eigenschaft der Benutzerentität enthält fünfzehn Eigenschaften der benutzerdefinierten Erweiterung-Attribut. Bei einem onPremisesSyncEnabled-Benutzer wird dieser Eigenschaftensatz als Master-Datensatz im lokalen Active Directory verwaltet und mit Azure AD synchronisiert. Er ist außerdem schreibgeschützt. Bei einem reinen Cloud-Benutzer (wenn „onPremisesSyncEnabled“ auf „false“ gesetzt ist) können diese Eigenschaften beim Erstellen oder Aktualisieren festgelegt werden.
localization_priority: Normal
ms.openlocfilehash: f44f71fdcd86d2165289282568a2d7153ccc99b1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518240"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="1ba4b-105">Ressourcentyp onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="1ba4b-105">onPremisesExtensionAttributes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ba4b-106">Die **OnPremisesExtensionAttributes** -Eigenschaft der [Benutzer](user.md) Entität enthält fünfzehn Eigenschaften der benutzerdefinierten Erweiterung-Attribut.</span><span class="sxs-lookup"><span data-stu-id="1ba4b-106">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="1ba4b-107">Bei einem onPremisesSyncEnabled-Benutzer wird dieser Eigenschaftensatz als Master-Datensatz im lokalen Active Directory verwaltet und mit Azure AD synchronisiert. Er ist außerdem schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1ba4b-107">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="1ba4b-108">Bei einem reinen Cloud-Benutzer (wenn „onPremisesSyncEnabled“ auf „false“ gesetzt ist) können diese Eigenschaften beim Erstellen oder Aktualisieren festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="1ba4b-108">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="1ba4b-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1ba4b-109">Properties</span></span>
| <span data-ttu-id="1ba4b-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1ba4b-110">Property</span></span>     | <span data-ttu-id="1ba4b-111">Typ</span><span class="sxs-lookup"><span data-stu-id="1ba4b-111">Type</span></span>   |<span data-ttu-id="1ba4b-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1ba4b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ba4b-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="1ba4b-113">extensionAttribute1</span></span>|<span data-ttu-id="1ba4b-114">String</span><span class="sxs-lookup"><span data-stu-id="1ba4b-114">String</span></span>| <span data-ttu-id="1ba4b-115">Erste anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="1ba4b-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="1ba4b-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="1ba4b-116">extensionAttribute2</span></span>|<span data-ttu-id="1ba4b-117">String</span><span class="sxs-lookup"><span data-stu-id="1ba4b-117">String</span></span>| <span data-ttu-id="1ba4b-118">Zweite anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="1ba4b-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="1ba4b-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="1ba4b-119">extensionAttribute3</span></span>|<span data-ttu-id="1ba4b-120">String</span><span class="sxs-lookup"><span data-stu-id="1ba4b-120">String</span></span>| <span data-ttu-id="1ba4b-121">Dritte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="1ba4b-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="1ba4b-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="1ba4b-122">extensionAttribute4</span></span>|<span data-ttu-id="1ba4b-123">String</span><span class="sxs-lookup"><span data-stu-id="1ba4b-123">String</span></span>| <span data-ttu-id="1ba4b-124">Vierte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="1ba4b-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="1ba4b-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="1ba4b-125">extensionAttribute5</span></span>|<span data-ttu-id="1ba4b-126">String</span><span class="sxs-lookup"><span data-stu-id="1ba4b-126">String</span></span>| <span data-ttu-id="1ba4b-127">Fünfte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="1ba4b-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="1ba4b-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="1ba4b-128">extensionAttribute6</span></span>|<span data-ttu-id="1ba4b-129">String</span><span class="sxs-lookup"><span data-stu-id="1ba4b-129">String</span></span>| <span data-ttu-id="1ba4b-130">Sechste anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="1ba4b-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="1ba4b-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="1ba4b-131">extensionAttribute7</span></span>|<span data-ttu-id="1ba4b-132">String</span><span class="sxs-lookup"><span data-stu-id="1ba4b-132">String</span></span>| <span data-ttu-id="1ba4b-133">Siebte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="1ba4b-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="1ba4b-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="1ba4b-134">extensionAttribute8</span></span>|<span data-ttu-id="1ba4b-135">String</span><span class="sxs-lookup"><span data-stu-id="1ba4b-135">String</span></span>| <span data-ttu-id="1ba4b-136">Achte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="1ba4b-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="1ba4b-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="1ba4b-137">extensionAttribute9</span></span>|<span data-ttu-id="1ba4b-138">String</span><span class="sxs-lookup"><span data-stu-id="1ba4b-138">String</span></span>| <span data-ttu-id="1ba4b-139">Neunte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="1ba4b-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="1ba4b-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="1ba4b-140">extensionAttribute10</span></span>|<span data-ttu-id="1ba4b-141">String</span><span class="sxs-lookup"><span data-stu-id="1ba4b-141">String</span></span>| <span data-ttu-id="1ba4b-142">Zehnte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="1ba4b-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="1ba4b-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="1ba4b-143">extensionAttribute11</span></span>|<span data-ttu-id="1ba4b-144">String</span><span class="sxs-lookup"><span data-stu-id="1ba4b-144">String</span></span>| <span data-ttu-id="1ba4b-145">Elfte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="1ba4b-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="1ba4b-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="1ba4b-146">extensionAttribute12</span></span>|<span data-ttu-id="1ba4b-147">String</span><span class="sxs-lookup"><span data-stu-id="1ba4b-147">String</span></span>| <span data-ttu-id="1ba4b-148">Zwölfte anpassbarer Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="1ba4b-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="1ba4b-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="1ba4b-149">extensionAttribute13</span></span>|<span data-ttu-id="1ba4b-150">String</span><span class="sxs-lookup"><span data-stu-id="1ba4b-150">String</span></span>| <span data-ttu-id="1ba4b-151">Dreizehnte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="1ba4b-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="1ba4b-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="1ba4b-152">extensionAttribute14</span></span>|<span data-ttu-id="1ba4b-153">String</span><span class="sxs-lookup"><span data-stu-id="1ba4b-153">String</span></span>| <span data-ttu-id="1ba4b-154">Vierzehnte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="1ba4b-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="1ba4b-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="1ba4b-155">extensionAttribute15</span></span>|<span data-ttu-id="1ba4b-156">String</span><span class="sxs-lookup"><span data-stu-id="1ba4b-156">String</span></span>| <span data-ttu-id="1ba4b-157">Fünfzehnte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="1ba4b-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1ba4b-158">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1ba4b-158">JSON representation</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisesextensionattributes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
