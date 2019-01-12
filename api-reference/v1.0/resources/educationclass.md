---
title: educationClass-Ressourcentyp
description: 'Stellt eine Klasse in einer Schule dar. Die **educationClass**-Ressource entspricht der Office 365-Gruppe und hat die gleiche ID. Kursteilnehmer sind reguläre Mitglieder der Klasse, Lehrer sind Besitzer und verfügen über entsprechende Rechte. Damit Office-Benutzeroberflächen ordnungsgemäß funktionieren, müssen Lehrer Mitglieder der Sammlungen der Lehrkräfte wie auch der Mitglieder sein.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: c5b145d12dd99293eef9c338ff840d5781c5ef3f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933988"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="ebd4f-106">educationClass-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ebd4f-106">educationClass resource type</span></span>

<span data-ttu-id="ebd4f-107">Stellt eine Klasse in einer Schule dar.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-107">Represents a class within a school.</span></span> <span data-ttu-id="ebd4f-108">Die **educationClass**-Ressource entspricht der Office 365-Gruppe und hat die gleiche ID.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-108">The **educationClass** resource corresponds to the Office 365 group and shares the same ID.</span></span> <span data-ttu-id="ebd4f-109">Kursteilnehmer sind reguläre Mitglieder der Klasse, Lehrer sind Besitzer und verfügen über entsprechende Rechte.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-109">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="ebd4f-110">Damit Office-Benutzeroberflächen ordnungsgemäß funktionieren, müssen Lehrer Mitglieder der Sammlungen der Lehrkräfte wie auch der Mitglieder sein.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-110">For Office experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>  


## <a name="methods"></a><span data-ttu-id="ebd4f-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="ebd4f-111">Methods</span></span>

| <span data-ttu-id="ebd4f-112">Methode</span><span class="sxs-lookup"><span data-stu-id="ebd4f-112">Method</span></span>           | <span data-ttu-id="ebd4f-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="ebd4f-113">Return Type</span></span>    |<span data-ttu-id="ebd4f-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ebd4f-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ebd4f-115">EducationClass abrufen</span><span class="sxs-lookup"><span data-stu-id="ebd4f-115">Get educationClass</span></span>](../api/educationclass-get.md) | [<span data-ttu-id="ebd4f-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="ebd4f-116">educationClass</span></span>](educationclass.md) |<span data-ttu-id="ebd4f-117">Lesen von Eigenschaften und Beziehungen eines **educationClass**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-117">Read properties and relationships of an **educationClass** object.</span></span>|
|[<span data-ttu-id="ebd4f-118">Mitglied hinzufügen</span><span class="sxs-lookup"><span data-stu-id="ebd4f-118">Add member</span></span>](../api/educationclass-post-members.md) |[<span data-ttu-id="ebd4f-119">educationUser</span><span class="sxs-lookup"><span data-stu-id="ebd4f-119">educationUser</span></span>](educationuser.md)| <span data-ttu-id="ebd4f-120">Hinzufügen eines neuen **educationUser** für die Klasse durch Bereitstellen in der Navigationseigenschaft „members“.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-120">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="ebd4f-121">Mitglieder auflisten</span><span class="sxs-lookup"><span data-stu-id="ebd4f-121">List members</span></span>](../api/educationclass-list-members.md) |<span data-ttu-id="ebd4f-122">[educationUser](educationuser.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ebd4f-122">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="ebd4f-123">Abrufen einer **educationUser**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-123">Get an **educationUser** object collection.</span></span>|
|[<span data-ttu-id="ebd4f-124">Kursteilnehmer entfernen</span><span class="sxs-lookup"><span data-stu-id="ebd4f-124">Remove student</span></span>](../api/educationclass-delete-members.md) |[<span data-ttu-id="ebd4f-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="ebd4f-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="ebd4f-126">Entfernen eines **educationUser** aus der Klasse über die Navigationseigenschaft „members“.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-126">Remove an **educationUser** from the class through the members navigation property.</span></span>|
|[<span data-ttu-id="ebd4f-127">Schulen auflisten</span><span class="sxs-lookup"><span data-stu-id="ebd4f-127">List schools</span></span>](../api/educationclass-list-schools.md) |<span data-ttu-id="ebd4f-128">[educationSchool](educationschool.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ebd4f-128">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="ebd4f-129">Abrufen einer **educationSchool**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-129">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="ebd4f-130">Lehrer hinzufügen</span><span class="sxs-lookup"><span data-stu-id="ebd4f-130">Add teacher</span></span>](../api/educationclass-post-teachers.md) |[<span data-ttu-id="ebd4f-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="ebd4f-131">educationUser</span></span>](educationuser.md)| <span data-ttu-id="ebd4f-132">Hinzufügen eines neuen **educationUser** für die Klasse durch Bereitstellen in der Navigationseigenschaft „teachers“.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-132">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span>|
|[<span data-ttu-id="ebd4f-133">Lehrer auflisten</span><span class="sxs-lookup"><span data-stu-id="ebd4f-133">List teachers</span></span>](../api/educationclass-list-teachers.md) |<span data-ttu-id="ebd4f-134">[educationUser](educationuser.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ebd4f-134">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="ebd4f-135">Abrufen einer Liste der Lehrer für die Klasse</span><span class="sxs-lookup"><span data-stu-id="ebd4f-135">Get a list of teachers for the class.</span></span>|
|[<span data-ttu-id="ebd4f-136">Lehrer entfernen</span><span class="sxs-lookup"><span data-stu-id="ebd4f-136">Remove teacher</span></span>](../api/educationclass-delete-teachers.md) |[<span data-ttu-id="ebd4f-137">educationUser</span><span class="sxs-lookup"><span data-stu-id="ebd4f-137">educationUser</span></span>](educationuser.md)| <span data-ttu-id="ebd4f-138">Entfernen eines **educationUser** aus der Klasse über die Navigationseigenschaft „teachers“.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-138">Remove an **educationUser** from the class through the teachers navigation property.</span></span>|
|[<span data-ttu-id="ebd4f-139">Gruppe abrufen</span><span class="sxs-lookup"><span data-stu-id="ebd4f-139">Get group</span></span>](../api/educationclass-get-group.md) |[<span data-ttu-id="ebd4f-140">group</span><span class="sxs-lookup"><span data-stu-id="ebd4f-140">group</span></span>](group.md)| <span data-ttu-id="ebd4f-141">Abrufen der Office 365-**Gruppe**, die dieser **educationClass** entspricht.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-141">Get the Office 365 **group** that corresponds to this **educationClass**.</span></span>|
|[<span data-ttu-id="ebd4f-142">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ebd4f-142">Update</span></span>](../api/educationclass-update.md) | [<span data-ttu-id="ebd4f-143">educationClass</span><span class="sxs-lookup"><span data-stu-id="ebd4f-143">educationClass</span></span>](educationclass.md)    |<span data-ttu-id="ebd4f-144">Aktualisieren eines **educationClass**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-144">Update **educationClass** object.</span></span> |
|[<span data-ttu-id="ebd4f-145">Löschen</span><span class="sxs-lookup"><span data-stu-id="ebd4f-145">Delete</span></span>](../api/educationclass-delete.md) | <span data-ttu-id="ebd4f-146">Keine</span><span class="sxs-lookup"><span data-stu-id="ebd4f-146">None</span></span> |<span data-ttu-id="ebd4f-147">Löschen eines **educationClass**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-147">Delete **educationClass** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ebd4f-148">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ebd4f-148">Properties</span></span>
| <span data-ttu-id="ebd4f-149">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ebd4f-149">Property</span></span>     | <span data-ttu-id="ebd4f-150">Typ</span><span class="sxs-lookup"><span data-stu-id="ebd4f-150">Type</span></span>   |<span data-ttu-id="ebd4f-151">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ebd4f-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ebd4f-152">id</span><span class="sxs-lookup"><span data-stu-id="ebd4f-152">id</span></span>| <span data-ttu-id="ebd4f-153">String</span><span class="sxs-lookup"><span data-stu-id="ebd4f-153">String</span></span>| <span data-ttu-id="ebd4f-154">Eindeutiger Bezeichner für die Klasse</span><span class="sxs-lookup"><span data-stu-id="ebd4f-154">Unique identifier for the class.</span></span>|
|<span data-ttu-id="ebd4f-155">description</span><span class="sxs-lookup"><span data-stu-id="ebd4f-155">description</span></span>|<span data-ttu-id="ebd4f-156">String</span><span class="sxs-lookup"><span data-stu-id="ebd4f-156">String</span></span>| <span data-ttu-id="ebd4f-157">Beschreibung der Klasse</span><span class="sxs-lookup"><span data-stu-id="ebd4f-157">Description of the class.</span></span>|
|<span data-ttu-id="ebd4f-158">displayName</span><span class="sxs-lookup"><span data-stu-id="ebd4f-158">displayName</span></span>|<span data-ttu-id="ebd4f-159">String</span><span class="sxs-lookup"><span data-stu-id="ebd4f-159">String</span></span>| <span data-ttu-id="ebd4f-160">Der Name der Klasse</span><span class="sxs-lookup"><span data-stu-id="ebd4f-160">Name of the class.</span></span>|
|<span data-ttu-id="ebd4f-161">mailNickname</span><span class="sxs-lookup"><span data-stu-id="ebd4f-161">mailNickname</span></span>|<span data-ttu-id="ebd4f-162">String</span><span class="sxs-lookup"><span data-stu-id="ebd4f-162">String</span></span>| <span data-ttu-id="ebd4f-163">E-Mail-Name zum Senden von E-Mails an alle Mitglieder, wenn diese Option aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-163">Mail name for sending email to all members, if this is enabled.</span></span> |
|<span data-ttu-id="ebd4f-164">createdBy</span><span class="sxs-lookup"><span data-stu-id="ebd4f-164">createdBy</span></span>|[<span data-ttu-id="ebd4f-165">identitySet</span><span class="sxs-lookup"><span data-stu-id="ebd4f-165">identitySet</span></span>](identityset.md)| <span data-ttu-id="ebd4f-166">Entität, die die Klasse erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-166">Entity who created the class</span></span> |
|<span data-ttu-id="ebd4f-167">classCode</span><span class="sxs-lookup"><span data-stu-id="ebd4f-167">classCode</span></span>|<span data-ttu-id="ebd4f-168">String</span><span class="sxs-lookup"><span data-stu-id="ebd4f-168">String</span></span>| <span data-ttu-id="ebd4f-169">Von der Schule verwendeter Klassencode zum Identifizieren der Klasse</span><span class="sxs-lookup"><span data-stu-id="ebd4f-169">Class code used by the school to identify the class.</span></span>|
|<span data-ttu-id="ebd4f-170">externalId</span><span class="sxs-lookup"><span data-stu-id="ebd4f-170">externalId</span></span>|<span data-ttu-id="ebd4f-171">String</span><span class="sxs-lookup"><span data-stu-id="ebd4f-171">String</span></span>| <span data-ttu-id="ebd4f-172">ID der Klasse aus dem Synchronisierungssystem</span><span class="sxs-lookup"><span data-stu-id="ebd4f-172">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="ebd4f-173">externalName</span><span class="sxs-lookup"><span data-stu-id="ebd4f-173">externalName</span></span>|<span data-ttu-id="ebd4f-174">String</span><span class="sxs-lookup"><span data-stu-id="ebd4f-174">String</span></span>|<span data-ttu-id="ebd4f-175">Der Name der Klasse im Synchronisierungssystem</span><span class="sxs-lookup"><span data-stu-id="ebd4f-175">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="ebd4f-176">externalSource</span><span class="sxs-lookup"><span data-stu-id="ebd4f-176">externalSource</span></span>|<span data-ttu-id="ebd4f-177">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="ebd4f-177">educationExternalSource</span></span>| <span data-ttu-id="ebd4f-178">Quelle, aus der diese Klasse erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-178">How this class was created.</span></span> <span data-ttu-id="ebd4f-179">Die möglichen Werte sind: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-179">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="ebd4f-180">term</span><span class="sxs-lookup"><span data-stu-id="ebd4f-180">term</span></span>|[<span data-ttu-id="ebd4f-181">educationTerm</span><span class="sxs-lookup"><span data-stu-id="ebd4f-181">educationTerm</span></span>](educationterm.md)|<span data-ttu-id="ebd4f-182">Der Zeitraum für diese Klasse.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-182">Term for this class.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebd4f-183">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ebd4f-183">Relationships</span></span>
| <span data-ttu-id="ebd4f-184">Beziehung</span><span class="sxs-lookup"><span data-stu-id="ebd4f-184">Relationship</span></span> | <span data-ttu-id="ebd4f-185">Typ</span><span class="sxs-lookup"><span data-stu-id="ebd4f-185">Type</span></span>   |<span data-ttu-id="ebd4f-186">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ebd4f-186">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ebd4f-187">members</span><span class="sxs-lookup"><span data-stu-id="ebd4f-187">members</span></span>|<span data-ttu-id="ebd4f-188">[educationUser](../resources/educationuser.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ebd4f-188">[educationUser](../resources/educationuser.md) collection</span></span>| <span data-ttu-id="ebd4f-189">Alle Benutzer in der Klasse.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-189">All users in the class.</span></span> <span data-ttu-id="ebd4f-190">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-190">Nullable.</span></span>|
|<span data-ttu-id="ebd4f-191">schools</span><span class="sxs-lookup"><span data-stu-id="ebd4f-191">schools</span></span>|<span data-ttu-id="ebd4f-192">[educationSchool](../resources/educationschool.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ebd4f-192">[educationSchool](../resources/educationschool.md) collection</span></span>| <span data-ttu-id="ebd4f-193">Alle Schulen, denen dieser Klasse zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-193">All schools that this class is associated with.</span></span> <span data-ttu-id="ebd4f-194">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-194">Nullable.</span></span>|
|<span data-ttu-id="ebd4f-195">teachers</span><span class="sxs-lookup"><span data-stu-id="ebd4f-195">teachers</span></span>|<span data-ttu-id="ebd4f-196">[educationUser](../resources/educationuser.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ebd4f-196">[educationUser](../resources/educationuser.md) collection</span></span>|  <span data-ttu-id="ebd4f-197">Alle Lehrer in der Klasse.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-197">All teachers in the class.</span></span> <span data-ttu-id="ebd4f-198">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-198">Nullable.</span></span>|
|<span data-ttu-id="ebd4f-199">group</span><span class="sxs-lookup"><span data-stu-id="ebd4f-199">group</span></span>|[<span data-ttu-id="ebd4f-200">group</span><span class="sxs-lookup"><span data-stu-id="ebd4f-200">group</span></span>](../resources/group.md)| <span data-ttu-id="ebd4f-201">Die Directory-Gruppe, die diese Klasse entspricht.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-201">The directory group corresponding to this class.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ebd4f-202">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ebd4f-202">JSON representation</span></span>

<span data-ttu-id="ebd4f-203">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ebd4f-203">The following is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationClass"
}-->

```json
{
  "id": "String",
  "description": "String",
  "classCode": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "string",
  "mailNickname": "String",
  "term": {"@odata.type": "microsoft.graph.educationTerm"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationClass resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
