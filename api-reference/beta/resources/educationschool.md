---
title: educationSchool-Ressourcentyp
description: 'Eine Bildungseinrichtung. Die **educationSchool**-Ressource entspricht derzeit einer administrativeUnit-Ressource und hat dieselbe ID.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 917395324e6ae519af468a4bb4b31056796e1498
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512542"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="b2bb1-104">educationSchool-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b2bb1-104">educationSchool resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2bb1-105">Eine Bildungseinrichtung.</span><span class="sxs-lookup"><span data-stu-id="b2bb1-105">A school.</span></span> <span data-ttu-id="b2bb1-106">Die **educationSchool**-Ressource entspricht derzeit einer [administrativeUnit](administrativeunit.md)-Ressource und hat dieselbe ID.</span><span class="sxs-lookup"><span data-stu-id="b2bb1-106">The **educationSchool** resource currently corresponds to an [administrativeUnit](administrativeunit.md) resource and shares the same ID.</span></span>  

<span data-ttu-id="b2bb1-107">Diese Ressource ist ein Untertyp von [educationOrganization](educationorganization.md).</span><span class="sxs-lookup"><span data-stu-id="b2bb1-107">This resource is a subtype of [educationOrganization](educationorganization.md).</span></span>




## <a name="methods"></a><span data-ttu-id="b2bb1-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="b2bb1-108">Methods</span></span>

| <span data-ttu-id="b2bb1-109">Methode</span><span class="sxs-lookup"><span data-stu-id="b2bb1-109">Method</span></span>           | <span data-ttu-id="b2bb1-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b2bb1-110">Return Type</span></span>    |<span data-ttu-id="b2bb1-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b2bb1-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b2bb1-112">Get</span><span class="sxs-lookup"><span data-stu-id="b2bb1-112">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="b2bb1-113">educationSchool</span><span class="sxs-lookup"><span data-stu-id="b2bb1-113">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="b2bb1-114">Lesen von Eigenschaften und Beziehungen eines **educationSchool**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b2bb1-114">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="b2bb1-115">Klasse hinzufügen</span><span class="sxs-lookup"><span data-stu-id="b2bb1-115">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="b2bb1-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="b2bb1-116">educationClass</span></span>](educationclass.md)| <span data-ttu-id="b2bb1-117">Hinzufügen einer neuen **educationClass** für die Schule durch Bereitstellen in der Navigationseigenschaft „classes“.</span><span class="sxs-lookup"><span data-stu-id="b2bb1-117">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="b2bb1-118">Klassen auflisten</span><span class="sxs-lookup"><span data-stu-id="b2bb1-118">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="b2bb1-119">[educationClass](educationclass.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b2bb1-119">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="b2bb1-120">Abrufen der **educationClass**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="b2bb1-120">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="b2bb1-121">Klasse entfernen</span><span class="sxs-lookup"><span data-stu-id="b2bb1-121">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="b2bb1-122">educationClass</span><span class="sxs-lookup"><span data-stu-id="b2bb1-122">educationClass</span></span>](educationclass.md)| <span data-ttu-id="b2bb1-123">Entfernen einer **educationClass** von der Schule über die Navigationseigenschaft „classes“.</span><span class="sxs-lookup"><span data-stu-id="b2bb1-123">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="b2bb1-124">Benutzer hinzufügen</span><span class="sxs-lookup"><span data-stu-id="b2bb1-124">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="b2bb1-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="b2bb1-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="b2bb1-126">Hinzufügen eines neuen **educationUser** für die Schule durch Bereitstellen in der Navigationseigenschaft **users**.</span><span class="sxs-lookup"><span data-stu-id="b2bb1-126">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="b2bb1-127">Benutzer auflisten</span><span class="sxs-lookup"><span data-stu-id="b2bb1-127">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="b2bb1-128">[educationUser](educationuser.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b2bb1-128">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="b2bb1-129">Abrufen der **educationUser**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="b2bb1-129">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="b2bb1-130">Benutzer entfernen</span><span class="sxs-lookup"><span data-stu-id="b2bb1-130">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="b2bb1-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="b2bb1-131">educationUser</span></span>](educationuser.md)| <span data-ttu-id="b2bb1-132">Entfernen eines **educationUser** von der Schule über die Navigationseigenschaft **users**.</span><span class="sxs-lookup"><span data-stu-id="b2bb1-132">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="b2bb1-133">AdministrativeUnit abrufen</span><span class="sxs-lookup"><span data-stu-id="b2bb1-133">Get administrativeUnit</span></span>](../api/educationschool-get-administrativeunit.md) |[<span data-ttu-id="b2bb1-134">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="b2bb1-134">administrativeUnit</span></span>](administrativeunit.md)| <span data-ttu-id="b2bb1-135">Abrufen der **administrativeUnit**, die dieser **educationSchool** entspricht.</span><span class="sxs-lookup"><span data-stu-id="b2bb1-135">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>|
|[<span data-ttu-id="b2bb1-136">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b2bb1-136">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="b2bb1-137">educationSchool</span><span class="sxs-lookup"><span data-stu-id="b2bb1-137">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="b2bb1-138">Aktualisieren eines **educationSchool**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b2bb1-138">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="b2bb1-139">Löschen</span><span class="sxs-lookup"><span data-stu-id="b2bb1-139">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="b2bb1-140">Keine</span><span class="sxs-lookup"><span data-stu-id="b2bb1-140">None</span></span> |<span data-ttu-id="b2bb1-141">Löschen eines **educationSchool**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b2bb1-141">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b2bb1-142">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b2bb1-142">Properties</span></span>
| <span data-ttu-id="b2bb1-143">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b2bb1-143">Property</span></span>     | <span data-ttu-id="b2bb1-144">Typ</span><span class="sxs-lookup"><span data-stu-id="b2bb1-144">Type</span></span>   |<span data-ttu-id="b2bb1-145">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b2bb1-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2bb1-146">id</span><span class="sxs-lookup"><span data-stu-id="b2bb1-146">id</span></span>|<span data-ttu-id="b2bb1-147">string</span><span class="sxs-lookup"><span data-stu-id="b2bb1-147">String</span></span>|<span data-ttu-id="b2bb1-148">GUID dieser Schule</span><span class="sxs-lookup"><span data-stu-id="b2bb1-148">GUID of this school.</span></span>|
|<span data-ttu-id="b2bb1-149">displayName</span><span class="sxs-lookup"><span data-stu-id="b2bb1-149">displayName</span></span>| <span data-ttu-id="b2bb1-150">String</span><span class="sxs-lookup"><span data-stu-id="b2bb1-150">String</span></span>| <span data-ttu-id="b2bb1-151">Anzeigename der Schule</span><span class="sxs-lookup"><span data-stu-id="b2bb1-151">Display name of the school.</span></span>| 
|<span data-ttu-id="b2bb1-152">description</span><span class="sxs-lookup"><span data-stu-id="b2bb1-152">description</span></span>| <span data-ttu-id="b2bb1-153">String</span><span class="sxs-lookup"><span data-stu-id="b2bb1-153">String</span></span> | <span data-ttu-id="b2bb1-154">Beschreibung der Schule</span><span class="sxs-lookup"><span data-stu-id="b2bb1-154">Description of the school.</span></span>| 
|<span data-ttu-id="b2bb1-155">status</span><span class="sxs-lookup"><span data-stu-id="b2bb1-155">status</span></span>| <span data-ttu-id="b2bb1-156">string</span><span class="sxs-lookup"><span data-stu-id="b2bb1-156">string</span></span>| <span data-ttu-id="b2bb1-157">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b2bb1-157">Read-Only.</span></span> <span data-ttu-id="b2bb1-158">Mögliche Werte: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="b2bb1-158">Possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="b2bb1-159">externalSource</span><span class="sxs-lookup"><span data-stu-id="b2bb1-159">externalSource</span></span>| <span data-ttu-id="b2bb1-160">string</span><span class="sxs-lookup"><span data-stu-id="b2bb1-160">string</span></span>| <span data-ttu-id="b2bb1-161">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b2bb1-161">Read-Only.</span></span>  <span data-ttu-id="b2bb1-162">Mögliche Werte sind: `sis`, `manual` und `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b2bb1-162">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="b2bb1-163">principalEmail</span><span class="sxs-lookup"><span data-stu-id="b2bb1-163">principalEmail</span></span>| <span data-ttu-id="b2bb1-164">String</span><span class="sxs-lookup"><span data-stu-id="b2bb1-164">String</span></span>| <span data-ttu-id="b2bb1-165">Die E-Mail-Adresse des Prinzipals</span><span class="sxs-lookup"><span data-stu-id="b2bb1-165">Email address of the principal.</span></span>|
|<span data-ttu-id="b2bb1-166">principalName</span><span class="sxs-lookup"><span data-stu-id="b2bb1-166">principalName</span></span>| <span data-ttu-id="b2bb1-167">String</span><span class="sxs-lookup"><span data-stu-id="b2bb1-167">String</span></span> | <span data-ttu-id="b2bb1-168">Der Name des Prinzipals</span><span class="sxs-lookup"><span data-stu-id="b2bb1-168">Name of the principal.</span></span>|
|<span data-ttu-id="b2bb1-169">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="b2bb1-169">externalPrincipalId</span></span>| <span data-ttu-id="b2bb1-170">String</span><span class="sxs-lookup"><span data-stu-id="b2bb1-170">String</span></span> | <span data-ttu-id="b2bb1-171">Die ID des Prinzipals im Synchronisierungssystem</span><span class="sxs-lookup"><span data-stu-id="b2bb1-171">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="b2bb1-172">highestGrade</span><span class="sxs-lookup"><span data-stu-id="b2bb1-172">highestGrade</span></span>|<span data-ttu-id="b2bb1-173">String</span><span class="sxs-lookup"><span data-stu-id="b2bb1-173">String</span></span>| <span data-ttu-id="b2bb1-174">Höchste unterrichtete Klasse</span><span class="sxs-lookup"><span data-stu-id="b2bb1-174">Highest grade taught.</span></span> |
|<span data-ttu-id="b2bb1-175">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="b2bb1-175">lowestGrade</span></span>|<span data-ttu-id="b2bb1-176">String</span><span class="sxs-lookup"><span data-stu-id="b2bb1-176">String</span></span>| <span data-ttu-id="b2bb1-177">Niedrigste unterrichtete Klasse</span><span class="sxs-lookup"><span data-stu-id="b2bb1-177">Lowest grade taught.</span></span> |
|<span data-ttu-id="b2bb1-178">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="b2bb1-178">schoolNumber</span></span>|<span data-ttu-id="b2bb1-179">String</span><span class="sxs-lookup"><span data-stu-id="b2bb1-179">String</span></span>| <span data-ttu-id="b2bb1-180">Schulnummer</span><span class="sxs-lookup"><span data-stu-id="b2bb1-180">School Number.</span></span>|
|<span data-ttu-id="b2bb1-181">externalId</span><span class="sxs-lookup"><span data-stu-id="b2bb1-181">externalId</span></span>|<span data-ttu-id="b2bb1-182">String</span><span class="sxs-lookup"><span data-stu-id="b2bb1-182">String</span></span>| <span data-ttu-id="b2bb1-183">Die ID der Schule im Synchronisierungssystem</span><span class="sxs-lookup"><span data-stu-id="b2bb1-183">ID of school in syncing system.</span></span> |
|<span data-ttu-id="b2bb1-184">phone</span><span class="sxs-lookup"><span data-stu-id="b2bb1-184">phone</span></span>|<span data-ttu-id="b2bb1-185">String</span><span class="sxs-lookup"><span data-stu-id="b2bb1-185">String</span></span>| <span data-ttu-id="b2bb1-186">Die Telefonnummer der Schule</span><span class="sxs-lookup"><span data-stu-id="b2bb1-186">Phone number of school.</span></span> |
|<span data-ttu-id="b2bb1-187">fax</span><span class="sxs-lookup"><span data-stu-id="b2bb1-187">fax</span></span>|<span data-ttu-id="b2bb1-188">String</span><span class="sxs-lookup"><span data-stu-id="b2bb1-188">String</span></span>| <span data-ttu-id="b2bb1-189">Die Faxnummer der Schule</span><span class="sxs-lookup"><span data-stu-id="b2bb1-189">Fax number of school.</span></span> |
|<span data-ttu-id="b2bb1-190">address</span><span class="sxs-lookup"><span data-stu-id="b2bb1-190">address</span></span>|[<span data-ttu-id="b2bb1-191">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="b2bb1-191">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="b2bb1-192">Die Adresse der Schule</span><span class="sxs-lookup"><span data-stu-id="b2bb1-192">Address of the school.</span></span>|
|<span data-ttu-id="b2bb1-193">createdBy</span><span class="sxs-lookup"><span data-stu-id="b2bb1-193">createdBy</span></span>|[<span data-ttu-id="b2bb1-194">identitySet</span><span class="sxs-lookup"><span data-stu-id="b2bb1-194">identitySet</span></span>](identityset.md)|<span data-ttu-id="b2bb1-195">Entität, die Schule erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="b2bb1-195">Entity who created the school.</span></span>|


## <a name="relationships"></a><span data-ttu-id="b2bb1-196">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b2bb1-196">Relationships</span></span>
| <span data-ttu-id="b2bb1-197">Beziehung</span><span class="sxs-lookup"><span data-stu-id="b2bb1-197">Relationship</span></span> | <span data-ttu-id="b2bb1-198">Typ</span><span class="sxs-lookup"><span data-stu-id="b2bb1-198">Type</span></span>   |<span data-ttu-id="b2bb1-199">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b2bb1-199">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2bb1-200">classes</span><span class="sxs-lookup"><span data-stu-id="b2bb1-200">classes</span></span>|<span data-ttu-id="b2bb1-201">[educationClass](educationclass.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b2bb1-201">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="b2bb1-202">In der Schule unterrichtete Klassen.</span><span class="sxs-lookup"><span data-stu-id="b2bb1-202">Classes taught at the school.</span></span> <span data-ttu-id="b2bb1-203">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="b2bb1-203">Nullable.</span></span>|
|<span data-ttu-id="b2bb1-204">users</span><span class="sxs-lookup"><span data-stu-id="b2bb1-204">users</span></span>|<span data-ttu-id="b2bb1-205">[educationUser](educationuser.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b2bb1-205">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="b2bb1-206">Benutzer in der Schule.</span><span class="sxs-lookup"><span data-stu-id="b2bb1-206">Users in the school.</span></span> <span data-ttu-id="b2bb1-207">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="b2bb1-207">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b2bb1-208">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b2bb1-208">JSON representation</span></span>

<span data-ttu-id="b2bb1-209">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b2bb1-209">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationschool.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
