---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: PersonOrGroupColumn
ms.openlocfilehash: 715c6ca22957cbd951784e6cf32edf2bf47f1098
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="personorgroupcolumn-resource-type"></a><span data-ttu-id="1c917-102">PersonOrGroupColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1c917-102">PersonOrGroupColumn resource type</span></span>

<span data-ttu-id="1c917-103">Die **personOrGroupColumn** zu einer [columnDefinition](columnDefinition.md)-Ressource gibt an, dass die Werte der Spalte eine aus dem Verzeichnis ausgewählte Person oder Gruppe darstellen.</span><span class="sxs-lookup"><span data-stu-id="1c917-103">The **personOrGroupColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values represent a person or group chosen from the directory.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c917-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1c917-104">JSON representation</span></span>

<span data-ttu-id="1c917-105">Es folgt eine JSON-Darstellung einer **personOrGroupColumn**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="1c917-105">Here is a JSON representation of a **drive** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a><span data-ttu-id="1c917-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1c917-106">Properties</span></span>

| <span data-ttu-id="1c917-107">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="1c917-107">Property name</span></span>              | <span data-ttu-id="1c917-108">Typ</span><span class="sxs-lookup"><span data-stu-id="1c917-108">Type</span></span>    | <span data-ttu-id="1c917-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1c917-109">Description</span></span>
|:---------------------------|:--------|:--------------------------------------
| <span data-ttu-id="1c917-110">**allowMultipleSelection**</span><span class="sxs-lookup"><span data-stu-id="1c917-110">**allowMultipleSelection**</span></span> | <span data-ttu-id="1c917-111">boolean</span><span class="sxs-lookup"><span data-stu-id="1c917-111">boolean</span></span> | <span data-ttu-id="1c917-112">Gibt an, ob mehrere Werte aus der Quelle ausgewählt werden können.</span><span class="sxs-lookup"><span data-stu-id="1c917-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="1c917-113">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="1c917-113">**displayAs**</span></span>              | <span data-ttu-id="1c917-114">string</span><span class="sxs-lookup"><span data-stu-id="1c917-114">string</span></span>  | <span data-ttu-id="1c917-115">Informationen zum Anzeigen der Informationen zu der ausgewählten Person oder Gruppe.</span><span class="sxs-lookup"><span data-stu-id="1c917-115">How to display the information about the person or group chosen.</span></span> <span data-ttu-id="1c917-116">Siehe unten.</span><span class="sxs-lookup"><span data-stu-id="1c917-116">See below.</span></span>
| <span data-ttu-id="1c917-117">**chooseFromType**</span><span class="sxs-lookup"><span data-stu-id="1c917-117">**chooseFromType**</span></span>         | <span data-ttu-id="1c917-118">string</span><span class="sxs-lookup"><span data-stu-id="1c917-118">string</span></span>  | <span data-ttu-id="1c917-119">Gibt an, ob nur Personen oder Personen und Gruppen ausgewählt werden können.</span><span class="sxs-lookup"><span data-stu-id="1c917-119">Whether to allow selection of people only, or people and groups.</span></span> <span data-ttu-id="1c917-120">Müssen `peopleAndGroups` oder `peopleOnly` sein.</span><span class="sxs-lookup"><span data-stu-id="1c917-120">Must be one of `peopleAndGroups` or `peopleOnly`.</span></span>

## <a name="displayas-values"></a><span data-ttu-id="1c917-121">DisplayAs-Werte</span><span class="sxs-lookup"><span data-stu-id="1c917-121">DisplayAs values</span></span>

| <span data-ttu-id="1c917-122">DisplayAs-Wert</span><span class="sxs-lookup"><span data-stu-id="1c917-122">DisplayAs value</span></span>               | <span data-ttu-id="1c917-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1c917-123">Description</span></span>
|:------------------------------|:-----------------------
| <span data-ttu-id="1c917-124">**account**</span><span class="sxs-lookup"><span data-stu-id="1c917-124">**Account**</span></span>                   | <span data-ttu-id="1c917-125">Die rohe SharePoint-codierte Anforderungszeichenfolge für die Person oder Gruppe (z. B.</span><span class="sxs-lookup"><span data-stu-id="1c917-125">The raw SharePoint encoded claim string for the person or group (eg.</span></span> <span data-ttu-id="1c917-126">i:0#.f</span><span class="sxs-lookup"><span data-stu-id="1c917-126">i:0#.f</span></span>|<span data-ttu-id="1c917-127">Mitgliedschaft</span><span class="sxs-lookup"><span data-stu-id="1c917-127">membership</span></span>|<span data-ttu-id="1c917-128">jane@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="1c917-128">jane@contoso.com).</span></span>
| <span data-ttu-id="1c917-129">**department**</span><span class="sxs-lookup"><span data-stu-id="1c917-129">**department**</span></span>                | <span data-ttu-id="1c917-130">Die Abteilung der Person oder Gruppe.</span><span class="sxs-lookup"><span data-stu-id="1c917-130">The person or group's department.</span></span>
| <span data-ttu-id="1c917-131">**firstName**</span><span class="sxs-lookup"><span data-stu-id="1c917-131">**FirstName**</span></span>                 | <span data-ttu-id="1c917-132">The person's first name.</span><span class="sxs-lookup"><span data-stu-id="1c917-132">The person's given name.</span></span>
| <span data-ttu-id="1c917-133">**id**</span><span class="sxs-lookup"><span data-stu-id="1c917-133">**id**</span></span>                        | <span data-ttu-id="1c917-134">Die ID der Person oder Gruppe im Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="1c917-134">The id of the person or group in the directory.</span></span>
| <span data-ttu-id="1c917-135">**lastName**</span><span class="sxs-lookup"><span data-stu-id="1c917-135">**LastName**</span></span>                  | <span data-ttu-id="1c917-136">Der Nachname der Person.</span><span class="sxs-lookup"><span data-stu-id="1c917-136">The person's given name.</span></span>
| <span data-ttu-id="1c917-137">**mobilePhone**</span><span class="sxs-lookup"><span data-stu-id="1c917-137">**mobilePhone**</span></span>               | <span data-ttu-id="1c917-138">Die Mobiltelefonnummer der Person.</span><span class="sxs-lookup"><span data-stu-id="1c917-138">The contact's mobile phone number.</span></span>
| <span data-ttu-id="1c917-139">**name**</span><span class="sxs-lookup"><span data-stu-id="1c917-139">**name**</span></span>                      | <span data-ttu-id="1c917-140">Der Name der Person.</span><span class="sxs-lookup"><span data-stu-id="1c917-140">The person's given name.</span></span>
| <span data-ttu-id="1c917-141">**nameWithPictureAndDetails**</span><span class="sxs-lookup"><span data-stu-id="1c917-141">**nameWithPictureAndDetails**</span></span> | <span data-ttu-id="1c917-142">Der Name der Person mit ihrem Bild und zusätzlichen Details.</span><span class="sxs-lookup"><span data-stu-id="1c917-142">The person's name along with their picture and additional details.</span></span>
| <span data-ttu-id="1c917-143">**nameWithPresence**</span><span class="sxs-lookup"><span data-stu-id="1c917-143">**nameWithPresence**</span></span>          | <span data-ttu-id="1c917-144">Standard.</span><span class="sxs-lookup"><span data-stu-id="1c917-144">Default.</span></span> <span data-ttu-id="1c917-145">Der Name der Person mit einem Anwesenheitssymbol (verfügbar/beschäftigt/usw.).</span><span class="sxs-lookup"><span data-stu-id="1c917-145">The person's name with a presence indicator icon (available/busy/etc.)</span></span>
| <span data-ttu-id="1c917-146">**office**</span><span class="sxs-lookup"><span data-stu-id="1c917-146">**Office**</span></span>                    | <span data-ttu-id="1c917-147">Die Büronummer der Person.</span><span class="sxs-lookup"><span data-stu-id="1c917-147">The person's office number.</span></span>
| <span data-ttu-id="1c917-148">**pictureOnly36x36**</span><span class="sxs-lookup"><span data-stu-id="1c917-148">**pictureOnly36x36**</span></span>          | <span data-ttu-id="1c917-149">Das Bild der Person, begrenzt durch ein 36-x-36-px-Quadrat.</span><span class="sxs-lookup"><span data-stu-id="1c917-149">The person's picture, bounded by a 36x36 px square.</span></span>
| <span data-ttu-id="1c917-150">**pictureOnly48x48**</span><span class="sxs-lookup"><span data-stu-id="1c917-150">**pictureOnly48x48**</span></span>          | <span data-ttu-id="1c917-151">Das Bild der Person, begrenzt durch ein 48-x-48-px-Quadrat.</span><span class="sxs-lookup"><span data-stu-id="1c917-151">The person's picture, bounded by a 48x48 px square.</span></span>
| <span data-ttu-id="1c917-152">**pictureOnly72x72**</span><span class="sxs-lookup"><span data-stu-id="1c917-152">**pictureOnly72x72**</span></span>          | <span data-ttu-id="1c917-153">Das Bild der Person, begrenzt durch ein 72-x-72-px-Quadrat.</span><span class="sxs-lookup"><span data-stu-id="1c917-153">The person's picture, bounded by a 72x72 px square.</span></span>
| <span data-ttu-id="1c917-154">**sipAddress**</span><span class="sxs-lookup"><span data-stu-id="1c917-154">**sipAddress**</span></span>                | <span data-ttu-id="1c917-155">Die SIP-Adresse der Person.</span><span class="sxs-lookup"><span data-stu-id="1c917-155">The person's sip address.</span></span>
| <span data-ttu-id="1c917-156">**title**</span><span class="sxs-lookup"><span data-stu-id="1c917-156">**title**</span></span>                     | <span data-ttu-id="1c917-157">Titel der Person in der Organisation.</span><span class="sxs-lookup"><span data-stu-id="1c917-157">The person's title in the organization.</span></span>
| <span data-ttu-id="1c917-158">**userName**</span><span class="sxs-lookup"><span data-stu-id="1c917-158">**Username**</span></span>                  | <span data-ttu-id="1c917-159">Die Person oder der Benutzername der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="1c917-159">The person or group's user name.</span></span>
| <span data-ttu-id="1c917-160">**workEmail**</span><span class="sxs-lookup"><span data-stu-id="1c917-160">**workEmail**</span></span>                 | <span data-ttu-id="1c917-161">Die Person oder die E-Mail-Adresse der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="1c917-161">The person or group's email address.</span></span>
| <span data-ttu-id="1c917-162">**workPhone**</span><span class="sxs-lookup"><span data-stu-id="1c917-162">**workPhone**</span></span>                 | <span data-ttu-id="1c917-163">Die Telefonnummer bei der Arbeit der Person.</span><span class="sxs-lookup"><span data-stu-id="1c917-163">The person's work phone number.</span></span>

<span data-ttu-id="1c917-164">Hinweis: Möglicherweise werden weitere DisplayAs-Typen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1c917-164">Note: Additional DisplayAs types may be returned.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/PersonOrGroupColumn"
} -->
