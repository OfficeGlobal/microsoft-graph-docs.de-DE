---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: PersonOrGroupColumn
ms.openlocfilehash: b0c6eab7d2111870192a4ed6c30c1cbd72e4163e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018780"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="021ab-102">PersonOrGroupColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="021ab-102">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="021ab-103">Die **personOrGroupColumn** zu einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass die Werte der Spalte eine aus dem Verzeichnis ausgewählte Person oder Gruppe darstellen.</span><span class="sxs-lookup"><span data-stu-id="021ab-103">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="021ab-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="021ab-104">JSON representation</span></span>

<span data-ttu-id="021ab-105">Es folgt eine JSON-Darstellung einer **personOrGroupColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="021ab-105">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="021ab-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="021ab-106">Properties</span></span>

| <span data-ttu-id="021ab-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="021ab-107">Property name</span></span>              | <span data-ttu-id="021ab-108">Typ</span><span class="sxs-lookup"><span data-stu-id="021ab-108">Type</span></span>    | <span data-ttu-id="021ab-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="021ab-109">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="021ab-110">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="021ab-110">**allowMultipleSelection**</span></span> | <span data-ttu-id="021ab-111">boolean</span><span class="sxs-lookup"><span data-stu-id="021ab-111">boolean</span></span> | <span data-ttu-id="021ab-112">Gibt an, ob mehrere Werte aus der Quelle ausgewählt werden können.</span><span class="sxs-lookup"><span data-stu-id="021ab-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="021ab-113">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="021ab-113">**displayAs**</span></span>              | <span data-ttu-id="021ab-114">string</span><span class="sxs-lookup"><span data-stu-id="021ab-114">string</span></span>  | <span data-ttu-id="021ab-115">Informationen zum Anzeigen der Informationen zu der ausgewählten Person oder Gruppe.</span><span class="sxs-lookup"><span data-stu-id="021ab-115">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="021ab-116">Siehe unten.</span><span class="sxs-lookup"><span data-stu-id="021ab-116">See below.</span></span>
| <span data-ttu-id="021ab-117">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="021ab-117">**chooseFromType**</span></span>         | <span data-ttu-id="021ab-118">string</span><span class="sxs-lookup"><span data-stu-id="021ab-118">string</span></span>  | <span data-ttu-id="021ab-119">Gibt an, ob nur Personen oder Personen und Gruppen ausgewählt werden können.</span><span class="sxs-lookup"><span data-stu-id="021ab-119">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="021ab-120">Müssen `peopleAndGroups` oder `peopleOnly` sein.</span><span class="sxs-lookup"><span data-stu-id="021ab-120">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-options"></a><span data-ttu-id="021ab-121">DisplayAs-Optionen</span><span class="sxs-lookup"><span data-stu-id="021ab-121">DisplayAs options</span></span>

| <span data-ttu-id="021ab-122">DisplayAs-Wert</span><span class="sxs-lookup"><span data-stu-id="021ab-122">DisplayAs value</span></span>               | <span data-ttu-id="021ab-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="021ab-123">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="021ab-124">**account**</span><span class="sxs-lookup"><span data-stu-id="021ab-124">**account**</span></span>                   | <span data-ttu-id="021ab-125">Die rohe SharePoint-codierte Anforderungszeichenfolge für die Person oder Gruppe (z. B.</span><span class="sxs-lookup"><span data-stu-id="021ab-125">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="021ab-126">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="021ab-126">i:0#.f</span></span>|<span data-ttu-id="021ab-127">Mitgliedschaft</span><span class="sxs-lookup"><span data-stu-id="021ab-127">membership</span></span>|<span data-ttu-id="021ab-128">jane@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="021ab-128">jane@contoso.com).</span></span>
| <span data-ttu-id="021ab-129">**department**</span><span class="sxs-lookup"><span data-stu-id="021ab-129">**department**</span></span>                | <span data-ttu-id="021ab-130">Die Abteilung der Person oder Gruppe.</span><span class="sxs-lookup"><span data-stu-id="021ab-130">The person or group's department.</span></span>
| <span data-ttu-id="021ab-131">**firstName**</span><span class="sxs-lookup"><span data-stu-id="021ab-131">**firstName**</span></span>                 | <span data-ttu-id="021ab-132">The person's first name.</span><span class="sxs-lookup"><span data-stu-id="021ab-132">The person's first name.</span></span>
| <span data-ttu-id="021ab-133">**id**</span><span class="sxs-lookup"><span data-stu-id="021ab-133">**id**</span></span>                        | <span data-ttu-id="021ab-134">Die ID der Person oder Gruppe im Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="021ab-134">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="021ab-135">**lastName**</span><span class="sxs-lookup"><span data-stu-id="021ab-135">**lastName**</span></span>                  | <span data-ttu-id="021ab-136">Der Nachname der Person.</span><span class="sxs-lookup"><span data-stu-id="021ab-136">The person's last name.</span></span>
| <span data-ttu-id="021ab-137">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="021ab-137">**mobilePhone**</span></span>               | <span data-ttu-id="021ab-138">Die Mobiltelefonnummer der Person.</span><span class="sxs-lookup"><span data-stu-id="021ab-138">The person's mobile phone number.</span></span>
| <span data-ttu-id="021ab-139">**name**</span><span class="sxs-lookup"><span data-stu-id="021ab-139">**name**</span></span>                      | <span data-ttu-id="021ab-140">Der Name der Person.</span><span class="sxs-lookup"><span data-stu-id="021ab-140">The person's name.</span></span>
| <span data-ttu-id="021ab-141">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="021ab-141">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="021ab-142">Der Name der Person mit ihrem Bild und zusätzlichen Details.</span><span class="sxs-lookup"><span data-stu-id="021ab-142">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="021ab-143">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="021ab-143">**nameWithPresence**</span></span>          | <span data-ttu-id="021ab-144">Standard.</span><span class="sxs-lookup"><span data-stu-id="021ab-144">Default.</span></span> <span data-ttu-id="021ab-145">Der Name der Person mit einem Anwesenheitssymbol (verfügbar/beschäftigt/usw.).</span><span class="sxs-lookup"><span data-stu-id="021ab-145">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="021ab-146">**office**</span><span class="sxs-lookup"><span data-stu-id="021ab-146">**office**</span></span>                    | <span data-ttu-id="021ab-147">Die Büronummer der Person.</span><span class="sxs-lookup"><span data-stu-id="021ab-147">The person's office number.</span></span>
| <span data-ttu-id="021ab-148">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="021ab-148">**pictureOnly36x36**</span></span>          | <span data-ttu-id="021ab-149">Das Bild der Person, begrenzt durch ein 36-x-36-px-Quadrat.</span><span class="sxs-lookup"><span data-stu-id="021ab-149">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="021ab-150">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="021ab-150">**pictureOnly48x48**</span></span>          | <span data-ttu-id="021ab-151">Das Bild der Person, begrenzt durch ein 48-x-48-px-Quadrat.</span><span class="sxs-lookup"><span data-stu-id="021ab-151">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="021ab-152">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="021ab-152">**pictureOnly72x72**</span></span>          | <span data-ttu-id="021ab-153">Das Bild der Person, begrenzt durch ein 72-x-72-px-Quadrat.</span><span class="sxs-lookup"><span data-stu-id="021ab-153">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="021ab-154">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="021ab-154">**sipAddress**</span></span>                | <span data-ttu-id="021ab-155">Die SIP-Adresse der Person.</span><span class="sxs-lookup"><span data-stu-id="021ab-155">The person's sip address.</span></span>
| <span data-ttu-id="021ab-156">**title**</span><span class="sxs-lookup"><span data-stu-id="021ab-156">**title**</span></span>                     | <span data-ttu-id="021ab-157">Titel der Person in der Organisation.</span><span class="sxs-lookup"><span data-stu-id="021ab-157">The person's title in the organization.</span></span>
| <span data-ttu-id="021ab-158">**userName**</span><span class="sxs-lookup"><span data-stu-id="021ab-158">**userName**</span></span>                  | <span data-ttu-id="021ab-159">Die Person oder der Benutzername der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="021ab-159">The person or group's user name.</span></span>
| <span data-ttu-id="021ab-160">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="021ab-160">**workEmail**</span></span>                 | <span data-ttu-id="021ab-161">Die Person oder die E-Mail-Adresse der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="021ab-161">The person or group's email address.</span></span>
| <span data-ttu-id="021ab-162">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="021ab-162">**workPhone**</span></span>                 | <span data-ttu-id="021ab-163">Die Telefonnummer bei der Arbeit der Person.</span><span class="sxs-lookup"><span data-stu-id="021ab-163">The person's work phone number.</span></span>

<span data-ttu-id="021ab-164">Hinweis: Möglicherweise werden weitere DisplayAs-Typen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="021ab-164">Note: Additional DisplayAs types may be returned.</span></span>

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
