---
title: domainDnsUnavailableRecord-Ressourcentyp
description: Wenn Sie für die Navigation-Eigenschaft **ServiceConfigurationRecords** für eine Domänenentität Abfragen, erhalten Sie eventuell wieder eine oder mehrere DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord und/oder DomainDnsTxtRecord Entitäten. Diese Entitäten Geben Sie an, welche DNS-Einträge, die Sie in der Domäne, die Zonendatei hinzufügen müssen, bevor die Domäne von Microsoft Online Services verwendet werden kann. Wenn es nicht möglich, eine solche Entitäten generieren ist, wird stattdessen eine Entität DomainDnsUnavailableRecord zurückgegeben. Geerbt von DomainDnsRecord Entität.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 99da0448d75375b84bb37c05102c1f702c222a25
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982792"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="0f10c-106">domainDnsUnavailableRecord-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0f10c-106">domainDnsUnavailableRecord resource type</span></span>

> <span data-ttu-id="0f10c-107">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0f10c-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f10c-108">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0f10c-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0f10c-p103">Wenn Sie die Navigationseigenschaft **serviceConfigurationRecords** für eine [Domain](domain.md)-Entität abfragen, werden möglicherweise eine oder mehrere [DomainDnsCnameRecord](domaindnscnamerecord.md)-, [DomainDnsMxRecord](domaindnsmxrecord.md)-, [DomainDnsSrvRecord](domaindnssrvrecord.md)- und/oder [DomainDnsTxtRecord](domaindnstxtrecord.md)-Entitäten zurückgegeben. Diese Entitäten geben die DNS-Einträge an, die Sie der Zonendatei der Domäne hinzufügen müssen, bevor die Domäne von Microsoft-Onlinediensten verwendet werden kann. Wenn es nicht möglich ist, solche Entitäten zu generieren, wird stattdessen eine DomainDnsUnavailableRecord-Entität zurückgegeben. Geerbt von der Entität [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="0f10c-p103">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities. These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services. When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="0f10c-113">Methoden</span><span class="sxs-lookup"><span data-stu-id="0f10c-113">Methods</span></span>
<span data-ttu-id="0f10c-p104">Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).</span><span class="sxs-lookup"><span data-stu-id="0f10c-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="0f10c-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0f10c-116">Properties</span></span>
| <span data-ttu-id="0f10c-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0f10c-117">Property</span></span>     | <span data-ttu-id="0f10c-118">Typ</span><span class="sxs-lookup"><span data-stu-id="0f10c-118">Type</span></span>   |<span data-ttu-id="0f10c-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f10c-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f10c-120">description</span><span class="sxs-lookup"><span data-stu-id="0f10c-120">description</span></span>|<span data-ttu-id="0f10c-121">String</span><span class="sxs-lookup"><span data-stu-id="0f10c-121">String</span></span>|<span data-ttu-id="0f10c-122">Gibt den Grund an, warum die **DomainDnsUnavailableRecord**-Entität zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="0f10c-122">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0f10c-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0f10c-123">Relationships</span></span>
<span data-ttu-id="0f10c-124">Keine</span><span class="sxs-lookup"><span data-stu-id="0f10c-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f10c-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0f10c-125">JSON representation</span></span>
<span data-ttu-id="0f10c-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0f10c-126">Here is a JSON representation of the resource.</span></span>

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
