---
author: simonhult
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: a3136d7c5b9563999eb9b21a9235317afdaeb63e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519297"
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="dd146-102">PersonOrGroupColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="dd146-102">PersonOrGroupColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd146-103">Die **personOrGroupColumn** zu einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass die Werte der Spalte eine aus dem Verzeichnis ausgewählte Person oder Gruppe darstellen.</span><span class="sxs-lookup"><span data-stu-id="dd146-103">The **personOrGroupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd146-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dd146-104">JSON representation</span></span>

<span data-ttu-id="dd146-105">Es folgt eine JSON-Darstellung einer **personOrGroupColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="dd146-105">Here is a JSON representation of a **personOrGroupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="dd146-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dd146-106">Properties</span></span>

| <span data-ttu-id="dd146-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="dd146-107">Property name</span></span>              | <span data-ttu-id="dd146-108">Typ</span><span class="sxs-lookup"><span data-stu-id="dd146-108">Type</span></span>    | <span data-ttu-id="dd146-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dd146-109">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="dd146-110">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="dd146-110">**allowMultipleSelection**</span></span> | <span data-ttu-id="dd146-111">boolean</span><span class="sxs-lookup"><span data-stu-id="dd146-111">boolean</span></span> | <span data-ttu-id="dd146-112">Gibt an, ob mehrere Werte aus der Quelle ausgewählt werden können.</span><span class="sxs-lookup"><span data-stu-id="dd146-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="dd146-113">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="dd146-113">**displayAs**</span></span>              | <span data-ttu-id="dd146-114">string</span><span class="sxs-lookup"><span data-stu-id="dd146-114">string</span></span>  | <span data-ttu-id="dd146-115">Informationen zum Anzeigen der Informationen zu der ausgewählten Person oder Gruppe.</span><span class="sxs-lookup"><span data-stu-id="dd146-115">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="dd146-116">Siehe unten.</span><span class="sxs-lookup"><span data-stu-id="dd146-116">See below.</span></span>
| <span data-ttu-id="dd146-117">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="dd146-117">**chooseFromType**</span></span>         | <span data-ttu-id="dd146-118">string</span><span class="sxs-lookup"><span data-stu-id="dd146-118">string</span></span>  | <span data-ttu-id="dd146-119">Gibt an, ob nur Personen oder Personen und Gruppen ausgewählt werden können.</span><span class="sxs-lookup"><span data-stu-id="dd146-119">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="dd146-120">Müssen `peopleAndGroups` oder `peopleOnly` sein.</span><span class="sxs-lookup"><span data-stu-id="dd146-120">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-values"></a><span data-ttu-id="dd146-121">DisplayAs-Werte</span><span class="sxs-lookup"><span data-stu-id="dd146-121">DisplayAs values</span></span>

| <span data-ttu-id="dd146-122">DisplayAs-Wert</span><span class="sxs-lookup"><span data-stu-id="dd146-122">DisplayAs value</span></span>               | <span data-ttu-id="dd146-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dd146-123">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="dd146-124">**account**</span><span class="sxs-lookup"><span data-stu-id="dd146-124">**account**</span></span>                   | <span data-ttu-id="dd146-125">Die rohe SharePoint-codierte Anforderungszeichenfolge für die Person oder Gruppe (z. B.</span><span class="sxs-lookup"><span data-stu-id="dd146-125">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="dd146-126">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="dd146-126">i:0#.f</span></span>|<span data-ttu-id="dd146-127">Mitgliedschaft</span><span class="sxs-lookup"><span data-stu-id="dd146-127">membership</span></span>|<span data-ttu-id="dd146-128">jane@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="dd146-128">jane@contoso.com).</span></span>
| <span data-ttu-id="dd146-129">**department**</span><span class="sxs-lookup"><span data-stu-id="dd146-129">**department**</span></span>                | <span data-ttu-id="dd146-130">Die Abteilung der Person oder Gruppe.</span><span class="sxs-lookup"><span data-stu-id="dd146-130">The person or group's department.</span></span>
| <span data-ttu-id="dd146-131">**firstName**</span><span class="sxs-lookup"><span data-stu-id="dd146-131">**firstName**</span></span>                 | <span data-ttu-id="dd146-132">The person's first name.</span><span class="sxs-lookup"><span data-stu-id="dd146-132">The person's first name.</span></span>
| <span data-ttu-id="dd146-133">**id**</span><span class="sxs-lookup"><span data-stu-id="dd146-133">**id**</span></span>                        | <span data-ttu-id="dd146-134">Die ID der Person oder Gruppe im Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="dd146-134">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="dd146-135">**lastName**</span><span class="sxs-lookup"><span data-stu-id="dd146-135">**lastName**</span></span>                  | <span data-ttu-id="dd146-136">Der Nachname der Person.</span><span class="sxs-lookup"><span data-stu-id="dd146-136">The person's last name.</span></span>
| <span data-ttu-id="dd146-137">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="dd146-137">**mobilePhone**</span></span>               | <span data-ttu-id="dd146-138">Die Mobiltelefonnummer der Person.</span><span class="sxs-lookup"><span data-stu-id="dd146-138">The person's mobile phone number.</span></span>
| <span data-ttu-id="dd146-139">**name**</span><span class="sxs-lookup"><span data-stu-id="dd146-139">**name**</span></span>                      | <span data-ttu-id="dd146-140">Der Name der Person.</span><span class="sxs-lookup"><span data-stu-id="dd146-140">The person's name.</span></span>
| <span data-ttu-id="dd146-141">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="dd146-141">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="dd146-142">Der Name der Person mit ihrem Bild und zusätzlichen Details.</span><span class="sxs-lookup"><span data-stu-id="dd146-142">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="dd146-143">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="dd146-143">**nameWithPresence**</span></span>          | <span data-ttu-id="dd146-144">Standard.</span><span class="sxs-lookup"><span data-stu-id="dd146-144">Default.</span></span> <span data-ttu-id="dd146-145">Der Name der Person mit einem Anwesenheitssymbol (verfügbar/beschäftigt/usw.).</span><span class="sxs-lookup"><span data-stu-id="dd146-145">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="dd146-146">**office**</span><span class="sxs-lookup"><span data-stu-id="dd146-146">**office**</span></span>                    | <span data-ttu-id="dd146-147">Die Büronummer der Person.</span><span class="sxs-lookup"><span data-stu-id="dd146-147">The person's office number.</span></span>
| <span data-ttu-id="dd146-148">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="dd146-148">**pictureOnly36x36**</span></span>          | <span data-ttu-id="dd146-149">Das Bild der Person, begrenzt durch ein 36-x-36-px-Quadrat.</span><span class="sxs-lookup"><span data-stu-id="dd146-149">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="dd146-150">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="dd146-150">**pictureOnly48x48**</span></span>          | <span data-ttu-id="dd146-151">Das Bild der Person, begrenzt durch ein 48-x-48-px-Quadrat.</span><span class="sxs-lookup"><span data-stu-id="dd146-151">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="dd146-152">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="dd146-152">**pictureOnly72x72**</span></span>          | <span data-ttu-id="dd146-153">Das Bild der Person, begrenzt durch ein 72-x-72-px-Quadrat.</span><span class="sxs-lookup"><span data-stu-id="dd146-153">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="dd146-154">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="dd146-154">**sipAddress**</span></span>                | <span data-ttu-id="dd146-155">Die SIP-Adresse der Person.</span><span class="sxs-lookup"><span data-stu-id="dd146-155">The person's sip address.</span></span>
| <span data-ttu-id="dd146-156">**title**</span><span class="sxs-lookup"><span data-stu-id="dd146-156">**title**</span></span>                     | <span data-ttu-id="dd146-157">Titel der Person in der Organisation.</span><span class="sxs-lookup"><span data-stu-id="dd146-157">The person's title in the organization.</span></span>
| <span data-ttu-id="dd146-158">**userName**</span><span class="sxs-lookup"><span data-stu-id="dd146-158">**userName**</span></span>                  | <span data-ttu-id="dd146-159">Die Person oder der Benutzername der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="dd146-159">The person or group's user name.</span></span>
| <span data-ttu-id="dd146-160">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="dd146-160">**workEmail**</span></span>                 | <span data-ttu-id="dd146-161">Die Person oder die E-Mail-Adresse der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="dd146-161">The person or group's email address.</span></span>
| <span data-ttu-id="dd146-162">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="dd146-162">**workPhone**</span></span>                 | <span data-ttu-id="dd146-163">Die Telefonnummer bei der Arbeit der Person.</span><span class="sxs-lookup"><span data-stu-id="dd146-163">The person's work phone number.</span></span>

<span data-ttu-id="dd146-164">Hinweis: Möglicherweise werden weitere DisplayAs-Typen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dd146-164">Note: Additional DisplayAs types may be returned.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/PersonOrGroupColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/personOrGroupColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
