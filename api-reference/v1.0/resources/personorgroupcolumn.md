---
author: simonhult
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 5ff8d61a2796edd615a66416b4f8f4d6d565909a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985450"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="280f4-102">PersonOrGroupColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="280f4-102">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="280f4-103">Die **personOrGroupColumn** zu einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass die Werte der Spalte eine aus dem Verzeichnis ausgewählte Person oder Gruppe darstellen.</span><span class="sxs-lookup"><span data-stu-id="280f4-103">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="280f4-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="280f4-104">JSON representation</span></span>

<span data-ttu-id="280f4-105">Es folgt eine JSON-Darstellung einer **personOrGroupColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="280f4-105">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="280f4-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="280f4-106">Properties</span></span>

| <span data-ttu-id="280f4-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="280f4-107">Property name</span></span>              | <span data-ttu-id="280f4-108">Typ</span><span class="sxs-lookup"><span data-stu-id="280f4-108">Type</span></span>    | <span data-ttu-id="280f4-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="280f4-109">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="280f4-110">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="280f4-110">**allowMultipleSelection**</span></span> | <span data-ttu-id="280f4-111">boolean</span><span class="sxs-lookup"><span data-stu-id="280f4-111">boolean</span></span> | <span data-ttu-id="280f4-112">Gibt an, ob mehrere Werte aus der Quelle ausgewählt werden können.</span><span class="sxs-lookup"><span data-stu-id="280f4-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="280f4-113">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="280f4-113">**displayAs**</span></span>              | <span data-ttu-id="280f4-114">string</span><span class="sxs-lookup"><span data-stu-id="280f4-114">string</span></span>  | <span data-ttu-id="280f4-115">Informationen zum Anzeigen der Informationen zu der ausgewählten Person oder Gruppe.</span><span class="sxs-lookup"><span data-stu-id="280f4-115">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="280f4-116">Siehe unten.</span><span class="sxs-lookup"><span data-stu-id="280f4-116">See below.</span></span>
| <span data-ttu-id="280f4-117">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="280f4-117">**chooseFromType**</span></span>         | <span data-ttu-id="280f4-118">string</span><span class="sxs-lookup"><span data-stu-id="280f4-118">string</span></span>  | <span data-ttu-id="280f4-119">Gibt an, ob nur Personen oder Personen und Gruppen ausgewählt werden können.</span><span class="sxs-lookup"><span data-stu-id="280f4-119">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="280f4-120">Müssen `peopleAndGroups` oder `peopleOnly` sein.</span><span class="sxs-lookup"><span data-stu-id="280f4-120">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-options"></a><span data-ttu-id="280f4-121">DisplayAs-Optionen</span><span class="sxs-lookup"><span data-stu-id="280f4-121">DisplayAs options</span></span>

| <span data-ttu-id="280f4-122">DisplayAs-Wert</span><span class="sxs-lookup"><span data-stu-id="280f4-122">DisplayAs value</span></span>               | <span data-ttu-id="280f4-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="280f4-123">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="280f4-124">**account**</span><span class="sxs-lookup"><span data-stu-id="280f4-124">**account**</span></span>                   | <span data-ttu-id="280f4-125">Die rohe SharePoint-codierte Anforderungszeichenfolge für die Person oder Gruppe (z. B.</span><span class="sxs-lookup"><span data-stu-id="280f4-125">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="280f4-126">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="280f4-126">i:0#.f</span></span>|<span data-ttu-id="280f4-127">Mitgliedschaft</span><span class="sxs-lookup"><span data-stu-id="280f4-127">membership</span></span>|<span data-ttu-id="280f4-128">jane@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="280f4-128">jane@contoso.com).</span></span>
| <span data-ttu-id="280f4-129">**department**</span><span class="sxs-lookup"><span data-stu-id="280f4-129">**department**</span></span>                | <span data-ttu-id="280f4-130">Die Abteilung der Person oder Gruppe.</span><span class="sxs-lookup"><span data-stu-id="280f4-130">The person or group's department.</span></span>
| <span data-ttu-id="280f4-131">**firstName**</span><span class="sxs-lookup"><span data-stu-id="280f4-131">**firstName**</span></span>                 | <span data-ttu-id="280f4-132">The person's first name.</span><span class="sxs-lookup"><span data-stu-id="280f4-132">The person's first name.</span></span>
| <span data-ttu-id="280f4-133">**id**</span><span class="sxs-lookup"><span data-stu-id="280f4-133">**id**</span></span>                        | <span data-ttu-id="280f4-134">Die ID der Person oder Gruppe im Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="280f4-134">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="280f4-135">**lastName**</span><span class="sxs-lookup"><span data-stu-id="280f4-135">**lastName**</span></span>                  | <span data-ttu-id="280f4-136">Der Nachname der Person.</span><span class="sxs-lookup"><span data-stu-id="280f4-136">The person's last name.</span></span>
| <span data-ttu-id="280f4-137">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="280f4-137">**mobilePhone**</span></span>               | <span data-ttu-id="280f4-138">Die Mobiltelefonnummer der Person.</span><span class="sxs-lookup"><span data-stu-id="280f4-138">The person's mobile phone number.</span></span>
| <span data-ttu-id="280f4-139">**name**</span><span class="sxs-lookup"><span data-stu-id="280f4-139">**name**</span></span>                      | <span data-ttu-id="280f4-140">Der Name der Person.</span><span class="sxs-lookup"><span data-stu-id="280f4-140">The person's name.</span></span>
| <span data-ttu-id="280f4-141">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="280f4-141">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="280f4-142">Der Name der Person mit ihrem Bild und zusätzlichen Details.</span><span class="sxs-lookup"><span data-stu-id="280f4-142">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="280f4-143">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="280f4-143">**nameWithPresence**</span></span>          | <span data-ttu-id="280f4-144">Standard.</span><span class="sxs-lookup"><span data-stu-id="280f4-144">Default.</span></span> <span data-ttu-id="280f4-145">Der Name der Person mit einem Anwesenheitssymbol (verfügbar/beschäftigt/usw.).</span><span class="sxs-lookup"><span data-stu-id="280f4-145">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="280f4-146">**office**</span><span class="sxs-lookup"><span data-stu-id="280f4-146">**office**</span></span>                    | <span data-ttu-id="280f4-147">Die Büronummer der Person.</span><span class="sxs-lookup"><span data-stu-id="280f4-147">The person's office number.</span></span>
| <span data-ttu-id="280f4-148">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="280f4-148">**pictureOnly36x36**</span></span>          | <span data-ttu-id="280f4-149">Das Bild der Person, begrenzt durch ein 36-x-36-px-Quadrat.</span><span class="sxs-lookup"><span data-stu-id="280f4-149">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="280f4-150">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="280f4-150">**pictureOnly48x48**</span></span>          | <span data-ttu-id="280f4-151">Das Bild der Person, begrenzt durch ein 48-x-48-px-Quadrat.</span><span class="sxs-lookup"><span data-stu-id="280f4-151">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="280f4-152">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="280f4-152">**pictureOnly72x72**</span></span>          | <span data-ttu-id="280f4-153">Das Bild der Person, begrenzt durch ein 72-x-72-px-Quadrat.</span><span class="sxs-lookup"><span data-stu-id="280f4-153">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="280f4-154">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="280f4-154">**sipAddress**</span></span>                | <span data-ttu-id="280f4-155">Die SIP-Adresse der Person.</span><span class="sxs-lookup"><span data-stu-id="280f4-155">The person's sip address.</span></span>
| <span data-ttu-id="280f4-156">**title**</span><span class="sxs-lookup"><span data-stu-id="280f4-156">**title**</span></span>                     | <span data-ttu-id="280f4-157">Titel der Person in der Organisation.</span><span class="sxs-lookup"><span data-stu-id="280f4-157">The person's title in the organization.</span></span>
| <span data-ttu-id="280f4-158">**userName**</span><span class="sxs-lookup"><span data-stu-id="280f4-158">**userName**</span></span>                  | <span data-ttu-id="280f4-159">Die Person oder der Benutzername der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="280f4-159">The person or group's user name.</span></span>
| <span data-ttu-id="280f4-160">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="280f4-160">**workEmail**</span></span>                 | <span data-ttu-id="280f4-161">Die Person oder die E-Mail-Adresse der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="280f4-161">The person or group's email address.</span></span>
| <span data-ttu-id="280f4-162">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="280f4-162">**workPhone**</span></span>                 | <span data-ttu-id="280f4-163">Die Telefonnummer bei der Arbeit der Person.</span><span class="sxs-lookup"><span data-stu-id="280f4-163">The person's work phone number.</span></span>

<span data-ttu-id="280f4-164">Hinweis: Möglicherweise werden weitere DisplayAs-Typen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="280f4-164">Note: Additional DisplayAs types may be returned.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/personorgroupcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(peopleAndGroups,peopleOnly) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/personorgroupcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(account,contentType,created,department,...) are in resource, but () are in table"
  ],
  "tocPath": "Resources/PersonOrGroupColumn"
} -->
