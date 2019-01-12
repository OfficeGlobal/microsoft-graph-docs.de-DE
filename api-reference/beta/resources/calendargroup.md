---
title: calendarGroup-Ressourcentyp
description: Eine Gruppe der Benutzerkalender.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 10a840fd9ae9835eb5ca6a96b88719605f89245b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985291"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="0309b-103">calendarGroup-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0309b-103">calendarGroup resource type</span></span>

> <span data-ttu-id="0309b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0309b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0309b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0309b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0309b-106">Eine Gruppe der Benutzerkalender.</span><span class="sxs-lookup"><span data-stu-id="0309b-106">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="0309b-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="0309b-107">Methods</span></span>

| <span data-ttu-id="0309b-108">Methode</span><span class="sxs-lookup"><span data-stu-id="0309b-108">Method</span></span>                                                      | <span data-ttu-id="0309b-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0309b-109">Return Type</span></span>                        | <span data-ttu-id="0309b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0309b-110">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="0309b-111">Kalendergruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="0309b-111">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="0309b-112">[Kalendersammlung](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="0309b-112">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="0309b-113">Dient zum Abrufen der Kalendergruppen des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="0309b-113">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="0309b-114">Kalendergruppe erstellen</span><span class="sxs-lookup"><span data-stu-id="0309b-114">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="0309b-115">Kalender</span><span class="sxs-lookup"><span data-stu-id="0309b-115">Calendar</span></span>](calendar.md)            | <span data-ttu-id="0309b-116">Erstellt eine neue Kalendergruppe.</span><span class="sxs-lookup"><span data-stu-id="0309b-116">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="0309b-117">Kalendergruppe abrufen</span><span class="sxs-lookup"><span data-stu-id="0309b-117">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="0309b-118">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="0309b-118">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="0309b-119">Dient zum Lesen der Eigenschaften und der Beziehungen eines Kalendergruppenobjekts.</span><span class="sxs-lookup"><span data-stu-id="0309b-119">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="0309b-120">Update</span><span class="sxs-lookup"><span data-stu-id="0309b-120">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="0309b-121">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="0309b-121">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="0309b-122">Dient zum Aktualisieren des calendarGroup-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0309b-122">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="0309b-123">Löschen</span><span class="sxs-lookup"><span data-stu-id="0309b-123">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="0309b-124">Keine</span><span class="sxs-lookup"><span data-stu-id="0309b-124">None</span></span>                               | <span data-ttu-id="0309b-125">Dient zum Löschen des calendarGroup-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0309b-125">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="0309b-126">Kalender auflisten</span><span class="sxs-lookup"><span data-stu-id="0309b-126">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="0309b-127">[Kalendersammlung](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="0309b-127">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="0309b-128">Listet Kalender in einer Kalendergruppe auf.</span><span class="sxs-lookup"><span data-stu-id="0309b-128">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="0309b-129">Kalender erstellen</span><span class="sxs-lookup"><span data-stu-id="0309b-129">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="0309b-130">Kalender</span><span class="sxs-lookup"><span data-stu-id="0309b-130">Calendar</span></span>](calendar.md)            | <span data-ttu-id="0309b-131">Erstellt einen neuen Kalender in einer Kalendergruppe.</span><span class="sxs-lookup"><span data-stu-id="0309b-131">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="0309b-132">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0309b-132">Properties</span></span>

| <span data-ttu-id="0309b-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0309b-133">Property</span></span>  | <span data-ttu-id="0309b-134">Typ</span><span class="sxs-lookup"><span data-stu-id="0309b-134">Type</span></span>   | <span data-ttu-id="0309b-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0309b-135">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="0309b-136">name</span><span class="sxs-lookup"><span data-stu-id="0309b-136">name</span></span>      | <span data-ttu-id="0309b-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0309b-137">String</span></span> | <span data-ttu-id="0309b-138">Der Gruppenname.</span><span class="sxs-lookup"><span data-stu-id="0309b-138">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="0309b-139">changeKey</span><span class="sxs-lookup"><span data-stu-id="0309b-139">changeKey</span></span> | <span data-ttu-id="0309b-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0309b-140">String</span></span> | <span data-ttu-id="0309b-p102">Gibt die Version der Kalendergruppe an. Jedes Mal, wenn die Kalendergruppe geändert wird, wird auch ChangeKey geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0309b-p102">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="0309b-145">classId</span><span class="sxs-lookup"><span data-stu-id="0309b-145">classId</span></span>   | <span data-ttu-id="0309b-146">Guid</span><span class="sxs-lookup"><span data-stu-id="0309b-146">Guid</span></span>   | <span data-ttu-id="0309b-p103">Die Klassen-ID. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0309b-p103">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="0309b-149">id</span><span class="sxs-lookup"><span data-stu-id="0309b-149">id</span></span>        | <span data-ttu-id="0309b-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0309b-150">String</span></span> | <span data-ttu-id="0309b-p104">Eindeutiger Bezeichner für die Gruppe. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0309b-p104">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="0309b-153">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0309b-153">Relationships</span></span>

| <span data-ttu-id="0309b-154">Beziehung</span><span class="sxs-lookup"><span data-stu-id="0309b-154">Relationship</span></span> | <span data-ttu-id="0309b-155">Typ</span><span class="sxs-lookup"><span data-stu-id="0309b-155">Type</span></span>                               | <span data-ttu-id="0309b-156">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0309b-156">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="0309b-157">Kalender</span><span class="sxs-lookup"><span data-stu-id="0309b-157">calendars</span></span>    | <span data-ttu-id="0309b-158">[Kalendersammlung](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="0309b-158">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="0309b-p105">Die Kalender in Kalendergruppe. Navigation-Eigenschaft Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="0309b-p105">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0309b-163">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0309b-163">JSON representation</span></span>

<span data-ttu-id="0309b-164">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0309b-164">Here is a JSON representation of the resource</span></span>

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
