---
title: calendarGroup-Ressourcentyp
description: Eine Gruppe der Benutzerkalender.
author: angelgolfer-ms
ms.openlocfilehash: fda8a3006631f45d49e83363d61f7b0363675ed1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334370"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="2e722-103">calendarGroup-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2e722-103">calendarGroup resource type</span></span>

> <span data-ttu-id="2e722-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2e722-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2e722-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2e722-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2e722-106">Eine Gruppe der Benutzerkalender.</span><span class="sxs-lookup"><span data-stu-id="2e722-106">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="2e722-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="2e722-107">Methods</span></span>

| <span data-ttu-id="2e722-108">Methode</span><span class="sxs-lookup"><span data-stu-id="2e722-108">Method</span></span>                                                      | <span data-ttu-id="2e722-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="2e722-109">Return Type</span></span>                        | <span data-ttu-id="2e722-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e722-110">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="2e722-111">Kalendergruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="2e722-111">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="2e722-112">[Kalendersammlung](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="2e722-112">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="2e722-113">Dient zum Abrufen der Kalendergruppen des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="2e722-113">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="2e722-114">Kalendergruppe erstellen</span><span class="sxs-lookup"><span data-stu-id="2e722-114">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="2e722-115">Kalender</span><span class="sxs-lookup"><span data-stu-id="2e722-115">Calendar</span></span>](calendar.md)            | <span data-ttu-id="2e722-116">Erstellt eine neue Kalendergruppe.</span><span class="sxs-lookup"><span data-stu-id="2e722-116">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="2e722-117">Kalendergruppe abrufen</span><span class="sxs-lookup"><span data-stu-id="2e722-117">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="2e722-118">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="2e722-118">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="2e722-119">Dient zum Lesen der Eigenschaften und der Beziehungen eines Kalendergruppenobjekts.</span><span class="sxs-lookup"><span data-stu-id="2e722-119">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="2e722-120">Update</span><span class="sxs-lookup"><span data-stu-id="2e722-120">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="2e722-121">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="2e722-121">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="2e722-122">Dient zum Aktualisieren des calendarGroup-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2e722-122">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="2e722-123">Löschen</span><span class="sxs-lookup"><span data-stu-id="2e722-123">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="2e722-124">Keine</span><span class="sxs-lookup"><span data-stu-id="2e722-124">None</span></span>                               | <span data-ttu-id="2e722-125">Dient zum Löschen des calendarGroup-Objekts.</span><span class="sxs-lookup"><span data-stu-id="2e722-125">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="2e722-126">Kalender auflisten</span><span class="sxs-lookup"><span data-stu-id="2e722-126">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="2e722-127">[Kalendersammlung](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="2e722-127">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="2e722-128">Listet Kalender in einer Kalendergruppe auf.</span><span class="sxs-lookup"><span data-stu-id="2e722-128">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="2e722-129">Kalender erstellen</span><span class="sxs-lookup"><span data-stu-id="2e722-129">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="2e722-130">Kalender</span><span class="sxs-lookup"><span data-stu-id="2e722-130">Calendar</span></span>](calendar.md)            | <span data-ttu-id="2e722-131">Erstellt einen neuen Kalender in einer Kalendergruppe.</span><span class="sxs-lookup"><span data-stu-id="2e722-131">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="2e722-132">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2e722-132">Properties</span></span>

| <span data-ttu-id="2e722-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2e722-133">Property</span></span>  | <span data-ttu-id="2e722-134">Typ</span><span class="sxs-lookup"><span data-stu-id="2e722-134">Type</span></span>   | <span data-ttu-id="2e722-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e722-135">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="2e722-136">name</span><span class="sxs-lookup"><span data-stu-id="2e722-136">name</span></span>      | <span data-ttu-id="2e722-137">String</span><span class="sxs-lookup"><span data-stu-id="2e722-137">String</span></span> | <span data-ttu-id="2e722-138">Der Gruppenname.</span><span class="sxs-lookup"><span data-stu-id="2e722-138">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="2e722-139">changeKey</span><span class="sxs-lookup"><span data-stu-id="2e722-139">changeKey</span></span> | <span data-ttu-id="2e722-140">String</span><span class="sxs-lookup"><span data-stu-id="2e722-140">String</span></span> | <span data-ttu-id="2e722-p102">Gibt die Version der Kalendergruppe an. Jedes Mal, wenn die Kalendergruppe geändert wird, wird auch ChangeKey geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2e722-p102">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="2e722-145">classId</span><span class="sxs-lookup"><span data-stu-id="2e722-145">classId</span></span>   | <span data-ttu-id="2e722-146">Guid</span><span class="sxs-lookup"><span data-stu-id="2e722-146">Guid</span></span>   | <span data-ttu-id="2e722-p103">Die Klassen-ID. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2e722-p103">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="2e722-149">id</span><span class="sxs-lookup"><span data-stu-id="2e722-149">id</span></span>        | <span data-ttu-id="2e722-150">String</span><span class="sxs-lookup"><span data-stu-id="2e722-150">String</span></span> | <span data-ttu-id="2e722-p104">Eindeutiger Bezeichner für die Gruppe. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2e722-p104">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="2e722-153">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2e722-153">Relationships</span></span>

| <span data-ttu-id="2e722-154">Beziehung</span><span class="sxs-lookup"><span data-stu-id="2e722-154">Relationship</span></span> | <span data-ttu-id="2e722-155">Typ</span><span class="sxs-lookup"><span data-stu-id="2e722-155">Type</span></span>                               | <span data-ttu-id="2e722-156">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e722-156">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="2e722-157">Kalender</span><span class="sxs-lookup"><span data-stu-id="2e722-157">calendars</span></span>    | <span data-ttu-id="2e722-158">[Kalendersammlung](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="2e722-158">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="2e722-p105">Die Kalender in Kalendergruppe. Navigation-Eigenschaft Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="2e722-p105">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2e722-163">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2e722-163">JSON representation</span></span>

<span data-ttu-id="2e722-164">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2e722-164">Here is a JSON representation of the resource</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "calendarGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
