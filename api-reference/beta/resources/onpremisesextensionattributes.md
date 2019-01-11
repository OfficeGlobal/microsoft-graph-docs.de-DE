---
title: Ressourcentyp onPremisesExtensionAttributes
description: Die **OnPremisesExtensionAttributes** -Eigenschaft der Benutzerentität enthält fünfzehn Eigenschaften der benutzerdefinierten Erweiterung-Attribut. Diese Gruppe von Eigenschaften ist für einen Benutzer **OnPremisesSyncEnabled** im lokalen Active Directory gesteuert und Azure AD synchronisiert und ist schreibgeschützt. Für einen nur-Cloud-Benutzer (wobei **OnPremisesSyncEnabled** ist false), können diese Eigenschaften festgelegt werden, während der Erstellung oder zu aktualisieren.
localization_priority: Normal
ms.openlocfilehash: 44589338e25e01cb483df6bfa3c1e078e352f5ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868159"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="07950-105">Ressourcentyp onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="07950-105">onPremisesExtensionAttributes resource type</span></span>

> <span data-ttu-id="07950-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="07950-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07950-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="07950-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="07950-108">Die **OnPremisesExtensionAttributes** -Eigenschaft der [Benutzer](user.md) Entität enthält fünfzehn Eigenschaften der benutzerdefinierten Erweiterung-Attribut.</span><span class="sxs-lookup"><span data-stu-id="07950-108">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="07950-109">Diese Gruppe von Eigenschaften ist für einen Benutzer **OnPremisesSyncEnabled** im lokalen Active Directory gesteuert und Azure AD synchronisiert und ist schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="07950-109">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="07950-110">Für einen nur-Cloud-Benutzer (wobei **OnPremisesSyncEnabled** ist false), können diese Eigenschaften festgelegt werden, während der Erstellung oder zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="07950-110">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="07950-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="07950-111">Properties</span></span>
| <span data-ttu-id="07950-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="07950-112">Property</span></span>     | <span data-ttu-id="07950-113">Typ</span><span class="sxs-lookup"><span data-stu-id="07950-113">Type</span></span>   |<span data-ttu-id="07950-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07950-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07950-115">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="07950-115">extensionAttribute1</span></span>|<span data-ttu-id="07950-116">String</span><span class="sxs-lookup"><span data-stu-id="07950-116">String</span></span>| <span data-ttu-id="07950-117">Erste anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="07950-117">First customizable extension attribute.</span></span> |
|<span data-ttu-id="07950-118">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="07950-118">extensionAttribute2</span></span>|<span data-ttu-id="07950-119">String</span><span class="sxs-lookup"><span data-stu-id="07950-119">String</span></span>| <span data-ttu-id="07950-120">Zweite anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="07950-120">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="07950-121">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="07950-121">extensionAttribute3</span></span>|<span data-ttu-id="07950-122">String</span><span class="sxs-lookup"><span data-stu-id="07950-122">String</span></span>| <span data-ttu-id="07950-123">Dritte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="07950-123">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="07950-124">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="07950-124">extensionAttribute4</span></span>|<span data-ttu-id="07950-125">String</span><span class="sxs-lookup"><span data-stu-id="07950-125">String</span></span>| <span data-ttu-id="07950-126">Vierte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="07950-126">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="07950-127">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="07950-127">extensionAttribute5</span></span>|<span data-ttu-id="07950-128">String</span><span class="sxs-lookup"><span data-stu-id="07950-128">String</span></span>| <span data-ttu-id="07950-129">Fünfte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="07950-129">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="07950-130">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="07950-130">extensionAttribute6</span></span>|<span data-ttu-id="07950-131">String</span><span class="sxs-lookup"><span data-stu-id="07950-131">String</span></span>| <span data-ttu-id="07950-132">Sechste anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="07950-132">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="07950-133">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="07950-133">extensionAttribute7</span></span>|<span data-ttu-id="07950-134">String</span><span class="sxs-lookup"><span data-stu-id="07950-134">String</span></span>| <span data-ttu-id="07950-135">Siebte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="07950-135">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="07950-136">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="07950-136">extensionAttribute8</span></span>|<span data-ttu-id="07950-137">String</span><span class="sxs-lookup"><span data-stu-id="07950-137">String</span></span>| <span data-ttu-id="07950-138">Achte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="07950-138">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="07950-139">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="07950-139">extensionAttribute9</span></span>|<span data-ttu-id="07950-140">String</span><span class="sxs-lookup"><span data-stu-id="07950-140">String</span></span>| <span data-ttu-id="07950-141">Neunte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="07950-141">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="07950-142">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="07950-142">extensionAttribute10</span></span>|<span data-ttu-id="07950-143">String</span><span class="sxs-lookup"><span data-stu-id="07950-143">String</span></span>| <span data-ttu-id="07950-144">Zehnte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="07950-144">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="07950-145">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="07950-145">extensionAttribute11</span></span>|<span data-ttu-id="07950-146">String</span><span class="sxs-lookup"><span data-stu-id="07950-146">String</span></span>| <span data-ttu-id="07950-147">Elfte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="07950-147">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="07950-148">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="07950-148">extensionAttribute12</span></span>|<span data-ttu-id="07950-149">String</span><span class="sxs-lookup"><span data-stu-id="07950-149">String</span></span>| <span data-ttu-id="07950-150">Zwölfte anpassbarer Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="07950-150">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="07950-151">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="07950-151">extensionAttribute13</span></span>|<span data-ttu-id="07950-152">String</span><span class="sxs-lookup"><span data-stu-id="07950-152">String</span></span>| <span data-ttu-id="07950-153">Dreizehnte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="07950-153">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="07950-154">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="07950-154">extensionAttribute14</span></span>|<span data-ttu-id="07950-155">String</span><span class="sxs-lookup"><span data-stu-id="07950-155">String</span></span>| <span data-ttu-id="07950-156">Vierzehnte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="07950-156">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="07950-157">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="07950-157">extensionAttribute15</span></span>|<span data-ttu-id="07950-158">String</span><span class="sxs-lookup"><span data-stu-id="07950-158">String</span></span>| <span data-ttu-id="07950-159">Fünfzehnte anpassbare Extension-Attribut.</span><span class="sxs-lookup"><span data-stu-id="07950-159">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="07950-160">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="07950-160">JSON representation</span></span>

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
