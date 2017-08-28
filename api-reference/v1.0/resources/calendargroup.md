# <a name="calendargroup-resource-type"></a><span data-ttu-id="e0a3d-101">calendarGroup-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e0a3d-101">calendarGroup resource type</span></span>

<span data-ttu-id="e0a3d-102">Eine Gruppe von Kalendern.</span><span class="sxs-lookup"><span data-stu-id="e0a3d-102">A group of calendars.</span></span>

<span data-ttu-id="e0a3d-p101">**Hinweis** Outlook.com unterstützt nur die Standardkalendergruppe, auf die über „/me/calendars“ zugegriffen werden kann. Sie können diese Kalendergruppe nicht löschen.</span><span class="sxs-lookup"><span data-stu-id="e0a3d-p101">**Note** Outlook.com supports only the default calendar group which is accessible by the ../me/calendars shortcut. You cannot delete that calendar group.</span></span>

## <a name="methods"></a><span data-ttu-id="e0a3d-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="e0a3d-105">Methods</span></span>

| <span data-ttu-id="e0a3d-106">Methode</span><span class="sxs-lookup"><span data-stu-id="e0a3d-106">Method</span></span>       | <span data-ttu-id="e0a3d-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e0a3d-107">Return Type</span></span>  |<span data-ttu-id="e0a3d-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0a3d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e0a3d-109">Kalendergruppen auflisten</span><span class="sxs-lookup"><span data-stu-id="e0a3d-109">List calendar groups</span></span>](../api/user_list_calendargroups.md) |<span data-ttu-id="e0a3d-110">[Kalendersammlung](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="e0a3d-110">[Calendar](calendar.md) collection</span></span>| <span data-ttu-id="e0a3d-111">Dient zum Abrufen der Kalendergruppen des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="e0a3d-111">Get the user's calendar groups.</span></span>|
|[<span data-ttu-id="e0a3d-112">Kalendergruppe erstellen</span><span class="sxs-lookup"><span data-stu-id="e0a3d-112">Create calendar group</span></span>](../api/user_post_calendargroups.md) |[<span data-ttu-id="e0a3d-113">Kalender</span><span class="sxs-lookup"><span data-stu-id="e0a3d-113">Calendar</span></span>](calendar.md)| <span data-ttu-id="e0a3d-114">Erstellt eine neue Kalendergruppe.</span><span class="sxs-lookup"><span data-stu-id="e0a3d-114">Create a new calendar group.</span></span>|
|[<span data-ttu-id="e0a3d-115">Kalendergruppe abrufen</span><span class="sxs-lookup"><span data-stu-id="e0a3d-115">Get calendar group</span></span>](../api/calendargroup_get.md) | [<span data-ttu-id="e0a3d-116">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="e0a3d-116">calendarGroup</span></span>](calendargroup.md) |<span data-ttu-id="e0a3d-117">Dient zum Lesen der Eigenschaften und der Beziehungen eines Kalendergruppenobjekts.</span><span class="sxs-lookup"><span data-stu-id="e0a3d-117">Read properties and relationships of a calendar group object.</span></span>|
|[<span data-ttu-id="e0a3d-118">Update</span><span class="sxs-lookup"><span data-stu-id="e0a3d-118">Update</span></span>](../api/calendargroup_update.md) | [<span data-ttu-id="e0a3d-119">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="e0a3d-119">calendarGroup</span></span>](calendargroup.md) |<span data-ttu-id="e0a3d-120">Dient zum Aktualisieren des calendarGroup-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e0a3d-120">Update calendarGroup object.</span></span> |
|[<span data-ttu-id="e0a3d-121">Löschen</span><span class="sxs-lookup"><span data-stu-id="e0a3d-121">Delete</span></span>](../api/calendargroup_delete.md) | <span data-ttu-id="e0a3d-122">Keine</span><span class="sxs-lookup"><span data-stu-id="e0a3d-122">None</span></span> |<span data-ttu-id="e0a3d-123">Dient zum Löschen des calendarGroup-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e0a3d-123">Delete calendarGroup object.</span></span> |
|[<span data-ttu-id="e0a3d-124">Kalender auflisten</span><span class="sxs-lookup"><span data-stu-id="e0a3d-124">List calendars</span></span>](../api/calendargroup_list_calendars.md) |<span data-ttu-id="e0a3d-125">[Kalendersammlung](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="e0a3d-125">[Calendar](calendar.md) collection</span></span>| <span data-ttu-id="e0a3d-126">Listet Kalender in einer Kalendergruppe auf.</span><span class="sxs-lookup"><span data-stu-id="e0a3d-126">List calendars in a calendar group.</span></span>|
|[<span data-ttu-id="e0a3d-127">Kalender erstellen</span><span class="sxs-lookup"><span data-stu-id="e0a3d-127">Create Calendar</span></span>](../api/calendargroup_post_calendars.md) |[<span data-ttu-id="e0a3d-128">Kalender</span><span class="sxs-lookup"><span data-stu-id="e0a3d-128">Calendar</span></span>](calendar.md)| <span data-ttu-id="e0a3d-129">Erstellt einen neuen Kalender in einer Kalendergruppe.</span><span class="sxs-lookup"><span data-stu-id="e0a3d-129">Create a new Calendar in a calendar group.</span></span>|

## <a name="properties"></a><span data-ttu-id="e0a3d-130">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e0a3d-130">Properties</span></span>
| <span data-ttu-id="e0a3d-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e0a3d-131">Property</span></span>     | <span data-ttu-id="e0a3d-132">Typ</span><span class="sxs-lookup"><span data-stu-id="e0a3d-132">Type</span></span>   |<span data-ttu-id="e0a3d-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0a3d-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0a3d-134">name</span><span class="sxs-lookup"><span data-stu-id="e0a3d-134">name</span></span>|<span data-ttu-id="e0a3d-135">String</span><span class="sxs-lookup"><span data-stu-id="e0a3d-135">String</span></span>|<span data-ttu-id="e0a3d-136">Der Gruppenname.</span><span class="sxs-lookup"><span data-stu-id="e0a3d-136">The group name.</span></span>|
|<span data-ttu-id="e0a3d-137">changeKey</span><span class="sxs-lookup"><span data-stu-id="e0a3d-137">changeKey</span></span>|<span data-ttu-id="e0a3d-138">String</span><span class="sxs-lookup"><span data-stu-id="e0a3d-138">String</span></span>|<span data-ttu-id="e0a3d-p102">Gibt die Version der Kalendergruppe an. Jedes Mal, wenn die Kalendergruppe geändert wird, wird auch ChangeKey geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e0a3d-p102">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span>|
|<span data-ttu-id="e0a3d-143">classId</span><span class="sxs-lookup"><span data-stu-id="e0a3d-143">classId</span></span>|<span data-ttu-id="e0a3d-144">Guid</span><span class="sxs-lookup"><span data-stu-id="e0a3d-144">Guid</span></span>|<span data-ttu-id="e0a3d-p103">Die Klassen-ID. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e0a3d-p103">The class identifier. Read-only.</span></span>|
|<span data-ttu-id="e0a3d-147">id</span><span class="sxs-lookup"><span data-stu-id="e0a3d-147">id</span></span>|<span data-ttu-id="e0a3d-148">String</span><span class="sxs-lookup"><span data-stu-id="e0a3d-148">String</span></span>|<span data-ttu-id="e0a3d-p104">Eindeutiger Bezeichner für die Gruppe. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e0a3d-p104">The group's unique identifier. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0a3d-151">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e0a3d-151">Relationships</span></span>
| <span data-ttu-id="e0a3d-152">Beziehung</span><span class="sxs-lookup"><span data-stu-id="e0a3d-152">Relationship</span></span> | <span data-ttu-id="e0a3d-153">Typ</span><span class="sxs-lookup"><span data-stu-id="e0a3d-153">Type</span></span>   |<span data-ttu-id="e0a3d-154">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0a3d-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0a3d-155">Kalender</span><span class="sxs-lookup"><span data-stu-id="e0a3d-155">calendars</span></span>|<span data-ttu-id="e0a3d-156">[Kalendersammlung](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="e0a3d-156">[Calendar](calendar.md) collection</span></span>|<span data-ttu-id="e0a3d-p105">Die Kalender in Kalendergruppe. Navigation-Eigenschaft Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="e0a3d-p105">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e0a3d-161">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e0a3d-161">JSON representation</span></span>

<span data-ttu-id="e0a3d-162">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e0a3d-162">Here is a JSON representation of the resource</span></span>

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
