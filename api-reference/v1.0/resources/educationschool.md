---
title: educationSchool-Ressourcentyp
description: 'Eine Ressource, eine Schule darstellt und zum Verwalten der Klassen, Lehrkräfte und Schüler der repräsentierten Schule verwendet wird.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 2549d8babd000a36f0ff3ccd38541ef3c1b2e466
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925819"
---
# <a name="educationschool-resource-type"></a><span data-ttu-id="a2957-103">educationSchool-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a2957-103">educationSchool resource type</span></span>

<span data-ttu-id="a2957-104">Eine Ressource, eine Schule darstellt und zum Verwalten der Klassen, Lehrkräfte und Schüler der repräsentierten Schule verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="a2957-104">A resource representing a school and used to manage the classes, teachers, and students of the represented school.</span></span>  


## <a name="methods"></a><span data-ttu-id="a2957-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="a2957-105">Methods</span></span>

| <span data-ttu-id="a2957-106">Methode</span><span class="sxs-lookup"><span data-stu-id="a2957-106">Method</span></span>           | <span data-ttu-id="a2957-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="a2957-107">Return Type</span></span>    |<span data-ttu-id="a2957-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a2957-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a2957-109">Get</span><span class="sxs-lookup"><span data-stu-id="a2957-109">Get</span></span>](../api/educationschool-get.md) | [<span data-ttu-id="a2957-110">educationSchool</span><span class="sxs-lookup"><span data-stu-id="a2957-110">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="a2957-111">Lesen von Eigenschaften und Beziehungen eines **educationSchool**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a2957-111">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="a2957-112">Klasse hinzufügen</span><span class="sxs-lookup"><span data-stu-id="a2957-112">Add class</span></span>](../api/educationschool-post-classes.md) |[<span data-ttu-id="a2957-113">educationClass</span><span class="sxs-lookup"><span data-stu-id="a2957-113">educationClass</span></span>](educationclass.md)| <span data-ttu-id="a2957-114">Hinzufügen einer neuen **educationClass** für die Schule durch Bereitstellen in der Navigationseigenschaft „classes“.</span><span class="sxs-lookup"><span data-stu-id="a2957-114">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="a2957-115">Klassen auflisten</span><span class="sxs-lookup"><span data-stu-id="a2957-115">List classes</span></span>](../api/educationschool-list-classes.md) |<span data-ttu-id="a2957-116">[educationClass](educationclass.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a2957-116">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="a2957-117">Abrufen der **educationClass**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="a2957-117">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="a2957-118">Klasse entfernen</span><span class="sxs-lookup"><span data-stu-id="a2957-118">Remove class</span></span>](../api/educationschool-delete-classes.md) |[<span data-ttu-id="a2957-119">educationClass</span><span class="sxs-lookup"><span data-stu-id="a2957-119">educationClass</span></span>](educationclass.md)| <span data-ttu-id="a2957-120">Entfernen einer **educationClass** von der Schule über die Navigationseigenschaft „classes“.</span><span class="sxs-lookup"><span data-stu-id="a2957-120">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="a2957-121">Benutzer hinzufügen</span><span class="sxs-lookup"><span data-stu-id="a2957-121">Add user</span></span>](../api/educationschool-post-users.md) |[<span data-ttu-id="a2957-122">educationUser</span><span class="sxs-lookup"><span data-stu-id="a2957-122">educationUser</span></span>](educationuser.md)| <span data-ttu-id="a2957-123">Hinzufügen eines neuen **educationUser** für die Schule durch Bereitstellen in der Navigationseigenschaft **users**.</span><span class="sxs-lookup"><span data-stu-id="a2957-123">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="a2957-124">Benutzer auflisten</span><span class="sxs-lookup"><span data-stu-id="a2957-124">List users</span></span>](../api/educationschool-list-users.md) |<span data-ttu-id="a2957-125">[educationUser](educationuser.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a2957-125">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="a2957-126">Abrufen der **educationUser**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="a2957-126">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="a2957-127">Benutzer entfernen</span><span class="sxs-lookup"><span data-stu-id="a2957-127">Remove user</span></span>](../api/educationschool-delete-users.md) |[<span data-ttu-id="a2957-128">educationUser</span><span class="sxs-lookup"><span data-stu-id="a2957-128">educationUser</span></span>](educationuser.md)| <span data-ttu-id="a2957-129">Entfernen eines **educationUser** von der Schule über die Navigationseigenschaft **users**.</span><span class="sxs-lookup"><span data-stu-id="a2957-129">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="a2957-130">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a2957-130">Update</span></span>](../api/educationschool-update.md) | [<span data-ttu-id="a2957-131">educationSchool</span><span class="sxs-lookup"><span data-stu-id="a2957-131">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="a2957-132">Aktualisieren eines **educationSchool**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a2957-132">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="a2957-133">Löschen</span><span class="sxs-lookup"><span data-stu-id="a2957-133">Delete</span></span>](../api/educationschool-delete.md) | <span data-ttu-id="a2957-134">Keine</span><span class="sxs-lookup"><span data-stu-id="a2957-134">None</span></span> |<span data-ttu-id="a2957-135">Löschen eines **educationSchool**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a2957-135">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a2957-136">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a2957-136">Properties</span></span>
| <span data-ttu-id="a2957-137">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a2957-137">Property</span></span>     | <span data-ttu-id="a2957-138">Typ</span><span class="sxs-lookup"><span data-stu-id="a2957-138">Type</span></span>   |<span data-ttu-id="a2957-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a2957-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2957-140">id</span><span class="sxs-lookup"><span data-stu-id="a2957-140">id</span></span>|<span data-ttu-id="a2957-141">String</span><span class="sxs-lookup"><span data-stu-id="a2957-141">String</span></span>|<span data-ttu-id="a2957-142">GUID dieser Schule</span><span class="sxs-lookup"><span data-stu-id="a2957-142">GUID of this school.</span></span>|
|<span data-ttu-id="a2957-143">displayName</span><span class="sxs-lookup"><span data-stu-id="a2957-143">displayName</span></span>| <span data-ttu-id="a2957-144">String</span><span class="sxs-lookup"><span data-stu-id="a2957-144">String</span></span>| <span data-ttu-id="a2957-145">Anzeigename der Schule</span><span class="sxs-lookup"><span data-stu-id="a2957-145">Display name of the school.</span></span>| 
|<span data-ttu-id="a2957-146">description</span><span class="sxs-lookup"><span data-stu-id="a2957-146">description</span></span>| <span data-ttu-id="a2957-147">String</span><span class="sxs-lookup"><span data-stu-id="a2957-147">String</span></span> | <span data-ttu-id="a2957-148">Beschreibung der Schule</span><span class="sxs-lookup"><span data-stu-id="a2957-148">Description of the school.</span></span>| 
|<span data-ttu-id="a2957-149">status</span><span class="sxs-lookup"><span data-stu-id="a2957-149">status</span></span>| <span data-ttu-id="a2957-150">string</span><span class="sxs-lookup"><span data-stu-id="a2957-150">string</span></span>| <span data-ttu-id="a2957-151">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a2957-151">Read-Only.</span></span> <span data-ttu-id="a2957-152">Die möglichen Werte sind: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="a2957-152">The possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="a2957-153">externalSource</span><span class="sxs-lookup"><span data-stu-id="a2957-153">externalSource</span></span>| <span data-ttu-id="a2957-154">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="a2957-154">educationExternalSource</span></span>| <span data-ttu-id="a2957-155">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a2957-155">Read-Only.</span></span>  <span data-ttu-id="a2957-156">Die möglichen Werte sind: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="a2957-156">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="a2957-157">principalEmail</span><span class="sxs-lookup"><span data-stu-id="a2957-157">principalEmail</span></span>| <span data-ttu-id="a2957-158">String</span><span class="sxs-lookup"><span data-stu-id="a2957-158">String</span></span>| <span data-ttu-id="a2957-159">Die E-Mail-Adresse des Prinzipals</span><span class="sxs-lookup"><span data-stu-id="a2957-159">Email address of the principal.</span></span>|
|<span data-ttu-id="a2957-160">principalName</span><span class="sxs-lookup"><span data-stu-id="a2957-160">principalName</span></span>| <span data-ttu-id="a2957-161">String</span><span class="sxs-lookup"><span data-stu-id="a2957-161">String</span></span> | <span data-ttu-id="a2957-162">Der Name des Prinzipals</span><span class="sxs-lookup"><span data-stu-id="a2957-162">Name of the principal.</span></span>|
|<span data-ttu-id="a2957-163">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="a2957-163">externalPrincipalId</span></span>| <span data-ttu-id="a2957-164">String</span><span class="sxs-lookup"><span data-stu-id="a2957-164">String</span></span> | <span data-ttu-id="a2957-165">Die ID des Prinzipals im Synchronisierungssystem</span><span class="sxs-lookup"><span data-stu-id="a2957-165">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="a2957-166">highestGrade</span><span class="sxs-lookup"><span data-stu-id="a2957-166">highestGrade</span></span>|<span data-ttu-id="a2957-167">String</span><span class="sxs-lookup"><span data-stu-id="a2957-167">String</span></span>| <span data-ttu-id="a2957-168">Höchste unterrichtete Klasse</span><span class="sxs-lookup"><span data-stu-id="a2957-168">Highest grade taught.</span></span> |
|<span data-ttu-id="a2957-169">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="a2957-169">lowestGrade</span></span>|<span data-ttu-id="a2957-170">String</span><span class="sxs-lookup"><span data-stu-id="a2957-170">String</span></span>| <span data-ttu-id="a2957-171">Niedrigste unterrichtete Klasse</span><span class="sxs-lookup"><span data-stu-id="a2957-171">Lowest grade taught.</span></span> |
|<span data-ttu-id="a2957-172">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="a2957-172">schoolNumber</span></span>|<span data-ttu-id="a2957-173">String</span><span class="sxs-lookup"><span data-stu-id="a2957-173">String</span></span>| <span data-ttu-id="a2957-174">Schulnummer</span><span class="sxs-lookup"><span data-stu-id="a2957-174">School Number.</span></span>|
|<span data-ttu-id="a2957-175">externalId</span><span class="sxs-lookup"><span data-stu-id="a2957-175">externalId</span></span>|<span data-ttu-id="a2957-176">String</span><span class="sxs-lookup"><span data-stu-id="a2957-176">String</span></span>| <span data-ttu-id="a2957-177">Die ID der Schule im Synchronisierungssystem</span><span class="sxs-lookup"><span data-stu-id="a2957-177">ID of school in syncing system.</span></span> |
|<span data-ttu-id="a2957-178">phone</span><span class="sxs-lookup"><span data-stu-id="a2957-178">phone</span></span>|<span data-ttu-id="a2957-179">String</span><span class="sxs-lookup"><span data-stu-id="a2957-179">String</span></span>| <span data-ttu-id="a2957-180">Die Telefonnummer der Schule</span><span class="sxs-lookup"><span data-stu-id="a2957-180">Phone number of school.</span></span> |
|<span data-ttu-id="a2957-181">fax</span><span class="sxs-lookup"><span data-stu-id="a2957-181">fax</span></span>|<span data-ttu-id="a2957-182">String</span><span class="sxs-lookup"><span data-stu-id="a2957-182">String</span></span>| <span data-ttu-id="a2957-183">Die Faxnummer der Schule</span><span class="sxs-lookup"><span data-stu-id="a2957-183">Fax number of school.</span></span> |
|<span data-ttu-id="a2957-184">address</span><span class="sxs-lookup"><span data-stu-id="a2957-184">address</span></span>|[<span data-ttu-id="a2957-185">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="a2957-185">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="a2957-186">Die Adresse der Schule</span><span class="sxs-lookup"><span data-stu-id="a2957-186">Address of the school.</span></span>|
|<span data-ttu-id="a2957-187">createdBy</span><span class="sxs-lookup"><span data-stu-id="a2957-187">createdBy</span></span>|[<span data-ttu-id="a2957-188">identitySet</span><span class="sxs-lookup"><span data-stu-id="a2957-188">identitySet</span></span>](identityset.md)|<span data-ttu-id="a2957-189">Entität, die Schule erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="a2957-189">Entity who created the school.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2957-190">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a2957-190">Relationships</span></span>
| <span data-ttu-id="a2957-191">Beziehung</span><span class="sxs-lookup"><span data-stu-id="a2957-191">Relationship</span></span> | <span data-ttu-id="a2957-192">Typ</span><span class="sxs-lookup"><span data-stu-id="a2957-192">Type</span></span>   |<span data-ttu-id="a2957-193">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a2957-193">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2957-194">classes</span><span class="sxs-lookup"><span data-stu-id="a2957-194">classes</span></span>|<span data-ttu-id="a2957-195">[educationClass](educationclass.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a2957-195">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="a2957-196">In der Schule unterrichtete Klassen.</span><span class="sxs-lookup"><span data-stu-id="a2957-196">Classes taught at the school.</span></span> <span data-ttu-id="a2957-197">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="a2957-197">Nullable.</span></span>|
|<span data-ttu-id="a2957-198">users</span><span class="sxs-lookup"><span data-stu-id="a2957-198">users</span></span>|<span data-ttu-id="a2957-199">[educationUser](educationuser.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a2957-199">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="a2957-200">Benutzer in der Schule.</span><span class="sxs-lookup"><span data-stu-id="a2957-200">Users in the school.</span></span> <span data-ttu-id="a2957-201">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="a2957-201">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2957-202">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a2957-202">JSON representation</span></span>

<span data-ttu-id="a2957-203">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a2957-203">The following is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.educationOrganization",
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
