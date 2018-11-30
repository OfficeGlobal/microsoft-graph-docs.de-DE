---
title: domainDnsUnavailableRecord-Ressourcentyp
description: Wenn Sie für die Navigation-Eigenschaft **ServiceConfigurationRecords** für eine Domänenentität Abfragen, erhalten Sie eventuell wieder eine oder mehrere DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord und/oder DomainDnsTxtRecord Entitäten. Diese Entitäten Geben Sie an, welche DNS-Einträge, die Sie in der Domäne, die Zonendatei hinzufügen müssen, bevor die Domäne von Microsoft Online Services verwendet werden kann. Wenn es nicht möglich, eine solche Entitäten generieren ist, wird stattdessen eine Entität DomainDnsUnavailableRecord zurückgegeben. Geerbt von DomainDnsRecord Entität.
ms.openlocfilehash: 0d920a2185cc84f5ca5cff571e1bb2c2d00400b5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058772"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="28340-106">domainDnsUnavailableRecord-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="28340-106">domainDnsUnavailableRecord resource type</span></span>

> <span data-ttu-id="28340-107">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="28340-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28340-108">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="28340-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="28340-p103">Wenn Sie die Navigationseigenschaft **serviceConfigurationRecords** für eine [Domain](domain.md)-Entität abfragen, werden möglicherweise eine oder mehrere [DomainDnsCnameRecord](domaindnscnamerecord.md)-, [DomainDnsMxRecord](domaindnsmxrecord.md)-, [DomainDnsSrvRecord](domaindnssrvrecord.md)- und/oder [DomainDnsTxtRecord](domaindnstxtrecord.md)-Entitäten zurückgegeben. Diese Entitäten geben die DNS-Einträge an, die Sie der Zonendatei der Domäne hinzufügen müssen, bevor die Domäne von Microsoft-Onlinediensten verwendet werden kann. Wenn es nicht möglich ist, solche Entitäten zu generieren, wird stattdessen eine DomainDnsUnavailableRecord-Entität zurückgegeben. Geerbt von der Entität [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="28340-p103">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities. These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services. When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="28340-113">Methoden</span><span class="sxs-lookup"><span data-stu-id="28340-113">Methods</span></span>
<span data-ttu-id="28340-p104">Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).</span><span class="sxs-lookup"><span data-stu-id="28340-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="28340-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="28340-116">Properties</span></span>
| <span data-ttu-id="28340-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="28340-117">Property</span></span>     | <span data-ttu-id="28340-118">Typ</span><span class="sxs-lookup"><span data-stu-id="28340-118">Type</span></span>   |<span data-ttu-id="28340-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28340-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28340-120">description</span><span class="sxs-lookup"><span data-stu-id="28340-120">description</span></span>|<span data-ttu-id="28340-121">String</span><span class="sxs-lookup"><span data-stu-id="28340-121">String</span></span>|<span data-ttu-id="28340-122">Gibt den Grund an, warum die **DomainDnsUnavailableRecord**-Entität zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="28340-122">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="28340-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="28340-123">Relationships</span></span>
<span data-ttu-id="28340-124">Keine</span><span class="sxs-lookup"><span data-stu-id="28340-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="28340-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="28340-125">JSON representation</span></span>
<span data-ttu-id="28340-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="28340-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "canonicalName": "String",
  "description": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "text": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->