---
title: educationSchool-Ressourcentyp
description: 'Eine Bildungseinrichtung. Die **educationSchool**-Ressource entspricht derzeit einer administrativeUnit-Ressource und hat dieselbe ID.  '
localization_priority: Normal
ms.openlocfilehash: 20eacb87b68cbf490131b98a15d3ab3239d73478
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830450"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="df9fb-104">educationSchool-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="df9fb-104">educationSchool resource type</span></span>

> <span data-ttu-id="df9fb-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="df9fb-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df9fb-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="df9fb-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="df9fb-107">Eine Bildungseinrichtung.</span><span class="sxs-lookup"><span data-stu-id="df9fb-107">A school.</span></span> <span data-ttu-id="df9fb-108">Die **educationSchool**-Ressource entspricht derzeit einer [administrativeUnit](administrativeunit.md)-Ressource und hat dieselbe ID.</span><span class="sxs-lookup"><span data-stu-id="df9fb-108">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>  

<span data-ttu-id="df9fb-109">Diese Ressource ist ein Untertyp von [educationOrganization](educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="df9fb-109">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>




## <a name="methods"></a><span data-ttu-id="df9fb-110">Methoden</span><span class="sxs-lookup"><span data-stu-id="df9fb-110">Methods</span></span>

| <span data-ttu-id="df9fb-111">Methode</span><span class="sxs-lookup"><span data-stu-id="df9fb-111">Method</span></span>           | <span data-ttu-id="df9fb-112">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="df9fb-112">Return Type</span></span>    |<span data-ttu-id="df9fb-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df9fb-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="df9fb-114">Get</span><span class="sxs-lookup"><span data-stu-id="df9fb-114">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="df9fb-115">educationSchool</span><span class="sxs-lookup"><span data-stu-id="df9fb-115">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="df9fb-116">Lesen von Eigenschaften und Beziehungen eines **educationSchool**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="df9fb-116">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="df9fb-117">Klasse hinzufügen</span><span class="sxs-lookup"><span data-stu-id="df9fb-117">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="df9fb-118">educationClass</span><span class="sxs-lookup"><span data-stu-id="df9fb-118">educationClass</span></span>](educationclass.md)| <span data-ttu-id="df9fb-119">Hinzufügen einer neuen **educationClass** für die Schule durch Bereitstellen in der Navigationseigenschaft „classes“.</span><span class="sxs-lookup"><span data-stu-id="df9fb-119">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="df9fb-120">Klassen auflisten</span><span class="sxs-lookup"><span data-stu-id="df9fb-120">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="df9fb-121">[educationClass](educationclass.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="df9fb-121">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="df9fb-122">Abrufen der **educationClass**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="df9fb-122">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="df9fb-123">Klasse entfernen</span><span class="sxs-lookup"><span data-stu-id="df9fb-123">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="df9fb-124">educationClass</span><span class="sxs-lookup"><span data-stu-id="df9fb-124">educationClass</span></span>](educationclass.md)| <span data-ttu-id="df9fb-125">Entfernen einer **educationClass** von der Schule über die Navigationseigenschaft „classes“.</span><span class="sxs-lookup"><span data-stu-id="df9fb-125">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="df9fb-126">Benutzer hinzufügen</span><span class="sxs-lookup"><span data-stu-id="df9fb-126">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="df9fb-127">educationUser</span><span class="sxs-lookup"><span data-stu-id="df9fb-127">educationUser</span></span>](educationuser.md)| <span data-ttu-id="df9fb-128">Hinzufügen eines neuen **educationUser** für die Schule durch Bereitstellen in der Navigationseigenschaft **users**.</span><span class="sxs-lookup"><span data-stu-id="df9fb-128">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="df9fb-129">Benutzer auflisten</span><span class="sxs-lookup"><span data-stu-id="df9fb-129">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="df9fb-130">[educationUser](educationuser.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="df9fb-130">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="df9fb-131">Abrufen der **educationUser**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="df9fb-131">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="df9fb-132">Benutzer entfernen</span><span class="sxs-lookup"><span data-stu-id="df9fb-132">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="df9fb-133">educationUser</span><span class="sxs-lookup"><span data-stu-id="df9fb-133">educationUser</span></span>](educationuser.md)| <span data-ttu-id="df9fb-134">Entfernen eines **educationUser** von der Schule über die Navigationseigenschaft **users**.</span><span class="sxs-lookup"><span data-stu-id="df9fb-134">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="df9fb-135">AdministrativeUnit abrufen</span><span class="sxs-lookup"><span data-stu-id="df9fb-135">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) |[<span data-ttu-id="df9fb-136">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="df9fb-136">administrativeUnit</span></span>](administrativeunit.md)| <span data-ttu-id="df9fb-137">Abrufen der **administrativeUnit**, die dieser **educationSchool** entspricht.</span><span class="sxs-lookup"><span data-stu-id="df9fb-137">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>|
|[<span data-ttu-id="df9fb-138">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="df9fb-138">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="df9fb-139">educationSchool</span><span class="sxs-lookup"><span data-stu-id="df9fb-139">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="df9fb-140">Aktualisieren eines **educationSchool**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="df9fb-140">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="df9fb-141">Löschen</span><span class="sxs-lookup"><span data-stu-id="df9fb-141">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="df9fb-142">Keine</span><span class="sxs-lookup"><span data-stu-id="df9fb-142">None</span></span> |<span data-ttu-id="df9fb-143">Löschen eines **educationSchool**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="df9fb-143">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="df9fb-144">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="df9fb-144">Properties</span></span>
| <span data-ttu-id="df9fb-145">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="df9fb-145">Property</span></span>     | <span data-ttu-id="df9fb-146">Typ</span><span class="sxs-lookup"><span data-stu-id="df9fb-146">Type</span></span>   |<span data-ttu-id="df9fb-147">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df9fb-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df9fb-148">id</span><span class="sxs-lookup"><span data-stu-id="df9fb-148">id</span></span>|<span data-ttu-id="df9fb-149">String</span><span class="sxs-lookup"><span data-stu-id="df9fb-149">String</span></span>|<span data-ttu-id="df9fb-150">GUID dieser Schule</span><span class="sxs-lookup"><span data-stu-id="df9fb-150">GUID of this school.</span></span>|
|<span data-ttu-id="df9fb-151">displayName</span><span class="sxs-lookup"><span data-stu-id="df9fb-151">displayName</span></span>| <span data-ttu-id="df9fb-152">String</span><span class="sxs-lookup"><span data-stu-id="df9fb-152">String</span></span>| <span data-ttu-id="df9fb-153">Anzeigename der Schule</span><span class="sxs-lookup"><span data-stu-id="df9fb-153">Display name of the school.</span></span>| 
|<span data-ttu-id="df9fb-154">description</span><span class="sxs-lookup"><span data-stu-id="df9fb-154">description</span></span>| <span data-ttu-id="df9fb-155">String</span><span class="sxs-lookup"><span data-stu-id="df9fb-155">String</span></span> | <span data-ttu-id="df9fb-156">Beschreibung der Schule</span><span class="sxs-lookup"><span data-stu-id="df9fb-156">Description of the school.</span></span>| 
|<span data-ttu-id="df9fb-157">status</span><span class="sxs-lookup"><span data-stu-id="df9fb-157">status</span></span>| <span data-ttu-id="df9fb-158">string</span><span class="sxs-lookup"><span data-stu-id="df9fb-158">string</span></span>| <span data-ttu-id="df9fb-159">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="df9fb-159">Read-Only.</span></span> <span data-ttu-id="df9fb-160">Mögliche Werte: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="df9fb-160">Possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="df9fb-161">externalSource</span><span class="sxs-lookup"><span data-stu-id="df9fb-161">externalSource</span></span>| <span data-ttu-id="df9fb-162">string</span><span class="sxs-lookup"><span data-stu-id="df9fb-162">string</span></span>| <span data-ttu-id="df9fb-163">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="df9fb-163">Read-Only.</span></span>  <span data-ttu-id="df9fb-164">Mögliche Werte sind: `sis`, `manual` und `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="df9fb-164">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="df9fb-165">principalEmail</span><span class="sxs-lookup"><span data-stu-id="df9fb-165">principalEmail</span></span>| <span data-ttu-id="df9fb-166">String</span><span class="sxs-lookup"><span data-stu-id="df9fb-166">String</span></span>| <span data-ttu-id="df9fb-167">Die E-Mail-Adresse des Prinzipals</span><span class="sxs-lookup"><span data-stu-id="df9fb-167">Email address of the principal.</span></span>|
|<span data-ttu-id="df9fb-168">principalName</span><span class="sxs-lookup"><span data-stu-id="df9fb-168">principalName</span></span>| <span data-ttu-id="df9fb-169">String</span><span class="sxs-lookup"><span data-stu-id="df9fb-169">String</span></span> | <span data-ttu-id="df9fb-170">Der Name des Prinzipals</span><span class="sxs-lookup"><span data-stu-id="df9fb-170">Name of the principal.</span></span>|
|<span data-ttu-id="df9fb-171">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="df9fb-171">externalPrincipalId</span></span>| <span data-ttu-id="df9fb-172">String</span><span class="sxs-lookup"><span data-stu-id="df9fb-172">String</span></span> | <span data-ttu-id="df9fb-173">Die ID des Prinzipals im Synchronisierungssystem</span><span class="sxs-lookup"><span data-stu-id="df9fb-173">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="df9fb-174">highestGrade</span><span class="sxs-lookup"><span data-stu-id="df9fb-174">highestGrade</span></span>|<span data-ttu-id="df9fb-175">String</span><span class="sxs-lookup"><span data-stu-id="df9fb-175">String</span></span>| <span data-ttu-id="df9fb-176">Höchste unterrichtete Klasse</span><span class="sxs-lookup"><span data-stu-id="df9fb-176">Highest grade taught.</span></span> |
|<span data-ttu-id="df9fb-177">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="df9fb-177">lowestGrade</span></span>|<span data-ttu-id="df9fb-178">String</span><span class="sxs-lookup"><span data-stu-id="df9fb-178">String</span></span>| <span data-ttu-id="df9fb-179">Niedrigste unterrichtete Klasse</span><span class="sxs-lookup"><span data-stu-id="df9fb-179">Lowest grade taught.</span></span> |
|<span data-ttu-id="df9fb-180">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="df9fb-180">schoolNumber</span></span>|<span data-ttu-id="df9fb-181">String</span><span class="sxs-lookup"><span data-stu-id="df9fb-181">String</span></span>| <span data-ttu-id="df9fb-182">Schulnummer</span><span class="sxs-lookup"><span data-stu-id="df9fb-182">School Number.</span></span>|
|<span data-ttu-id="df9fb-183">externalId</span><span class="sxs-lookup"><span data-stu-id="df9fb-183">externalId</span></span>|<span data-ttu-id="df9fb-184">String</span><span class="sxs-lookup"><span data-stu-id="df9fb-184">String</span></span>| <span data-ttu-id="df9fb-185">Die ID der Schule im Synchronisierungssystem</span><span class="sxs-lookup"><span data-stu-id="df9fb-185">ID of school in syncing system.</span></span> |
|<span data-ttu-id="df9fb-186">phone</span><span class="sxs-lookup"><span data-stu-id="df9fb-186">phone</span></span>|<span data-ttu-id="df9fb-187">String</span><span class="sxs-lookup"><span data-stu-id="df9fb-187">String</span></span>| <span data-ttu-id="df9fb-188">Die Telefonnummer der Schule</span><span class="sxs-lookup"><span data-stu-id="df9fb-188">Phone number of school.</span></span> |
|<span data-ttu-id="df9fb-189">fax</span><span class="sxs-lookup"><span data-stu-id="df9fb-189">fax</span></span>|<span data-ttu-id="df9fb-190">String</span><span class="sxs-lookup"><span data-stu-id="df9fb-190">String</span></span>| <span data-ttu-id="df9fb-191">Die Faxnummer der Schule</span><span class="sxs-lookup"><span data-stu-id="df9fb-191">Fax number of school.</span></span> |
|<span data-ttu-id="df9fb-192">address</span><span class="sxs-lookup"><span data-stu-id="df9fb-192">address</span></span>|[<span data-ttu-id="df9fb-193">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="df9fb-193">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="df9fb-194">Die Adresse der Schule</span><span class="sxs-lookup"><span data-stu-id="df9fb-194">Address of the school.</span></span>|
|<span data-ttu-id="df9fb-195">createdBy</span><span class="sxs-lookup"><span data-stu-id="df9fb-195">createdBy</span></span>|[<span data-ttu-id="df9fb-196">identitySet</span><span class="sxs-lookup"><span data-stu-id="df9fb-196">identitySet</span></span>](identityset.md)|<span data-ttu-id="df9fb-197">Entität, die Schule erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="df9fb-197">Entity who created the school.</span></span>|


## <a name="relationships"></a><span data-ttu-id="df9fb-198">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="df9fb-198">Relationships</span></span>
| <span data-ttu-id="df9fb-199">Beziehung</span><span class="sxs-lookup"><span data-stu-id="df9fb-199">Relationship</span></span> | <span data-ttu-id="df9fb-200">Typ</span><span class="sxs-lookup"><span data-stu-id="df9fb-200">Type</span></span>   |<span data-ttu-id="df9fb-201">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df9fb-201">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df9fb-202">classes</span><span class="sxs-lookup"><span data-stu-id="df9fb-202">classes</span></span>|<span data-ttu-id="df9fb-203">[educationClass](educationclass.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="df9fb-203">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="df9fb-204">In der Schule unterrichtete Klassen.</span><span class="sxs-lookup"><span data-stu-id="df9fb-204">Classes taught at the school.</span></span> <span data-ttu-id="df9fb-205">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="df9fb-205">Nullable.</span></span>|
|<span data-ttu-id="df9fb-206">users</span><span class="sxs-lookup"><span data-stu-id="df9fb-206">users</span></span>|<span data-ttu-id="df9fb-207">[educationUser](educationuser.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="df9fb-207">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="df9fb-208">Benutzer in der Schule.</span><span class="sxs-lookup"><span data-stu-id="df9fb-208">Users in the school.</span></span> <span data-ttu-id="df9fb-209">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="df9fb-209">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="df9fb-210">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="df9fb-210">JSON representation</span></span>

<span data-ttu-id="df9fb-211">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="df9fb-211">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSchool"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "description": "String",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "highestGrade": "String",
  "lowestGrade": "String",
  "schoolNumber": "String",
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalId": "String",
  "fax": "String",
  "phone": "String",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
