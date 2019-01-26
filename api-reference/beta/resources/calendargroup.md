---
title: calendarGroup-Ressourcentyp
description: Eine Gruppe der Benutzerkalender.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a40b01136df2bb20a143a8de01188efaa2585191
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574796"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="e6192-103">calendarGroup-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e6192-103">calendarGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6192-104">Eine Gruppe der Benutzerkalender.</span><span class="sxs-lookup"><span data-stu-id="e6192-104">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="e6192-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="e6192-105">Methods</span></span>

| <span data-ttu-id="e6192-106">Methode</span><span class="sxs-lookup"><span data-stu-id="e6192-106">Method</span></span>                                                      | <span data-ttu-id="e6192-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e6192-107">Return Type</span></span>                        | <span data-ttu-id="e6192-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6192-108">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="e6192-109">Kalendergruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="e6192-109">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="e6192-110">[Kalendersammlung](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="e6192-110">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="e6192-111">Dient zum Abrufen der Kalendergruppen des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="e6192-111">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="e6192-112">Kalendergruppe erstellen</span><span class="sxs-lookup"><span data-stu-id="e6192-112">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="e6192-113">Kalender</span><span class="sxs-lookup"><span data-stu-id="e6192-113">Calendar</span></span>](calendar.md)            | <span data-ttu-id="e6192-114">Erstellt eine neue Kalendergruppe.</span><span class="sxs-lookup"><span data-stu-id="e6192-114">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="e6192-115">Kalendergruppe abrufen</span><span class="sxs-lookup"><span data-stu-id="e6192-115">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="e6192-116">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="e6192-116">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="e6192-117">Dient zum Lesen der Eigenschaften und der Beziehungen eines Kalendergruppenobjekts.</span><span class="sxs-lookup"><span data-stu-id="e6192-117">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="e6192-118">Update</span><span class="sxs-lookup"><span data-stu-id="e6192-118">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="e6192-119">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="e6192-119">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="e6192-120">Dient zum Aktualisieren des calendarGroup-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e6192-120">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="e6192-121">Löschen</span><span class="sxs-lookup"><span data-stu-id="e6192-121">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="e6192-122">Keine</span><span class="sxs-lookup"><span data-stu-id="e6192-122">None</span></span>                               | <span data-ttu-id="e6192-123">Dient zum Löschen des calendarGroup-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e6192-123">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="e6192-124">Kalender auflisten</span><span class="sxs-lookup"><span data-stu-id="e6192-124">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="e6192-125">[Kalendersammlung](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="e6192-125">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="e6192-126">Listet Kalender in einer Kalendergruppe auf.</span><span class="sxs-lookup"><span data-stu-id="e6192-126">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="e6192-127">Kalender erstellen</span><span class="sxs-lookup"><span data-stu-id="e6192-127">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="e6192-128">Kalender</span><span class="sxs-lookup"><span data-stu-id="e6192-128">Calendar</span></span>](calendar.md)            | <span data-ttu-id="e6192-129">Erstellt einen neuen Kalender in einer Kalendergruppe.</span><span class="sxs-lookup"><span data-stu-id="e6192-129">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="e6192-130">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e6192-130">Properties</span></span>

| <span data-ttu-id="e6192-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e6192-131">Property</span></span>  | <span data-ttu-id="e6192-132">Typ</span><span class="sxs-lookup"><span data-stu-id="e6192-132">Type</span></span>   | <span data-ttu-id="e6192-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6192-133">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e6192-134">name</span><span class="sxs-lookup"><span data-stu-id="e6192-134">name</span></span>      | <span data-ttu-id="e6192-135">String</span><span class="sxs-lookup"><span data-stu-id="e6192-135">String</span></span> | <span data-ttu-id="e6192-136">Der Gruppenname.</span><span class="sxs-lookup"><span data-stu-id="e6192-136">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="e6192-137">changeKey</span><span class="sxs-lookup"><span data-stu-id="e6192-137">changeKey</span></span> | <span data-ttu-id="e6192-138">String</span><span class="sxs-lookup"><span data-stu-id="e6192-138">String</span></span> | <span data-ttu-id="e6192-p101">Gibt die Version der Kalendergruppe an. Jedes Mal, wenn die Kalendergruppe geändert wird, wird auch ChangeKey geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e6192-p101">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="e6192-143">classId</span><span class="sxs-lookup"><span data-stu-id="e6192-143">classId</span></span>   | <span data-ttu-id="e6192-144">Guid</span><span class="sxs-lookup"><span data-stu-id="e6192-144">Guid</span></span>   | <span data-ttu-id="e6192-p102">Die Klassen-ID. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e6192-p102">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="e6192-147">id</span><span class="sxs-lookup"><span data-stu-id="e6192-147">id</span></span>        | <span data-ttu-id="e6192-148">String</span><span class="sxs-lookup"><span data-stu-id="e6192-148">String</span></span> | <span data-ttu-id="e6192-p103">Eindeutiger Bezeichner für die Gruppe. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e6192-p103">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="e6192-151">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e6192-151">Relationships</span></span>

| <span data-ttu-id="e6192-152">Beziehung</span><span class="sxs-lookup"><span data-stu-id="e6192-152">Relationship</span></span> | <span data-ttu-id="e6192-153">Typ</span><span class="sxs-lookup"><span data-stu-id="e6192-153">Type</span></span>                               | <span data-ttu-id="e6192-154">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6192-154">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="e6192-155">Kalender</span><span class="sxs-lookup"><span data-stu-id="e6192-155">calendars</span></span>    | <span data-ttu-id="e6192-156">[Kalendersammlung](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="e6192-156">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="e6192-p104">Die Kalender in Kalendergruppe. Navigation-Eigenschaft Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="e6192-p104">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e6192-161">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e6192-161">JSON representation</span></span>

<span data-ttu-id="e6192-162">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e6192-162">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "calendars"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.calendarGroup",
  "@odata.annotations": [
    {
      "property": "calendars",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "changeKey": "string",
  "classId": "guid",
  "id": "string (identifier)",
  "name": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "calendarGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/calendargroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
