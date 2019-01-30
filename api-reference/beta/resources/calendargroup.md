---
title: calendarGroup-Ressourcentyp
description: Eine Gruppe der Benutzerkalender.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: cea68da3a91396972c4e237d1fdaf0e16d65e3a3
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643713"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="f4e5e-103">calendarGroup-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f4e5e-103">calendarGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4e5e-104">Eine Gruppe der Benutzerkalender.</span><span class="sxs-lookup"><span data-stu-id="f4e5e-104">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="f4e5e-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="f4e5e-105">Methods</span></span>

| <span data-ttu-id="f4e5e-106">Methode</span><span class="sxs-lookup"><span data-stu-id="f4e5e-106">Method</span></span>                                                      | <span data-ttu-id="f4e5e-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f4e5e-107">Return Type</span></span>                        | <span data-ttu-id="f4e5e-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f4e5e-108">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="f4e5e-109">Kalendergruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="f4e5e-109">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="f4e5e-110">[Kalendersammlung](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="f4e5e-110">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="f4e5e-111">Dient zum Abrufen der Kalendergruppen des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="f4e5e-111">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="f4e5e-112">Kalendergruppe erstellen</span><span class="sxs-lookup"><span data-stu-id="f4e5e-112">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="f4e5e-113">Kalender</span><span class="sxs-lookup"><span data-stu-id="f4e5e-113">Calendar</span></span>](calendar.md)            | <span data-ttu-id="f4e5e-114">Erstellt eine neue Kalendergruppe.</span><span class="sxs-lookup"><span data-stu-id="f4e5e-114">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="f4e5e-115">Kalendergruppe abrufen</span><span class="sxs-lookup"><span data-stu-id="f4e5e-115">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="f4e5e-116">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="f4e5e-116">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="f4e5e-117">Dient zum Lesen der Eigenschaften und der Beziehungen eines Kalendergruppenobjekts.</span><span class="sxs-lookup"><span data-stu-id="f4e5e-117">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="f4e5e-118">Update</span><span class="sxs-lookup"><span data-stu-id="f4e5e-118">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="f4e5e-119">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="f4e5e-119">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="f4e5e-120">Dient zum Aktualisieren des calendarGroup-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f4e5e-120">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="f4e5e-121">Löschen</span><span class="sxs-lookup"><span data-stu-id="f4e5e-121">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="f4e5e-122">Keine</span><span class="sxs-lookup"><span data-stu-id="f4e5e-122">None</span></span>                               | <span data-ttu-id="f4e5e-123">Dient zum Löschen des calendarGroup-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f4e5e-123">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="f4e5e-124">Kalender auflisten</span><span class="sxs-lookup"><span data-stu-id="f4e5e-124">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="f4e5e-125">[Kalendersammlung](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="f4e5e-125">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="f4e5e-126">Listet Kalender in einer Kalendergruppe auf.</span><span class="sxs-lookup"><span data-stu-id="f4e5e-126">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="f4e5e-127">Kalender erstellen</span><span class="sxs-lookup"><span data-stu-id="f4e5e-127">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="f4e5e-128">Kalender</span><span class="sxs-lookup"><span data-stu-id="f4e5e-128">Calendar</span></span>](calendar.md)            | <span data-ttu-id="f4e5e-129">Erstellt einen neuen Kalender in einer Kalendergruppe.</span><span class="sxs-lookup"><span data-stu-id="f4e5e-129">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="f4e5e-130">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f4e5e-130">Properties</span></span>

| <span data-ttu-id="f4e5e-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f4e5e-131">Property</span></span>  | <span data-ttu-id="f4e5e-132">Typ</span><span class="sxs-lookup"><span data-stu-id="f4e5e-132">Type</span></span>   | <span data-ttu-id="f4e5e-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f4e5e-133">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f4e5e-134">name</span><span class="sxs-lookup"><span data-stu-id="f4e5e-134">name</span></span>      | <span data-ttu-id="f4e5e-135">String</span><span class="sxs-lookup"><span data-stu-id="f4e5e-135">String</span></span> | <span data-ttu-id="f4e5e-136">Der Gruppenname.</span><span class="sxs-lookup"><span data-stu-id="f4e5e-136">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="f4e5e-137">changeKey</span><span class="sxs-lookup"><span data-stu-id="f4e5e-137">changeKey</span></span> | <span data-ttu-id="f4e5e-138">String</span><span class="sxs-lookup"><span data-stu-id="f4e5e-138">String</span></span> | <span data-ttu-id="f4e5e-p101">Gibt die Version der Kalendergruppe an. Jedes Mal, wenn die Kalendergruppe geändert wird, wird auch ChangeKey geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f4e5e-p101">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="f4e5e-143">classId</span><span class="sxs-lookup"><span data-stu-id="f4e5e-143">classId</span></span>   | <span data-ttu-id="f4e5e-144">Guid</span><span class="sxs-lookup"><span data-stu-id="f4e5e-144">Guid</span></span>   | <span data-ttu-id="f4e5e-p102">Die Klassen-ID. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f4e5e-p102">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="f4e5e-147">id</span><span class="sxs-lookup"><span data-stu-id="f4e5e-147">id</span></span>        | <span data-ttu-id="f4e5e-148">String</span><span class="sxs-lookup"><span data-stu-id="f4e5e-148">String</span></span> | <span data-ttu-id="f4e5e-p103">Eindeutiger Bezeichner für die Gruppe. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f4e5e-p103">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="f4e5e-151">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f4e5e-151">Relationships</span></span>

| <span data-ttu-id="f4e5e-152">Beziehung</span><span class="sxs-lookup"><span data-stu-id="f4e5e-152">Relationship</span></span> | <span data-ttu-id="f4e5e-153">Typ</span><span class="sxs-lookup"><span data-stu-id="f4e5e-153">Type</span></span>                               | <span data-ttu-id="f4e5e-154">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f4e5e-154">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="f4e5e-155">Kalender</span><span class="sxs-lookup"><span data-stu-id="f4e5e-155">calendars</span></span>    | <span data-ttu-id="f4e5e-156">[Kalendersammlung](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="f4e5e-156">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="f4e5e-p104">Die Kalender in Kalendergruppe. Navigation-Eigenschaft Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="f4e5e-p104">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f4e5e-161">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f4e5e-161">JSON representation</span></span>

<span data-ttu-id="f4e5e-162">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f4e5e-162">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "calendars"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendarGroup"
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
