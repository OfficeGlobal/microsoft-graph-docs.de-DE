---
title: domainDnsUnavailableRecord-Ressourcentyp
description: Wenn Sie für die Navigation-Eigenschaft **ServiceConfigurationRecords** für eine Domänenentität Abfragen, erhalten Sie eventuell wieder eine oder mehrere DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord und/oder DomainDnsTxtRecord Entitäten. Diese Entitäten Geben Sie an, welche DNS-Einträge, die Sie in der Domäne, die Zonendatei hinzufügen müssen, bevor die Domäne von Microsoft Online Services verwendet werden kann. Wenn es nicht möglich, eine solche Entitäten generieren ist, wird stattdessen eine Entität DomainDnsUnavailableRecord zurückgegeben. Geerbt von DomainDnsRecord Entität.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5f033c39c9cf8dc11c2a41b0cedb0b8de5ce7736
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968176"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="29fa8-106">domainDnsUnavailableRecord-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="29fa8-106">domainDnsUnavailableRecord resource type</span></span>

<span data-ttu-id="29fa8-p102">Wenn Sie die Navigationseigenschaft **serviceConfigurationRecords** für eine [Domain](domain.md)-Entität abfragen, werden möglicherweise eine oder mehrere [DomainDnsCnameRecord](domaindnscnamerecord.md)-, [DomainDnsMxRecord](domaindnsmxrecord.md)-, [DomainDnsSrvRecord](domaindnssrvrecord.md)- und/oder [DomainDnsTxtRecord](domaindnstxtrecord.md)-Entitäten zurückgegeben. Diese Entitäten geben die DNS-Einträge an, die Sie der Zonendatei der Domäne hinzufügen müssen, bevor die Domäne von Microsoft-Onlinediensten verwendet werden kann. Wenn es nicht möglich ist, solche Entitäten zu generieren, wird stattdessen eine DomainDnsUnavailableRecord-Entität zurückgegeben. Geerbt von der Entität [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="29fa8-p102">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities. These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services. When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="29fa8-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="29fa8-111">Methods</span></span>
<span data-ttu-id="29fa8-p103">Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).</span><span class="sxs-lookup"><span data-stu-id="29fa8-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="29fa8-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="29fa8-114">Properties</span></span>
| <span data-ttu-id="29fa8-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="29fa8-115">Property</span></span>     | <span data-ttu-id="29fa8-116">Typ</span><span class="sxs-lookup"><span data-stu-id="29fa8-116">Type</span></span>   |<span data-ttu-id="29fa8-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="29fa8-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29fa8-118">description</span><span class="sxs-lookup"><span data-stu-id="29fa8-118">description</span></span>|<span data-ttu-id="29fa8-119">String</span><span class="sxs-lookup"><span data-stu-id="29fa8-119">String</span></span>|<span data-ttu-id="29fa8-120">Gibt den Grund an, warum die **DomainDnsUnavailableRecord**-Entität zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="29fa8-120">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="29fa8-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="29fa8-121">Relationships</span></span>
<span data-ttu-id="29fa8-122">Keine</span><span class="sxs-lookup"><span data-stu-id="29fa8-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29fa8-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="29fa8-123">JSON representation</span></span>
<span data-ttu-id="29fa8-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="29fa8-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "description": "String"
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
