---
title: Ressourcentyp connectorGroup
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 211efe5d8caae57457a6a5cc4fa95d145cd176f3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823191"
---
# <a name="connectorgroup-resource-type"></a><span data-ttu-id="e4414-103">Ressourcentyp connectorGroup</span><span class="sxs-lookup"><span data-stu-id="e4414-103">connectorGroup resource type</span></span>

> <span data-ttu-id="e4414-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e4414-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4414-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e4414-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="methods"></a><span data-ttu-id="e4414-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="e4414-106">Methods</span></span>

| <span data-ttu-id="e4414-107">Methode</span><span class="sxs-lookup"><span data-stu-id="e4414-107">Method</span></span>           | <span data-ttu-id="e4414-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e4414-108">Return Type</span></span>    |<span data-ttu-id="e4414-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4414-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e4414-110">Abrufen von connectorGroup</span><span class="sxs-lookup"><span data-stu-id="e4414-110">Get connectorGroup</span></span>](../api/connectorgroup-get.md) | [<span data-ttu-id="e4414-111">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="e4414-111">connectorGroup</span></span>](connectorgroup.md) |<span data-ttu-id="e4414-112">Lesen Sie Eigenschaften und Beziehungen des ConnectorGroup-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e4414-112">Read properties and relationships of connectorGroup object.</span></span>|
|[<span data-ttu-id="e4414-113">Erstellen der Anwendung</span><span class="sxs-lookup"><span data-stu-id="e4414-113">Create application</span></span>](../api/connectorgroup-post-applications.md) |[<span data-ttu-id="e4414-114">application</span><span class="sxs-lookup"><span data-stu-id="e4414-114">application</span></span>](application.md)| <span data-ttu-id="e4414-115">Ordnen Sie eine Anwendung mit der Connector-Gruppe durch das Veröffentlichen in der Auflistung Applications.</span><span class="sxs-lookup"><span data-stu-id="e4414-115">Associate an application with the connector group by posting to the applications collection.</span></span>|
|[<span data-ttu-id="e4414-116">Liste applications</span><span class="sxs-lookup"><span data-stu-id="e4414-116">List applications</span></span>](../api/connectorgroup-list-applications.md) |<span data-ttu-id="e4414-117">[Application](application.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="e4414-117">[application](application.md) collection</span></span>| <span data-ttu-id="e4414-118">Ruft die Auflistung der verbundenen Anwendung-Objekt.</span><span class="sxs-lookup"><span data-stu-id="e4414-118">Get the associated application object collection.</span></span>|
|[<span data-ttu-id="e4414-119">Erstellen Sie connector</span><span class="sxs-lookup"><span data-stu-id="e4414-119">Create connector</span></span>](../api/connectorgroup-post-members.md) |[<span data-ttu-id="e4414-120">Connector</span><span class="sxs-lookup"><span data-stu-id="e4414-120">connector</span></span>](connector.md)| <span data-ttu-id="e4414-121">Hinzufügen einer Verbindung an den Konnektor Gruppe durch die Veröffentlichung auf die Members-Auflistung.</span><span class="sxs-lookup"><span data-stu-id="e4414-121">Add a connector to the connector Group by posting to the members collection.</span></span>|
|[<span data-ttu-id="e4414-122">Mitglieder auflisten</span><span class="sxs-lookup"><span data-stu-id="e4414-122">List members</span></span>](../api/connectorgroup-list-members.md) |<span data-ttu-id="e4414-123">[Connector](connector.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="e4414-123">[connector](connector.md) collection</span></span>| <span data-ttu-id="e4414-124">Rufen Sie einen Connector-Auflistung-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e4414-124">Get a connector object collection.</span></span>|
|[<span data-ttu-id="e4414-125">Update</span><span class="sxs-lookup"><span data-stu-id="e4414-125">Update</span></span>](../api/connectorgroup-update.md) | [<span data-ttu-id="e4414-126">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="e4414-126">connectorGroup</span></span>](connectorgroup.md)    |<span data-ttu-id="e4414-127">ConnectorGroup-Objekt zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="e4414-127">Update connectorGroup object.</span></span> |
|[<span data-ttu-id="e4414-128">Delete</span><span class="sxs-lookup"><span data-stu-id="e4414-128">Delete</span></span>](../api/connectorgroup-delete.md) | <span data-ttu-id="e4414-129">Keine</span><span class="sxs-lookup"><span data-stu-id="e4414-129">None</span></span> |<span data-ttu-id="e4414-130">ConnectorGroup-Objekt zu löschen.</span><span class="sxs-lookup"><span data-stu-id="e4414-130">Delete connectorGroup object.</span></span> <span data-ttu-id="e4414-131">Sämtliche Verbinder muss entfernen, bevor eine Gruppe Connector gelöscht werden kann.</span><span class="sxs-lookup"><span data-stu-id="e4414-131">All connectors must be remove before a conector group can be deleted.</span></span> |

## <a name="properties"></a><span data-ttu-id="e4414-132">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e4414-132">Properties</span></span>
| <span data-ttu-id="e4414-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e4414-133">Property</span></span>     | <span data-ttu-id="e4414-134">Typ</span><span class="sxs-lookup"><span data-stu-id="e4414-134">Type</span></span>   |<span data-ttu-id="e4414-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4414-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4414-136">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="e4414-136">connectorGroupType</span></span>|<span data-ttu-id="e4414-137">string</span><span class="sxs-lookup"><span data-stu-id="e4414-137">string</span></span>| <span data-ttu-id="e4414-138">Der Typ des Connectors, die mit der Gruppe verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="e4414-138">The type of connectors that will be used with the group.</span></span> <span data-ttu-id="e4414-139">Mögliche Werte sind: `applicationProxy`.</span><span class="sxs-lookup"><span data-stu-id="e4414-139">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="e4414-140">id</span><span class="sxs-lookup"><span data-stu-id="e4414-140">id</span></span>|<span data-ttu-id="e4414-141">String</span><span class="sxs-lookup"><span data-stu-id="e4414-141">String</span></span>| <span data-ttu-id="e4414-142">Die Objekt-Id der connectorGroup</span><span class="sxs-lookup"><span data-stu-id="e4414-142">The object id of the connectorGroup</span></span>|
|<span data-ttu-id="e4414-143">isDefault</span><span class="sxs-lookup"><span data-stu-id="e4414-143">isDefault</span></span>|<span data-ttu-id="e4414-144">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e4414-144">Boolean</span></span>| <span data-ttu-id="e4414-145">Gibt an, ob die ConnectorGroup der Standardgruppe Connector.</span><span class="sxs-lookup"><span data-stu-id="e4414-145">Indicates if the connectorGroup is the default connector group.</span></span> <span data-ttu-id="e4414-146">Nur ein einzelner Connector Gruppe kann die Standard-ConnectorGroup und wird vom System festgelegt.</span><span class="sxs-lookup"><span data-stu-id="e4414-146">Only a single connector Group can be the default connectorGroup and is set by the system.</span></span>|
|<span data-ttu-id="e4414-147">name</span><span class="sxs-lookup"><span data-stu-id="e4414-147">name</span></span>|<span data-ttu-id="e4414-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4414-148">String</span></span>| <span data-ttu-id="e4414-149">Der Name der ConnectorGroup zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="e4414-149">The name associated with the connectorGroup.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4414-150">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e4414-150">Relationships</span></span>
| <span data-ttu-id="e4414-151">Beziehung</span><span class="sxs-lookup"><span data-stu-id="e4414-151">Relationship</span></span> | <span data-ttu-id="e4414-152">Typ</span><span class="sxs-lookup"><span data-stu-id="e4414-152">Type</span></span>   |<span data-ttu-id="e4414-153">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4414-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4414-154">Anwendungen</span><span class="sxs-lookup"><span data-stu-id="e4414-154">applications</span></span>|<span data-ttu-id="e4414-155">[Application](application.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="e4414-155">[application](application.md) collection</span></span>| <span data-ttu-id="e4414-p105">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="e4414-p105">Read-only. Nullable.</span></span>|
|<span data-ttu-id="e4414-158">Elemente</span><span class="sxs-lookup"><span data-stu-id="e4414-158">members</span></span>|<span data-ttu-id="e4414-159">[Connector](connector.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="e4414-159">[connector](connector.md) collection</span></span>| <span data-ttu-id="e4414-p106">Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="e4414-p106">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e4414-162">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e4414-162">JSON representation</span></span>

<span data-ttu-id="e4414-163">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e4414-163">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
