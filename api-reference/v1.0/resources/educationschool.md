# <a name="educationschool-resource-type"></a><span data-ttu-id="28fe3-101">educationSchool-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="28fe3-101">educationSchool resource type</span></span>

<span data-ttu-id="28fe3-102">Eine Ressource, eine Schule darstellt und zum Verwalten der Klassen, Lehrkräfte und Schüler der repräsentierten Schule verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="28fe3-102">A resource representing a school and used to manage the classes, teachers, and students of the represented school.</span></span>  


## <a name="methods"></a><span data-ttu-id="28fe3-103">Methoden</span><span class="sxs-lookup"><span data-stu-id="28fe3-103">Methods</span></span>

| <span data-ttu-id="28fe3-104">Methode</span><span class="sxs-lookup"><span data-stu-id="28fe3-104">Method</span></span>           | <span data-ttu-id="28fe3-105">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="28fe3-105">Return Type</span></span>    |<span data-ttu-id="28fe3-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28fe3-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="28fe3-107">Get</span><span class="sxs-lookup"><span data-stu-id="28fe3-107">Get</span></span>](../api/educationschool_get.md) | [<span data-ttu-id="28fe3-108">educationSchool</span><span class="sxs-lookup"><span data-stu-id="28fe3-108">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="28fe3-109">Lesen von Eigenschaften und Beziehungen eines **educationSchool**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="28fe3-109">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="28fe3-110">Klasse hinzufügen</span><span class="sxs-lookup"><span data-stu-id="28fe3-110">Add class</span></span>](../api/educationschool_post_classes.md) |[<span data-ttu-id="28fe3-111">educationClass</span><span class="sxs-lookup"><span data-stu-id="28fe3-111">educationClass</span></span>](educationclass.md)| <span data-ttu-id="28fe3-112">Hinzufügen einer neuen **educationClass** für die Schule durch Bereitstellen in der Navigationseigenschaft „classes“.</span><span class="sxs-lookup"><span data-stu-id="28fe3-112">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="28fe3-113">Klassen auflisten</span><span class="sxs-lookup"><span data-stu-id="28fe3-113">List classes</span></span>](../api/educationschool_list_classes.md) |<span data-ttu-id="28fe3-114">[educationClass](educationclass.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="28fe3-114">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="28fe3-115">Abrufen der **educationClass**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="28fe3-115">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="28fe3-116">Klasse entfernen</span><span class="sxs-lookup"><span data-stu-id="28fe3-116">Remove class</span></span>](../api/educationschool_delete_classes.md) |[<span data-ttu-id="28fe3-117">educationClass</span><span class="sxs-lookup"><span data-stu-id="28fe3-117">educationClass</span></span>](educationclass.md)| <span data-ttu-id="28fe3-118">Entfernen einer **educationClass** von der Schule über die Navigationseigenschaft „classes“.</span><span class="sxs-lookup"><span data-stu-id="28fe3-118">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="28fe3-119">Benutzer hinzufügen</span><span class="sxs-lookup"><span data-stu-id="28fe3-119">Add user</span></span>](../api/educationschool_post_users.md) |[<span data-ttu-id="28fe3-120">educationUser</span><span class="sxs-lookup"><span data-stu-id="28fe3-120">educationUser</span></span>](educationuser.md)| <span data-ttu-id="28fe3-121">Hinzufügen eines neuen **educationUser** für die Schule durch Bereitstellen in der Navigationseigenschaft **users**.</span><span class="sxs-lookup"><span data-stu-id="28fe3-121">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="28fe3-122">Benutzer auflisten</span><span class="sxs-lookup"><span data-stu-id="28fe3-122">List users</span></span>](../api/educationschool_list_users.md) |<span data-ttu-id="28fe3-123">[educationUser](educationuser.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="28fe3-123">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="28fe3-124">Abrufen der **educationUser**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="28fe3-124">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="28fe3-125">Benutzer entfernen</span><span class="sxs-lookup"><span data-stu-id="28fe3-125">Remove user</span></span>](../api/educationschool_delete_users.md) |[<span data-ttu-id="28fe3-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="28fe3-126">educationUser</span></span>](educationuser.md)| <span data-ttu-id="28fe3-127">Entfernen eines **educationUser** von der Schule über die Navigationseigenschaft **users**.</span><span class="sxs-lookup"><span data-stu-id="28fe3-127">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="28fe3-128">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="28fe3-128">Update</span></span>](../api/educationschool_update.md) | [<span data-ttu-id="28fe3-129">educationSchool</span><span class="sxs-lookup"><span data-stu-id="28fe3-129">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="28fe3-130">Aktualisieren eines **educationSchool**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="28fe3-130">Update an **event** object.</span></span> |
|[<span data-ttu-id="28fe3-131">Löschen</span><span class="sxs-lookup"><span data-stu-id="28fe3-131">Delete</span></span>](../api/educationschool_delete.md) | <span data-ttu-id="28fe3-132">Keine</span><span class="sxs-lookup"><span data-stu-id="28fe3-132">None</span></span> |<span data-ttu-id="28fe3-133">Löschen eines **educationSchool**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="28fe3-133">Delete an **event** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="28fe3-134">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="28fe3-134">Properties</span></span>
| <span data-ttu-id="28fe3-135">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="28fe3-135">Property</span></span>     | <span data-ttu-id="28fe3-136">Typ</span><span class="sxs-lookup"><span data-stu-id="28fe3-136">Type</span></span>   |<span data-ttu-id="28fe3-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28fe3-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28fe3-138">id</span><span class="sxs-lookup"><span data-stu-id="28fe3-138">id</span></span>|<span data-ttu-id="28fe3-139">String</span><span class="sxs-lookup"><span data-stu-id="28fe3-139">String</span></span>|<span data-ttu-id="28fe3-140">GUID dieser Schule</span><span class="sxs-lookup"><span data-stu-id="28fe3-140">GUID of this school.</span></span>|
|<span data-ttu-id="28fe3-141">displayName</span><span class="sxs-lookup"><span data-stu-id="28fe3-141">displayName</span></span>| <span data-ttu-id="28fe3-142">String</span><span class="sxs-lookup"><span data-stu-id="28fe3-142">String</span></span>| <span data-ttu-id="28fe3-143">Anzeigename der Schule</span><span class="sxs-lookup"><span data-stu-id="28fe3-143">Display name of the template.</span></span>| 
|<span data-ttu-id="28fe3-144">description</span><span class="sxs-lookup"><span data-stu-id="28fe3-144">description</span></span>| <span data-ttu-id="28fe3-145">String</span><span class="sxs-lookup"><span data-stu-id="28fe3-145">String</span></span> | <span data-ttu-id="28fe3-146">Beschreibung der Schule</span><span class="sxs-lookup"><span data-stu-id="28fe3-146">Description of the template.</span></span>| 
|<span data-ttu-id="28fe3-147">status</span><span class="sxs-lookup"><span data-stu-id="28fe3-147">status</span></span>| <span data-ttu-id="28fe3-148">string</span><span class="sxs-lookup"><span data-stu-id="28fe3-148">string</span></span>| <span data-ttu-id="28fe3-149">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="28fe3-149">Read-only.</span></span> <span data-ttu-id="28fe3-150">Mögliche Werte: `inactive`, `active`, `expired`, `deleteable`.</span><span class="sxs-lookup"><span data-stu-id="28fe3-150">Possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="28fe3-151">externalSource</span><span class="sxs-lookup"><span data-stu-id="28fe3-151">externalSource</span></span>| <span data-ttu-id="28fe3-152">string</span><span class="sxs-lookup"><span data-stu-id="28fe3-152">string</span></span>| <span data-ttu-id="28fe3-153">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="28fe3-153">Read-only.</span></span>  <span data-ttu-id="28fe3-154">Mögliche Werte sind: `sis`, `manual` und `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="28fe3-154">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="28fe3-155">principalEmail</span><span class="sxs-lookup"><span data-stu-id="28fe3-155">principalEmail</span></span>| <span data-ttu-id="28fe3-156">String</span><span class="sxs-lookup"><span data-stu-id="28fe3-156">String</span></span>| <span data-ttu-id="28fe3-157">Die E-Mail-Adresse des Prinzipals</span><span class="sxs-lookup"><span data-stu-id="28fe3-157">Email address of the principal.</span></span>|
|<span data-ttu-id="28fe3-158">principalName</span><span class="sxs-lookup"><span data-stu-id="28fe3-158">principalName</span></span>| <span data-ttu-id="28fe3-159">String</span><span class="sxs-lookup"><span data-stu-id="28fe3-159">String</span></span> | <span data-ttu-id="28fe3-160">Der Name des Prinzipals</span><span class="sxs-lookup"><span data-stu-id="28fe3-160">Name of the principal.</span></span>|
|<span data-ttu-id="28fe3-161">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="28fe3-161">externalPrincipalId</span></span>| <span data-ttu-id="28fe3-162">String</span><span class="sxs-lookup"><span data-stu-id="28fe3-162">String</span></span> | <span data-ttu-id="28fe3-163">Die ID des Prinzipals im Synchronisierungssystem</span><span class="sxs-lookup"><span data-stu-id="28fe3-163">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="28fe3-164">highestGrade</span><span class="sxs-lookup"><span data-stu-id="28fe3-164">highestGrade</span></span>|<span data-ttu-id="28fe3-165">String</span><span class="sxs-lookup"><span data-stu-id="28fe3-165">String</span></span>| <span data-ttu-id="28fe3-166">Höchste unterrichtete Klasse</span><span class="sxs-lookup"><span data-stu-id="28fe3-166">Highest grade taught.</span></span> |
|<span data-ttu-id="28fe3-167">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="28fe3-167">lowestGrade</span></span>|<span data-ttu-id="28fe3-168">String</span><span class="sxs-lookup"><span data-stu-id="28fe3-168">String</span></span>| <span data-ttu-id="28fe3-169">Niedrigste unterrichtete Klasse</span><span class="sxs-lookup"><span data-stu-id="28fe3-169">Lowest grade taught.</span></span> |
|<span data-ttu-id="28fe3-170">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="28fe3-170">schoolNumber</span></span>|<span data-ttu-id="28fe3-171">String</span><span class="sxs-lookup"><span data-stu-id="28fe3-171">String</span></span>| <span data-ttu-id="28fe3-172">Schulnummer</span><span class="sxs-lookup"><span data-stu-id="28fe3-172">School Number.</span></span>|
|<span data-ttu-id="28fe3-173">externalId</span><span class="sxs-lookup"><span data-stu-id="28fe3-173">externalId</span></span>|<span data-ttu-id="28fe3-174">String</span><span class="sxs-lookup"><span data-stu-id="28fe3-174">String</span></span>| <span data-ttu-id="28fe3-175">Die ID der Schule im Synchronisierungssystem</span><span class="sxs-lookup"><span data-stu-id="28fe3-175">ID of school in syncing system.</span></span> |
|<span data-ttu-id="28fe3-176">phone</span><span class="sxs-lookup"><span data-stu-id="28fe3-176">Phone</span></span>|<span data-ttu-id="28fe3-177">String</span><span class="sxs-lookup"><span data-stu-id="28fe3-177">String</span></span>| <span data-ttu-id="28fe3-178">Die Telefonnummer der Schule</span><span class="sxs-lookup"><span data-stu-id="28fe3-178">Phone number of school.</span></span> |
|<span data-ttu-id="28fe3-179">fax</span><span class="sxs-lookup"><span data-stu-id="28fe3-179">fax</span></span>|<span data-ttu-id="28fe3-180">String</span><span class="sxs-lookup"><span data-stu-id="28fe3-180">String</span></span>| <span data-ttu-id="28fe3-181">Die Faxnummer der Schule</span><span class="sxs-lookup"><span data-stu-id="28fe3-181">Fax number of school.</span></span> |
|<span data-ttu-id="28fe3-182">address</span><span class="sxs-lookup"><span data-stu-id="28fe3-182">address</span></span>|[<span data-ttu-id="28fe3-183">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="28fe3-183">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="28fe3-184">Die Adresse der Schule</span><span class="sxs-lookup"><span data-stu-id="28fe3-184">Address of the school.</span></span>|
|<span data-ttu-id="28fe3-185">createdBy</span><span class="sxs-lookup"><span data-stu-id="28fe3-185">createdBy</span></span>|[<span data-ttu-id="28fe3-186">identitySet</span><span class="sxs-lookup"><span data-stu-id="28fe3-186">identitySet</span></span>](identityset.md)|<span data-ttu-id="28fe3-187">Entität, die Schule erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="28fe3-187">Entity who created the school.</span></span>|


## <a name="relationships"></a><span data-ttu-id="28fe3-188">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="28fe3-188">Relationships</span></span>
| <span data-ttu-id="28fe3-189">Beziehung</span><span class="sxs-lookup"><span data-stu-id="28fe3-189">Relationship</span></span> | <span data-ttu-id="28fe3-190">Typ</span><span class="sxs-lookup"><span data-stu-id="28fe3-190">Type</span></span>   |<span data-ttu-id="28fe3-191">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28fe3-191">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28fe3-192">classes</span><span class="sxs-lookup"><span data-stu-id="28fe3-192">Classes</span></span>|<span data-ttu-id="28fe3-193">[educationClass](educationclass.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="28fe3-193">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="28fe3-194">In der Schule unterrichtete Klassen.</span><span class="sxs-lookup"><span data-stu-id="28fe3-194">Classes taught at the school.</span></span> <span data-ttu-id="28fe3-195">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="28fe3-195">Nullable.</span></span>|
|<span data-ttu-id="28fe3-196">users</span><span class="sxs-lookup"><span data-stu-id="28fe3-196">users</span></span>|<span data-ttu-id="28fe3-197">[educationUser](educationuser.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="28fe3-197">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="28fe3-198">Benutzer in der Schule.</span><span class="sxs-lookup"><span data-stu-id="28fe3-198">Users in the school.</span></span> <span data-ttu-id="28fe3-199">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="28fe3-199">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="28fe3-200">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="28fe3-200">JSON representation</span></span>

<span data-ttu-id="28fe3-201">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="28fe3-201">The following is a JSON representation of the resource.</span></span>

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
