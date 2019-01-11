---
title: Connector-Ressourcentyp
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 98fa998a37b01ad64e556b229912932f4d1cfc75
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884623"
---
# <a name="connector-resource-type"></a><span data-ttu-id="c6eeb-103">Connector-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c6eeb-103">connector resource type</span></span>

> <span data-ttu-id="c6eeb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c6eeb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6eeb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c6eeb-105">Use of these APIs in production applications is not supported.</span></span>

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a><span data-ttu-id="c6eeb-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="c6eeb-106">Methods</span></span>

| <span data-ttu-id="c6eeb-107">Methode</span><span class="sxs-lookup"><span data-stu-id="c6eeb-107">Method</span></span>           | <span data-ttu-id="c6eeb-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="c6eeb-108">Return Type</span></span>    |<span data-ttu-id="c6eeb-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6eeb-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c6eeb-110">Get-connector</span><span class="sxs-lookup"><span data-stu-id="c6eeb-110">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="c6eeb-111">Connector</span><span class="sxs-lookup"><span data-stu-id="c6eeb-111">connector</span></span>](connector.md) |<span data-ttu-id="c6eeb-112">Lesen Sie Eigenschaften und Beziehungen des Connector-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c6eeb-112">Read properties and relationships of connector object.</span></span>|
|[<span data-ttu-id="c6eeb-113">memberOf auflisten</span><span class="sxs-lookup"><span data-stu-id="c6eeb-113">List memberOf</span></span>](../api/connector-list-memberof.md) |<span data-ttu-id="c6eeb-114">[ConnectorGroup](connectorgroup.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="c6eeb-114">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="c6eeb-115">Ruft das ConnectorGroup-Objekt, das den Connector zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="c6eeb-115">Get the connectorGroup object associated with the connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="c6eeb-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c6eeb-116">Properties</span></span>
| <span data-ttu-id="c6eeb-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c6eeb-117">Property</span></span>     | <span data-ttu-id="c6eeb-118">Typ</span><span class="sxs-lookup"><span data-stu-id="c6eeb-118">Type</span></span>   |<span data-ttu-id="c6eeb-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6eeb-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6eeb-120">externalIp</span><span class="sxs-lookup"><span data-stu-id="c6eeb-120">externalIp</span></span>|<span data-ttu-id="c6eeb-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c6eeb-121">String</span></span>|<span data-ttu-id="c6eeb-122">Externe IP-Adresse als ermittelte vom Dienst für den Connectorcomputer.</span><span class="sxs-lookup"><span data-stu-id="c6eeb-122">The external IP address as detected by the service for the connector machine.</span></span> <span data-ttu-id="c6eeb-123">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c6eeb-123">Read-only</span></span>|
|<span data-ttu-id="c6eeb-124">id</span><span class="sxs-lookup"><span data-stu-id="c6eeb-124">id</span></span>|<span data-ttu-id="c6eeb-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c6eeb-125">String</span></span>| <span data-ttu-id="c6eeb-126">Die Objekt-Id der Verbindung.</span><span class="sxs-lookup"><span data-stu-id="c6eeb-126">The object id of the connector.</span></span> <BR><span data-ttu-id="c6eeb-127">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c6eeb-127">Read-only.</span></span>|
|<span data-ttu-id="c6eeb-128">Computername</span><span class="sxs-lookup"><span data-stu-id="c6eeb-128">machineName</span></span>|<span data-ttu-id="c6eeb-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c6eeb-129">String</span></span>| <span data-ttu-id="c6eeb-130">Der Name des Computers, der der Connector ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="c6eeb-130">The name of the machine that the connector is running on.</span></span> <BR><span data-ttu-id="c6eeb-131">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c6eeb-131">Read-only</span></span>|
|<span data-ttu-id="c6eeb-132">status</span><span class="sxs-lookup"><span data-stu-id="c6eeb-132">status</span></span>|<span data-ttu-id="c6eeb-133">string</span><span class="sxs-lookup"><span data-stu-id="c6eeb-133">string</span></span>| <span data-ttu-id="c6eeb-134">Gibt den Status der Verbindung.</span><span class="sxs-lookup"><span data-stu-id="c6eeb-134">Indicates the status of the connector.</span></span> <span data-ttu-id="c6eeb-135">Mögliche Werte sind: `active` und `inactive`.</span><span class="sxs-lookup"><span data-stu-id="c6eeb-135">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="c6eeb-136">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c6eeb-136">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="c6eeb-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c6eeb-137">Relationships</span></span>
| <span data-ttu-id="c6eeb-138">Beziehung</span><span class="sxs-lookup"><span data-stu-id="c6eeb-138">Relationship</span></span> | <span data-ttu-id="c6eeb-139">Typ</span><span class="sxs-lookup"><span data-stu-id="c6eeb-139">Type</span></span>   |<span data-ttu-id="c6eeb-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6eeb-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6eeb-141">memberOf</span><span class="sxs-lookup"><span data-stu-id="c6eeb-141">memberOf</span></span>|<span data-ttu-id="c6eeb-142">[ConnectorGroup](connectorgroup.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="c6eeb-142">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="c6eeb-143">Die ConnectorGroup, die Verbindung herstellen, ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="c6eeb-143">The connectorGroup that the connect is a member of.</span></span><br><span data-ttu-id="c6eeb-144">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="c6eeb-144">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c6eeb-145">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c6eeb-145">JSON representation</span></span>

<span data-ttu-id="c6eeb-146">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c6eeb-146">Here is a JSON representation of the resource.</span></span>

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
