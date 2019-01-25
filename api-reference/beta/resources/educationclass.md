---
title: educationClass-Ressourcentyp
description: 'Stellt eine Klasse in einer Schule dar. Die **educationClass**-Ressource entspricht der Office 365-Gruppe und hat die gleiche ID. Kursteilnehmer sind reguläre Mitglieder der Klasse, Lehrer sind Besitzer und verfügen über entsprechende Rechte. Damit Office-Benutzeroberflächen ordnungsgemäß funktionieren, müssen Lehrer Mitglieder der Sammlungen der Lehrkräfte wie auch der Mitglieder sein.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 5a4bbc0560f2a40b5a438ec8276bbcf984a22721
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526732"
---
# <a name="educationclass-resource-type"></a><span data-ttu-id="aa086-106">educationClass-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="aa086-106">educationClass resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa086-107">Stellt eine Klasse in einer Schule dar.</span><span class="sxs-lookup"><span data-stu-id="aa086-107">Represents a class within a school.</span></span> <span data-ttu-id="aa086-108">Die **educationClass**-Ressource entspricht der Office 365-Gruppe und hat die gleiche ID.</span><span class="sxs-lookup"><span data-stu-id="aa086-108">The **educationClass** resource corresponds to the Office 365 group and shares the same ID.</span></span> <span data-ttu-id="aa086-109">Kursteilnehmer sind reguläre Mitglieder der Klasse, Lehrer sind Besitzer und verfügen über entsprechende Rechte.</span><span class="sxs-lookup"><span data-stu-id="aa086-109">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="aa086-110">Damit Office-Benutzeroberflächen ordnungsgemäß funktionieren, müssen Lehrer Mitglieder der Sammlungen der Lehrkräfte wie auch der Mitglieder sein.</span><span class="sxs-lookup"><span data-stu-id="aa086-110">For Office experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>  


## <a name="methods"></a><span data-ttu-id="aa086-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="aa086-111">Methods</span></span>

| <span data-ttu-id="aa086-112">Methode</span><span class="sxs-lookup"><span data-stu-id="aa086-112">Method</span></span>           | <span data-ttu-id="aa086-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="aa086-113">Return Type</span></span>    |<span data-ttu-id="aa086-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa086-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aa086-115">EducationClass abrufen</span><span class="sxs-lookup"><span data-stu-id="aa086-115">Get educationClass</span></span>](../api/educationclass-get.md) | [<span data-ttu-id="aa086-116">educationClass</span><span class="sxs-lookup"><span data-stu-id="aa086-116">educationClass</span></span>](educationclass.md) |<span data-ttu-id="aa086-117">Lesen von Eigenschaften und Beziehungen eines **educationClass**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="aa086-117">Read properties and relationships of an **educationClass** object.</span></span>|
|[<span data-ttu-id="aa086-118">Mitglied hinzufügen</span><span class="sxs-lookup"><span data-stu-id="aa086-118">Add member</span></span>](../api/educationclass-post-members.md) |[<span data-ttu-id="aa086-119">educationUser</span><span class="sxs-lookup"><span data-stu-id="aa086-119">educationUser</span></span>](educationuser.md)| <span data-ttu-id="aa086-120">Hinzufügen eines neuen **educationUser** für die Klasse durch Bereitstellen in der Navigationseigenschaft „members“.</span><span class="sxs-lookup"><span data-stu-id="aa086-120">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="aa086-121">Mitglieder auflisten</span><span class="sxs-lookup"><span data-stu-id="aa086-121">List members</span></span>](../api/educationclass-list-members.md) |<span data-ttu-id="aa086-122">[educationUser](educationuser.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="aa086-122">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="aa086-123">Abrufen einer **educationUser**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="aa086-123">Get an **educationUser** object collection.</span></span>|
|[<span data-ttu-id="aa086-124">Kursteilnehmer entfernen</span><span class="sxs-lookup"><span data-stu-id="aa086-124">Remove student</span></span>](../api/educationclass-delete-members.md) |[<span data-ttu-id="aa086-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="aa086-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="aa086-126">Entfernen eines **educationUser** aus der Klasse über die Navigationseigenschaft „members“.</span><span class="sxs-lookup"><span data-stu-id="aa086-126">Remove an **educationUser** from the class through the members navigation property.</span></span>|
|[<span data-ttu-id="aa086-127">Schulen auflisten</span><span class="sxs-lookup"><span data-stu-id="aa086-127">List schools</span></span>](../api/educationclass-list-schools.md) |<span data-ttu-id="aa086-128">[educationSchool](educationschool.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="aa086-128">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="aa086-129">Abrufen einer **educationSchool**-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="aa086-129">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="aa086-130">Lehrer hinzufügen</span><span class="sxs-lookup"><span data-stu-id="aa086-130">Add teacher</span></span>](../api/educationclass-post-teachers.md) |[<span data-ttu-id="aa086-131">educationUser</span><span class="sxs-lookup"><span data-stu-id="aa086-131">educationUser</span></span>](educationuser.md)| <span data-ttu-id="aa086-132">Hinzufügen eines neuen **educationUser** für die Klasse durch Bereitstellen in der Navigationseigenschaft „teachers“.</span><span class="sxs-lookup"><span data-stu-id="aa086-132">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span>|
|[<span data-ttu-id="aa086-133">Lehrer auflisten</span><span class="sxs-lookup"><span data-stu-id="aa086-133">List teachers</span></span>](../api/educationclass-list-teachers.md) |<span data-ttu-id="aa086-134">[educationUser](educationuser.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="aa086-134">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="aa086-135">Abrufen einer Liste der Lehrer für die Klasse</span><span class="sxs-lookup"><span data-stu-id="aa086-135">Get a list of teachers for the class.</span></span>|
|[<span data-ttu-id="aa086-136">Lehrer entfernen</span><span class="sxs-lookup"><span data-stu-id="aa086-136">Remove teacher</span></span>](../api/educationclass-delete-teachers.md) |[<span data-ttu-id="aa086-137">educationUser</span><span class="sxs-lookup"><span data-stu-id="aa086-137">educationUser</span></span>](educationuser.md)| <span data-ttu-id="aa086-138">Entfernen eines **educationUser** aus der Klasse über die Navigationseigenschaft „teachers“.</span><span class="sxs-lookup"><span data-stu-id="aa086-138">Remove an **educationUser** from the class through the teachers navigation property.</span></span>|
|[<span data-ttu-id="aa086-139">Erstellen von educationAssignment</span><span class="sxs-lookup"><span data-stu-id="aa086-139">Create educationAssignment</span></span>](../api/educationclass-post-assignments.md) |[<span data-ttu-id="aa086-140">educationAssignment</span><span class="sxs-lookup"><span data-stu-id="aa086-140">educationAssignment</span></span>](../resources/educationassignment.md)| <span data-ttu-id="aa086-141">Erstellen Sie eine neue **EducationAssignment** , durch die Veröffentlichung auf der Assignments-Auflistung.</span><span class="sxs-lookup"><span data-stu-id="aa086-141">Create a new **educationAssignment** by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="aa086-142">Liste Zuordnungen</span><span class="sxs-lookup"><span data-stu-id="aa086-142">List assignments</span></span>](../api/educationclass-list-assignments.md) |<span data-ttu-id="aa086-143">[EducationAssignment](../resources/educationassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="aa086-143">[educationAssignment](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="aa086-144">Rufen Sie eine Auflistung der **EducationAssignment** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="aa086-144">Get an **educationAssignment** object collection.</span></span>|
|[<span data-ttu-id="aa086-145">Gruppe abrufen</span><span class="sxs-lookup"><span data-stu-id="aa086-145">Get group</span></span>](../api/educationclass-get-group.md) |[<span data-ttu-id="aa086-146">group</span><span class="sxs-lookup"><span data-stu-id="aa086-146">group</span></span>](group.md)| <span data-ttu-id="aa086-147">Abrufen der Office 365-**Gruppe**, die dieser **educationClass** entspricht.</span><span class="sxs-lookup"><span data-stu-id="aa086-147">Get the Office 365 **group** that corresponds to this **educationClass**.</span></span>|
|[<span data-ttu-id="aa086-148">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="aa086-148">Update</span></span>](../api/educationclass-update.md) | [<span data-ttu-id="aa086-149">educationClass</span><span class="sxs-lookup"><span data-stu-id="aa086-149">educationClass</span></span>](educationclass.md)    |<span data-ttu-id="aa086-150">Aktualisieren eines **educationClass**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="aa086-150">Update **educationClass** object.</span></span> |
|[<span data-ttu-id="aa086-151">Löschen</span><span class="sxs-lookup"><span data-stu-id="aa086-151">Delete</span></span>](../api/educationclass-delete.md) | <span data-ttu-id="aa086-152">Keine</span><span class="sxs-lookup"><span data-stu-id="aa086-152">None</span></span> |<span data-ttu-id="aa086-153">Löschen eines **educationClass**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="aa086-153">Delete **educationClass** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="aa086-154">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="aa086-154">Properties</span></span>
| <span data-ttu-id="aa086-155">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aa086-155">Property</span></span>     | <span data-ttu-id="aa086-156">Typ</span><span class="sxs-lookup"><span data-stu-id="aa086-156">Type</span></span>   |<span data-ttu-id="aa086-157">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa086-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa086-158">id</span><span class="sxs-lookup"><span data-stu-id="aa086-158">id</span></span>| <span data-ttu-id="aa086-159">string</span><span class="sxs-lookup"><span data-stu-id="aa086-159">String</span></span>| <span data-ttu-id="aa086-160">Eindeutiger Bezeichner für die Klasse</span><span class="sxs-lookup"><span data-stu-id="aa086-160">Unique identifier for the class.</span></span>|
|<span data-ttu-id="aa086-161">description</span><span class="sxs-lookup"><span data-stu-id="aa086-161">description</span></span>|<span data-ttu-id="aa086-162">String</span><span class="sxs-lookup"><span data-stu-id="aa086-162">String</span></span>| <span data-ttu-id="aa086-163">Beschreibung der Klasse</span><span class="sxs-lookup"><span data-stu-id="aa086-163">Description of the class.</span></span>|
|<span data-ttu-id="aa086-164">displayName</span><span class="sxs-lookup"><span data-stu-id="aa086-164">displayName</span></span>|<span data-ttu-id="aa086-165">String</span><span class="sxs-lookup"><span data-stu-id="aa086-165">String</span></span>| <span data-ttu-id="aa086-166">Der Name der Klasse</span><span class="sxs-lookup"><span data-stu-id="aa086-166">Name of the class.</span></span>|
|<span data-ttu-id="aa086-167">mailNickname</span><span class="sxs-lookup"><span data-stu-id="aa086-167">mailNickname</span></span>|<span data-ttu-id="aa086-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="aa086-168">String</span></span>| <span data-ttu-id="aa086-169">E-Mail-Name zum Senden von E-Mails an alle Mitglieder, wenn diese Option aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="aa086-169">Mail name for sending email to all members, if this is enabled.</span></span> |
|<span data-ttu-id="aa086-170">createdBy</span><span class="sxs-lookup"><span data-stu-id="aa086-170">createdBy</span></span>|[<span data-ttu-id="aa086-171">identitySet</span><span class="sxs-lookup"><span data-stu-id="aa086-171">identitySet</span></span>](identityset.md)| <span data-ttu-id="aa086-172">Entität, die die Klasse erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="aa086-172">Entity who created the class</span></span> |
|<span data-ttu-id="aa086-173">classCode</span><span class="sxs-lookup"><span data-stu-id="aa086-173">classCode</span></span>|<span data-ttu-id="aa086-174">String</span><span class="sxs-lookup"><span data-stu-id="aa086-174">String</span></span>| <span data-ttu-id="aa086-175">Von der Schule verwendeter Klassencode zum Identifizieren der Klasse</span><span class="sxs-lookup"><span data-stu-id="aa086-175">Class code used by the school to identify the class.</span></span>|
|<span data-ttu-id="aa086-176">externalId</span><span class="sxs-lookup"><span data-stu-id="aa086-176">externalId</span></span>|<span data-ttu-id="aa086-177">String</span><span class="sxs-lookup"><span data-stu-id="aa086-177">String</span></span>| <span data-ttu-id="aa086-178">ID der Klasse aus dem Synchronisierungssystem</span><span class="sxs-lookup"><span data-stu-id="aa086-178">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="aa086-179">externalName</span><span class="sxs-lookup"><span data-stu-id="aa086-179">externalName</span></span>|<span data-ttu-id="aa086-180">String</span><span class="sxs-lookup"><span data-stu-id="aa086-180">String</span></span>|<span data-ttu-id="aa086-181">Der Name der Klasse im Synchronisierungssystem</span><span class="sxs-lookup"><span data-stu-id="aa086-181">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="aa086-182">externalSource</span><span class="sxs-lookup"><span data-stu-id="aa086-182">externalSource</span></span>|<span data-ttu-id="aa086-183">string</span><span class="sxs-lookup"><span data-stu-id="aa086-183">string</span></span>| <span data-ttu-id="aa086-184">Quelle, aus der diese Klasse erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="aa086-184">How this class was created.</span></span> <span data-ttu-id="aa086-185">Mögliche Werte sind: `sis`, `manual` und `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="aa086-185">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="aa086-186">term</span><span class="sxs-lookup"><span data-stu-id="aa086-186">term</span></span>|[<span data-ttu-id="aa086-187">educationTerm</span><span class="sxs-lookup"><span data-stu-id="aa086-187">educationTerm</span></span>](educationterm.md)|<span data-ttu-id="aa086-188">Der Zeitraum für diese Klasse.</span><span class="sxs-lookup"><span data-stu-id="aa086-188">Term for this class.</span></span>|


## <a name="relationships"></a><span data-ttu-id="aa086-189">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="aa086-189">Relationships</span></span>
| <span data-ttu-id="aa086-190">Beziehung</span><span class="sxs-lookup"><span data-stu-id="aa086-190">Relationship</span></span> | <span data-ttu-id="aa086-191">Typ</span><span class="sxs-lookup"><span data-stu-id="aa086-191">Type</span></span>   |<span data-ttu-id="aa086-192">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa086-192">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa086-193">members</span><span class="sxs-lookup"><span data-stu-id="aa086-193">members</span></span>|<span data-ttu-id="aa086-194">[educationUser](../resources/educationuser.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="aa086-194">[educationUser](../resources/educationuser.md) collection</span></span>| <span data-ttu-id="aa086-195">Alle Benutzer in der Klasse.</span><span class="sxs-lookup"><span data-stu-id="aa086-195">All users in the class.</span></span> <span data-ttu-id="aa086-196">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="aa086-196">Nullable.</span></span>|
|<span data-ttu-id="aa086-197">schools</span><span class="sxs-lookup"><span data-stu-id="aa086-197">schools</span></span>|<span data-ttu-id="aa086-198">[educationSchool](../resources/educationschool.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="aa086-198">[educationSchool](../resources/educationschool.md) collection</span></span>| <span data-ttu-id="aa086-199">Alle Schulen, denen dieser Klasse zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="aa086-199">All schools that this class is associated with.</span></span> <span data-ttu-id="aa086-200">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="aa086-200">Nullable.</span></span>|
|<span data-ttu-id="aa086-201">teachers</span><span class="sxs-lookup"><span data-stu-id="aa086-201">teachers</span></span>|<span data-ttu-id="aa086-202">[educationUser](../resources/educationuser.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="aa086-202">[educationUser](../resources/educationuser.md) collection</span></span>|  <span data-ttu-id="aa086-203">Alle Lehrer in der Klasse.</span><span class="sxs-lookup"><span data-stu-id="aa086-203">All teachers in the class.</span></span> <span data-ttu-id="aa086-204">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="aa086-204">Nullable.</span></span>|
|<span data-ttu-id="aa086-205">assignments</span><span class="sxs-lookup"><span data-stu-id="aa086-205">assignments</span></span>|<span data-ttu-id="aa086-206">[EducationAssignment](../resources/educationassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="aa086-206">[educationAssignment](../resources/educationassignment.md) collection</span></span>| <span data-ttu-id="aa086-207">Alle Aufgaben, die diese Klasse zugeordnet werden.</span><span class="sxs-lookup"><span data-stu-id="aa086-207">All assignments associated with this class.</span></span> <span data-ttu-id="aa086-208">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="aa086-208">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa086-209">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="aa086-209">JSON representation</span></span>

<span data-ttu-id="aa086-210">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="aa086-210">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "educationClass resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationclass.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
