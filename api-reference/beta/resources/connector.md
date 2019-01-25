---
title: Connector-Ressourcentyp
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: eed936c808e920f35a741a836a1fab64b2754bf8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525731"
---
# <a name="connector-resource-type"></a><span data-ttu-id="7b622-103">Connector-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7b622-103">connector resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a><span data-ttu-id="7b622-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="7b622-104">Methods</span></span>

| <span data-ttu-id="7b622-105">Methode</span><span class="sxs-lookup"><span data-stu-id="7b622-105">Method</span></span>           | <span data-ttu-id="7b622-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="7b622-106">Return Type</span></span>    |<span data-ttu-id="7b622-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b622-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7b622-108">Get-connector</span><span class="sxs-lookup"><span data-stu-id="7b622-108">Get connector</span></span>](../api/connector-get.md) | <span data-ttu-id="7b622-109">Connector</span><span class="sxs-lookup"><span data-stu-id="7b622-109">[connector](connector.md)</span></span> |<span data-ttu-id="7b622-110">Lesen Sie Eigenschaften und Beziehungen des Connector-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7b622-110">Read properties and relationships of connector object.</span></span>|
|[<span data-ttu-id="7b622-111">memberOf auflisten</span><span class="sxs-lookup"><span data-stu-id="7b622-111">List memberOf</span></span>](../api/connector-list-memberof.md) |<span data-ttu-id="7b622-112">[ConnectorGroup](connectorgroup.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="7b622-112">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="7b622-113">Ruft das ConnectorGroup-Objekt, das den Connector zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="7b622-113">Get the connectorGroup object associated with the connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="7b622-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7b622-114">Properties</span></span>
| <span data-ttu-id="7b622-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7b622-115">Property</span></span>     | <span data-ttu-id="7b622-116">Typ</span><span class="sxs-lookup"><span data-stu-id="7b622-116">Type</span></span>   |<span data-ttu-id="7b622-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b622-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b622-118">externalIp</span><span class="sxs-lookup"><span data-stu-id="7b622-118">externalIp</span></span>|<span data-ttu-id="7b622-119">String</span><span class="sxs-lookup"><span data-stu-id="7b622-119">String</span></span>|<span data-ttu-id="7b622-120">Externe IP-Adresse als ermittelte vom Dienst für den Connectorcomputer.</span><span class="sxs-lookup"><span data-stu-id="7b622-120">The external IP address as detected by the service for the connector machine.</span></span> <span data-ttu-id="7b622-121">Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="7b622-121">Read-only</span></span>|
|<span data-ttu-id="7b622-122">id</span><span class="sxs-lookup"><span data-stu-id="7b622-122">id</span></span>|<span data-ttu-id="7b622-123">String</span><span class="sxs-lookup"><span data-stu-id="7b622-123">String</span></span>| <span data-ttu-id="7b622-124">Die Objekt-Id der Verbindung.</span><span class="sxs-lookup"><span data-stu-id="7b622-124">The object id of the connector.</span></span> <BR><span data-ttu-id="7b622-125">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7b622-125">Read-only.</span></span>|
|<span data-ttu-id="7b622-126">Computername</span><span class="sxs-lookup"><span data-stu-id="7b622-126">machineName</span></span>|<span data-ttu-id="7b622-127">String</span><span class="sxs-lookup"><span data-stu-id="7b622-127">String</span></span>| <span data-ttu-id="7b622-128">Der Name des Computers, der der Connector ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="7b622-128">The name of the machine that the connector is running on.</span></span> <BR><span data-ttu-id="7b622-129">Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="7b622-129">Read-only</span></span>|
|<span data-ttu-id="7b622-130">status</span><span class="sxs-lookup"><span data-stu-id="7b622-130">status</span></span>|<span data-ttu-id="7b622-131">string</span><span class="sxs-lookup"><span data-stu-id="7b622-131">string</span></span>| <span data-ttu-id="7b622-132">Gibt den Status der Verbindung.</span><span class="sxs-lookup"><span data-stu-id="7b622-132">Indicates the status of the connector.</span></span> <span data-ttu-id="7b622-133">Mögliche Werte sind: `active` und `inactive`.</span><span class="sxs-lookup"><span data-stu-id="7b622-133">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="7b622-134">Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="7b622-134">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="7b622-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7b622-135">Relationships</span></span>
| <span data-ttu-id="7b622-136">Beziehung</span><span class="sxs-lookup"><span data-stu-id="7b622-136">Relationship</span></span> | <span data-ttu-id="7b622-137">Typ</span><span class="sxs-lookup"><span data-stu-id="7b622-137">Type</span></span>   |<span data-ttu-id="7b622-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b622-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b622-139">memberOf</span><span class="sxs-lookup"><span data-stu-id="7b622-139">memberOf</span></span>|<span data-ttu-id="7b622-140">[ConnectorGroup](connectorgroup.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="7b622-140">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="7b622-141">Die ConnectorGroup, die Verbindung herstellen, ein Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="7b622-141">The connectorGroup that the connect is a member of.</span></span><br><span data-ttu-id="7b622-142">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7b622-142">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7b622-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7b622-143">JSON representation</span></span>

<span data-ttu-id="7b622-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7b622-144">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "connector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/connector.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
