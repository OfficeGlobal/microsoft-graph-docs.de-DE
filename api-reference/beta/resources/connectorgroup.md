---
title: Ressourcentyp connectorGroup
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: de405d2f0cbe0417271ab54e66c5c30073d8ee7f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517498"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="adb58-103">Ressourcentyp connectorGroup</span><span class="sxs-lookup"><span data-stu-id="adb58-103">connectorGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a><span data-ttu-id="adb58-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="adb58-104">Methods</span></span>

| <span data-ttu-id="adb58-105">Methode</span><span class="sxs-lookup"><span data-stu-id="adb58-105">Method</span></span>           | <span data-ttu-id="adb58-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="adb58-106">Return Type</span></span>    |<span data-ttu-id="adb58-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="adb58-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="adb58-108">Abrufen von connectorGroup</span><span class="sxs-lookup"><span data-stu-id="adb58-108">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="adb58-109">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="adb58-109">connectorGroup</span></span>](connectorgroup.md) |<span data-ttu-id="adb58-110">Lesen Sie Eigenschaften und Beziehungen des ConnectorGroup-Objekts.</span><span class="sxs-lookup"><span data-stu-id="adb58-110">Read properties and relationships of connectorGroup object.</span></span>|
|[<span data-ttu-id="adb58-111">Erstellen der Anwendung</span><span class="sxs-lookup"><span data-stu-id="adb58-111">Create application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="adb58-112">application</span><span class="sxs-lookup"><span data-stu-id="adb58-112">application</span></span>](application.md)| <span data-ttu-id="adb58-113">Ordnen Sie eine Anwendung mit der Connector-Gruppe durch das Veröffentlichen in der Auflistung Applications.</span><span class="sxs-lookup"><span data-stu-id="adb58-113">Associate an application with the connector group by posting to the applications collection.</span></span>|
|[<span data-ttu-id="adb58-114">Liste applications</span><span class="sxs-lookup"><span data-stu-id="adb58-114">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="adb58-115">[Application](application.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="adb58-115">[application](application.md) collection</span></span>| <span data-ttu-id="adb58-116">Ruft die Auflistung der verbundenen Anwendung-Objekt.</span><span class="sxs-lookup"><span data-stu-id="adb58-116">Get the associated application object collection.</span></span>|
|[<span data-ttu-id="adb58-117">Erstellen Sie connector</span><span class="sxs-lookup"><span data-stu-id="adb58-117">Create connector</span></span>](../api/connectorgroup-post-members.md) |<span data-ttu-id="adb58-118">Connector</span><span class="sxs-lookup"><span data-stu-id="adb58-118">[connector](connector.md)</span></span>| <span data-ttu-id="adb58-119">Hinzufügen einer Verbindung an den Konnektor Gruppe durch die Veröffentlichung auf die Members-Auflistung.</span><span class="sxs-lookup"><span data-stu-id="adb58-119">Add a connector to the connector Group by posting to the members collection.</span></span>|
|[<span data-ttu-id="adb58-120">Mitglieder auflisten</span><span class="sxs-lookup"><span data-stu-id="adb58-120">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="adb58-121">[Connector](connector.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="adb58-121">[connector](connector.md) collection</span></span>| <span data-ttu-id="adb58-122">Rufen Sie einen Connector-Auflistung-Objekts.</span><span class="sxs-lookup"><span data-stu-id="adb58-122">Get a connector object collection.</span></span>|
|[<span data-ttu-id="adb58-123">Update</span><span class="sxs-lookup"><span data-stu-id="adb58-123">Update</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="adb58-124">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="adb58-124">connectorGroup</span></span>](connectorgroup.md)    |<span data-ttu-id="adb58-125">ConnectorGroup-Objekt zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="adb58-125">Update connectorGroup object.</span></span> |
|[<span data-ttu-id="adb58-126">Delete</span><span class="sxs-lookup"><span data-stu-id="adb58-126">Delete</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="adb58-127">Keine</span><span class="sxs-lookup"><span data-stu-id="adb58-127">None</span></span> |<span data-ttu-id="adb58-128">ConnectorGroup-Objekt zu löschen.</span><span class="sxs-lookup"><span data-stu-id="adb58-128">Delete connectorGroup object.</span></span> <span data-ttu-id="adb58-129">Sämtliche Verbinder muss entfernen, bevor eine Gruppe Connector gelöscht werden kann.</span><span class="sxs-lookup"><span data-stu-id="adb58-129">All connectors must be remove before a conector group can be deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="adb58-130">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="adb58-130">Properties</span></span>
| <span data-ttu-id="adb58-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="adb58-131">Property</span></span>     | <span data-ttu-id="adb58-132">Typ</span><span class="sxs-lookup"><span data-stu-id="adb58-132">Type</span></span>   |<span data-ttu-id="adb58-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="adb58-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="adb58-134">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="adb58-134">connectorGroupType</span></span>|<span data-ttu-id="adb58-135">string</span><span class="sxs-lookup"><span data-stu-id="adb58-135">string</span></span>| <span data-ttu-id="adb58-136">Der Typ des Connectors, die mit der Gruppe verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="adb58-136">The type of connectors that will be used with the group.</span></span> <span data-ttu-id="adb58-137">Mögliche Werte sind: `applicationProxy`.</span><span class="sxs-lookup"><span data-stu-id="adb58-137">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="adb58-138">id</span><span class="sxs-lookup"><span data-stu-id="adb58-138">id</span></span>|<span data-ttu-id="adb58-139">String</span><span class="sxs-lookup"><span data-stu-id="adb58-139">String</span></span>| <span data-ttu-id="adb58-140">Die Objekt-Id der connectorGroup</span><span class="sxs-lookup"><span data-stu-id="adb58-140">The object id of the connectorGroup</span></span>|
|<span data-ttu-id="adb58-141">isDefault</span><span class="sxs-lookup"><span data-stu-id="adb58-141">isDefault</span></span>|<span data-ttu-id="adb58-142">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="adb58-142">Boolean</span></span>| <span data-ttu-id="adb58-143">Gibt an, ob die ConnectorGroup der Standardgruppe Connector.</span><span class="sxs-lookup"><span data-stu-id="adb58-143">Indicates if the connectorGroup is the default connector group.</span></span> <span data-ttu-id="adb58-144">Nur ein einzelner Connector Gruppe kann die Standard-ConnectorGroup und wird vom System festgelegt.</span><span class="sxs-lookup"><span data-stu-id="adb58-144">Only a single connector Group can be the default connectorGroup and is set by the system.</span></span>|
|<span data-ttu-id="adb58-145">name</span><span class="sxs-lookup"><span data-stu-id="adb58-145">name</span></span>|<span data-ttu-id="adb58-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="adb58-146">String</span></span>| <span data-ttu-id="adb58-147">Der Name der ConnectorGroup zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="adb58-147">The name associated with the connectorGroup.</span></span>|

## <a name="relationships"></a><span data-ttu-id="adb58-148">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="adb58-148">Relationships</span></span>
| <span data-ttu-id="adb58-149">Beziehung</span><span class="sxs-lookup"><span data-stu-id="adb58-149">Relationship</span></span> | <span data-ttu-id="adb58-150">Typ</span><span class="sxs-lookup"><span data-stu-id="adb58-150">Type</span></span>   |<span data-ttu-id="adb58-151">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="adb58-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="adb58-152">Anwendungen</span><span class="sxs-lookup"><span data-stu-id="adb58-152">applications</span></span>|<span data-ttu-id="adb58-153">[Application](application.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="adb58-153">[application](application.md) collection</span></span>| <span data-ttu-id="adb58-p104">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="adb58-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="adb58-156">members</span><span class="sxs-lookup"><span data-stu-id="adb58-156">members</span></span>|<span data-ttu-id="adb58-157">[Connector](connector.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="adb58-157">[connector](connector.md) collection</span></span>| <span data-ttu-id="adb58-p105">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="adb58-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="adb58-160">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="adb58-160">JSON representation</span></span>

<span data-ttu-id="adb58-161">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="adb58-161">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectorGroup"
}-->

```json
{
  "connectorGroupType": "string",
  "id": "String (identifier)",
  "isDefault": true,
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/connectorgroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
