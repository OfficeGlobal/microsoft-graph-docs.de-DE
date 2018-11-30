---
title: Connector-Ressourcentyp
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 6d4cb7e5ca1a5384dbb6c8be92e7ce4eb107388a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064598"
---
# <a name="connector-resource-type"></a><span data-ttu-id="16422-103">Connector-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="16422-103">connector resource type</span></span>

> <span data-ttu-id="16422-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="16422-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16422-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="16422-105">Use of these APIs in production applications is not supported.</span></span>

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a><span data-ttu-id="16422-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="16422-106">Methods</span></span>

| <span data-ttu-id="16422-107">Methode</span><span class="sxs-lookup"><span data-stu-id="16422-107">Method</span></span>           | <span data-ttu-id="16422-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="16422-108">Return Type</span></span>    |<span data-ttu-id="16422-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16422-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="16422-110">Get-connector</span><span class="sxs-lookup"><span data-stu-id="16422-110">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="16422-111">Connector</span><span class="sxs-lookup"><span data-stu-id="16422-111">connector</span></span>](connector.md) |<span data-ttu-id="16422-112">Lesen Sie Eigenschaften und Beziehungen des Connector-Objekts.</span><span class="sxs-lookup"><span data-stu-id="16422-112">Read properties and relationships of connector object.</span></span>|
|[<span data-ttu-id="16422-113">memberOf auflisten</span><span class="sxs-lookup"><span data-stu-id="16422-113">List memberOf</span></span>](../api/connector-list-memberof.md) |<span data-ttu-id="16422-114">[ConnectorGroup](connectorgroup.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="16422-114">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="16422-115">Ruft das ConnectorGroup-Objekt, das den Connector zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="16422-115">Get the connectorGroup object associated with the connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="16422-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="16422-116">Properties</span></span>
| <span data-ttu-id="16422-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="16422-117">Property</span></span>     | <span data-ttu-id="16422-118">Typ</span><span class="sxs-lookup"><span data-stu-id="16422-118">Type</span></span>   |<span data-ttu-id="16422-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16422-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16422-120">externalIp</span><span class="sxs-lookup"><span data-stu-id="16422-120">externalIp</span></span>|<span data-ttu-id="16422-121">String</span><span class="sxs-lookup"><span data-stu-id="16422-121">String</span></span>|<span data-ttu-id="16422-122">Externe IP-Adresse als ermittelte vom Dienst für den Connectorcomputer.</span><span class="sxs-lookup"><span data-stu-id="16422-122">The external IP address as detected by the service for the connector machine.</span></span> <span data-ttu-id="16422-123">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="16422-123">Read-only</span></span>|
|<span data-ttu-id="16422-124">id</span><span class="sxs-lookup"><span data-stu-id="16422-124">id</span></span>|<span data-ttu-id="16422-125">String</span><span class="sxs-lookup"><span data-stu-id="16422-125">String</span></span>| <span data-ttu-id="16422-126">Die Objekt-Id der Verbindung.</span><span class="sxs-lookup"><span data-stu-id="16422-126">The object id of the connector.</span></span> <BR><span data-ttu-id="16422-127">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="16422-127">Read-only.</span></span>|
|<span data-ttu-id="16422-128">Computername</span><span class="sxs-lookup"><span data-stu-id="16422-128">machineName</span></span>|<span data-ttu-id="16422-129">String</span><span class="sxs-lookup"><span data-stu-id="16422-129">String</span></span>| <span data-ttu-id="16422-130">Der Name des Computers, der der Connector ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="16422-130">The name of the machine that the connector is running on.</span></span> <BR><span data-ttu-id="16422-131">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="16422-131">Read-only</span></span>|
|<span data-ttu-id="16422-132">status</span><span class="sxs-lookup"><span data-stu-id="16422-132">status</span></span>|<span data-ttu-id="16422-133">string</span><span class="sxs-lookup"><span data-stu-id="16422-133">string</span></span>| <span data-ttu-id="16422-134">Gibt den Status der Verbindung.</span><span class="sxs-lookup"><span data-stu-id="16422-134">Indicates the status of the connector.</span></span> <span data-ttu-id="16422-135">Mögliche Werte sind: `active` und `inactive`.</span><span class="sxs-lookup"><span data-stu-id="16422-135">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="16422-136">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="16422-136">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="16422-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="16422-137">Relationships</span></span>
| <span data-ttu-id="16422-138">Beziehung</span><span class="sxs-lookup"><span data-stu-id="16422-138">Relationship</span></span> | <span data-ttu-id="16422-139">Typ</span><span class="sxs-lookup"><span data-stu-id="16422-139">Type</span></span>   |<span data-ttu-id="16422-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16422-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16422-141">memberOf</span><span class="sxs-lookup"><span data-stu-id="16422-141">memberOf</span></span>|<span data-ttu-id="16422-142">[ConnectorGroup](connectorgroup.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="16422-142">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="16422-143">Die ConnectorGroup, die Verbindung herstellen, ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="16422-143">The connectorGroup that the connect is a member of.</span></span><br><span data-ttu-id="16422-144">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="16422-144">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="16422-145">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="16422-145">JSON representation</span></span>

<span data-ttu-id="16422-146">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="16422-146">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connector"
}-->

```json
{
  "externalIp": "String",
  "id": "String (identifier)",
  "machineName": "String",
  "status": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
