---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.openlocfilehash: bd75d9e112ff67e455cae07791ab3284861d5b72
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874172"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="e2b68-102">PersonOrGroupColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e2b68-102">PersonOrGroupColumn resource type</span></span>

> <span data-ttu-id="e2b68-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e2b68-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2b68-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e2b68-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e2b68-105">Die **personOrGroupColumn** zu einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass die Werte der Spalte eine aus dem Verzeichnis ausgewählte Person oder Gruppe darstellen.</span><span class="sxs-lookup"><span data-stu-id="e2b68-105">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2b68-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e2b68-106">JSON representation</span></span>

<span data-ttu-id="e2b68-107">Es folgt eine JSON-Darstellung einer **personOrGroupColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="e2b68-107">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="e2b68-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e2b68-108">Properties</span></span>

| <span data-ttu-id="e2b68-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="e2b68-109">Property name</span></span>              | <span data-ttu-id="e2b68-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e2b68-110">Type</span></span>    | <span data-ttu-id="e2b68-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e2b68-111">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="e2b68-112">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="e2b68-112">**allowMultipleSelection**</span></span> | <span data-ttu-id="e2b68-113">boolean</span><span class="sxs-lookup"><span data-stu-id="e2b68-113">boolean</span></span> | <span data-ttu-id="e2b68-114">Gibt an, ob mehrere Werte aus der Quelle ausgewählt werden können.</span><span class="sxs-lookup"><span data-stu-id="e2b68-114">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="e2b68-115">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="e2b68-115">**displayAs**</span></span>              | <span data-ttu-id="e2b68-116">string</span><span class="sxs-lookup"><span data-stu-id="e2b68-116">string</span></span>  | <span data-ttu-id="e2b68-117">Informationen zum Anzeigen der Informationen zu der ausgewählten Person oder Gruppe.</span><span class="sxs-lookup"><span data-stu-id="e2b68-117">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="e2b68-118">Siehe unten.</span><span class="sxs-lookup"><span data-stu-id="e2b68-118">See below.</span></span>
| <span data-ttu-id="e2b68-119">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="e2b68-119">**chooseFromType**</span></span>         | <span data-ttu-id="e2b68-120">string</span><span class="sxs-lookup"><span data-stu-id="e2b68-120">string</span></span>  | <span data-ttu-id="e2b68-121">Gibt an, ob nur Personen oder Personen und Gruppen ausgewählt werden können.</span><span class="sxs-lookup"><span data-stu-id="e2b68-121">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="e2b68-122">Müssen `peopleAndGroups` oder `peopleOnly` sein.</span><span class="sxs-lookup"><span data-stu-id="e2b68-122">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-values"></a><span data-ttu-id="e2b68-123">DisplayAs-Werte</span><span class="sxs-lookup"><span data-stu-id="e2b68-123">DisplayAs values</span></span>

| <span data-ttu-id="e2b68-124">DisplayAs-Wert</span><span class="sxs-lookup"><span data-stu-id="e2b68-124">DisplayAs value</span></span>               | <span data-ttu-id="e2b68-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e2b68-125">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="e2b68-126">**account**</span><span class="sxs-lookup"><span data-stu-id="e2b68-126">**account**</span></span>                   | <span data-ttu-id="e2b68-127">Die rohe SharePoint-codierte Anforderungszeichenfolge für die Person oder Gruppe (z. B.</span><span class="sxs-lookup"><span data-stu-id="e2b68-127">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="e2b68-128">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="e2b68-128">i:0#.f</span></span>|<span data-ttu-id="e2b68-129">Mitgliedschaft</span><span class="sxs-lookup"><span data-stu-id="e2b68-129">membership</span></span>|<span data-ttu-id="e2b68-130">jane@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="e2b68-130">jane@contoso.com).</span></span>
| <span data-ttu-id="e2b68-131">**department**</span><span class="sxs-lookup"><span data-stu-id="e2b68-131">**department**</span></span>                | <span data-ttu-id="e2b68-132">Die Abteilung der Person oder Gruppe.</span><span class="sxs-lookup"><span data-stu-id="e2b68-132">The person or group's department.</span></span>
| <span data-ttu-id="e2b68-133">**firstName**</span><span class="sxs-lookup"><span data-stu-id="e2b68-133">**firstName**</span></span>                 | <span data-ttu-id="e2b68-134">The person's first name.</span><span class="sxs-lookup"><span data-stu-id="e2b68-134">The person's first name.</span></span>
| <span data-ttu-id="e2b68-135">**id**</span><span class="sxs-lookup"><span data-stu-id="e2b68-135">**id**</span></span>                        | <span data-ttu-id="e2b68-136">Die ID der Person oder Gruppe im Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="e2b68-136">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="e2b68-137">**lastName**</span><span class="sxs-lookup"><span data-stu-id="e2b68-137">**lastName**</span></span>                  | <span data-ttu-id="e2b68-138">Der Nachname der Person.</span><span class="sxs-lookup"><span data-stu-id="e2b68-138">The person's last name.</span></span>
| <span data-ttu-id="e2b68-139">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="e2b68-139">**mobilePhone**</span></span>               | <span data-ttu-id="e2b68-140">Die Mobiltelefonnummer der Person.</span><span class="sxs-lookup"><span data-stu-id="e2b68-140">The person's mobile phone number.</span></span>
| <span data-ttu-id="e2b68-141">**name**</span><span class="sxs-lookup"><span data-stu-id="e2b68-141">**name**</span></span>                      | <span data-ttu-id="e2b68-142">Der Name der Person.</span><span class="sxs-lookup"><span data-stu-id="e2b68-142">The person's name.</span></span>
| <span data-ttu-id="e2b68-143">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="e2b68-143">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="e2b68-144">Der Name der Person mit ihrem Bild und zusätzlichen Details.</span><span class="sxs-lookup"><span data-stu-id="e2b68-144">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="e2b68-145">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="e2b68-145">**nameWithPresence**</span></span>          | <span data-ttu-id="e2b68-146">Standard.</span><span class="sxs-lookup"><span data-stu-id="e2b68-146">Default.</span></span> <span data-ttu-id="e2b68-147">Der Name der Person mit einem Anwesenheitssymbol (verfügbar/beschäftigt/usw.).</span><span class="sxs-lookup"><span data-stu-id="e2b68-147">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="e2b68-148">**office**</span><span class="sxs-lookup"><span data-stu-id="e2b68-148">**office**</span></span>                    | <span data-ttu-id="e2b68-149">Die Büronummer der Person.</span><span class="sxs-lookup"><span data-stu-id="e2b68-149">The person's office number.</span></span>
| <span data-ttu-id="e2b68-150">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="e2b68-150">**pictureOnly36x36**</span></span>          | <span data-ttu-id="e2b68-151">Das Bild der Person, begrenzt durch ein 36-x-36-px-Quadrat.</span><span class="sxs-lookup"><span data-stu-id="e2b68-151">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="e2b68-152">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="e2b68-152">**pictureOnly48x48**</span></span>          | <span data-ttu-id="e2b68-153">Das Bild der Person, begrenzt durch ein 48-x-48-px-Quadrat.</span><span class="sxs-lookup"><span data-stu-id="e2b68-153">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="e2b68-154">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="e2b68-154">**pictureOnly72x72**</span></span>          | <span data-ttu-id="e2b68-155">Das Bild der Person, begrenzt durch ein 72-x-72-px-Quadrat.</span><span class="sxs-lookup"><span data-stu-id="e2b68-155">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="e2b68-156">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="e2b68-156">**sipAddress**</span></span>                | <span data-ttu-id="e2b68-157">Die SIP-Adresse der Person.</span><span class="sxs-lookup"><span data-stu-id="e2b68-157">The person's sip address.</span></span>
| <span data-ttu-id="e2b68-158">**title**</span><span class="sxs-lookup"><span data-stu-id="e2b68-158">**title**</span></span>                     | <span data-ttu-id="e2b68-159">Titel der Person in der Organisation.</span><span class="sxs-lookup"><span data-stu-id="e2b68-159">The person's title in the organization.</span></span>
| <span data-ttu-id="e2b68-160">**userName**</span><span class="sxs-lookup"><span data-stu-id="e2b68-160">**userName**</span></span>                  | <span data-ttu-id="e2b68-161">Die Person oder der Benutzername der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="e2b68-161">The person or group's user name.</span></span>
| <span data-ttu-id="e2b68-162">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="e2b68-162">**workEmail**</span></span>                 | <span data-ttu-id="e2b68-163">Die Person oder die E-Mail-Adresse der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="e2b68-163">The person or group's email address.</span></span>
| <span data-ttu-id="e2b68-164">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="e2b68-164">**workPhone**</span></span>                 | <span data-ttu-id="e2b68-165">Die Telefonnummer bei der Arbeit der Person.</span><span class="sxs-lookup"><span data-stu-id="e2b68-165">The person's work phone number.</span></span>

<span data-ttu-id="e2b68-166">Hinweis: Möglicherweise werden weitere DisplayAs-Typen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e2b68-166">Note: Additional DisplayAs types may be returned.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/PersonOrGroupColumn"
} -->
