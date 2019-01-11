---
title: domainDnsRecord-Ressourcentyp
description: Für jede Domäne im Mandanten möglicherweise erforderliche DNS-Einträge in die DNS-Zonendatei der Domäne hinzufügen, bevor die Domäne von Microsoft Online Services verwendet werden kann. Die Entität **DomainDnsRecord** wird verwendet, um diese DNS-Einträge vorhanden. Basis Entität für DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord und DomainDnsSrvRecord-Entitäten.
localization_priority: Normal
ms.openlocfilehash: 30c5f63f4ecac2c716f7884ccf82fd129125c8b1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822344"
---
# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="f1d86-105">domainDnsRecord-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f1d86-105">domainDnsRecord resource type</span></span>

<span data-ttu-id="f1d86-p102">Möglicherweise müssen Sie für jede Domäne im Mandanten DNS-Einträge zur DNS-Zonendatei der Domäne hinzufügen, bevor die Domäne von Microsoft-Onlinediensten verwendet werden kann. Die **DomainDnsRecord**-Entität wird verwendet, um eine solche DNS-Einträge darzustellen. Basisentität für [DomainDnsCnameRecord](domaindnscnamerecord.md)-, [DomainDnsMxRecord](domaindnsmxrecord.md)-, [DomainDnsSrvRecord](domaindnssrvrecord.md)- und [DomainDnsSrvRecord](domaindnssrvrecord.md)-Entitäten.</span><span class="sxs-lookup"><span data-stu-id="f1d86-p102">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services. The **DomainDnsRecord** entity is used to present such DNS records. Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsSrvRecord](domaindnssrvrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="f1d86-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="f1d86-109">Methods</span></span>
<span data-ttu-id="f1d86-p103">Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).</span><span class="sxs-lookup"><span data-stu-id="f1d86-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="f1d86-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f1d86-112">Properties</span></span>
| <span data-ttu-id="f1d86-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f1d86-113">Property</span></span>     | <span data-ttu-id="f1d86-114">Typ</span><span class="sxs-lookup"><span data-stu-id="f1d86-114">Type</span></span>   |<span data-ttu-id="f1d86-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f1d86-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1d86-116">id</span><span class="sxs-lookup"><span data-stu-id="f1d86-116">id</span></span>|<span data-ttu-id="f1d86-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f1d86-117">String</span></span>| <span data-ttu-id="f1d86-p104">Eindeutiger Bezeichner, der dieser Entität zugewiesen ist. Lässt keine Nullwerte zu, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f1d86-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="f1d86-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="f1d86-120">isOptional</span></span>|<span data-ttu-id="f1d86-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1d86-121">Boolean</span></span>| <span data-ttu-id="f1d86-122">Wenn „false“, muss dieser Eintrag vom Kunden auf dem DNS-Host konfiguriert werden, damit Microsoft-Onlinedienste ordnungsgemäß mit der Domäne funktionieren.</span><span class="sxs-lookup"><span data-stu-id="f1d86-122">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="f1d86-123">label</span><span class="sxs-lookup"><span data-stu-id="f1d86-123">label</span></span>|<span data-ttu-id="f1d86-124">String</span><span class="sxs-lookup"><span data-stu-id="f1d86-124">String</span></span>| <span data-ttu-id="f1d86-125">Wert, der beim Konfigurieren des Namens des DNS-Eintrags auf dem DNS-Host verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="f1d86-125">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="f1d86-126">recordType</span><span class="sxs-lookup"><span data-stu-id="f1d86-126">recordType</span></span>|<span data-ttu-id="f1d86-127">String</span><span class="sxs-lookup"><span data-stu-id="f1d86-127">String</span></span>| <span data-ttu-id="f1d86-128">Gibt an, welche Art von DNS-Eintrag diese Entität darstellt.</span><span class="sxs-lookup"><span data-stu-id="f1d86-128">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="f1d86-129">Folgende Werte sind möglich: *CName*, *Mx*, *Srv*, *Txt*</span><span class="sxs-lookup"><span data-stu-id="f1d86-129">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="f1d86-130">Schlüssel</span><span class="sxs-lookup"><span data-stu-id="f1d86-130">Key</span></span> |
|<span data-ttu-id="f1d86-131">supportedService</span><span class="sxs-lookup"><span data-stu-id="f1d86-131">supportedService</span></span>|<span data-ttu-id="f1d86-132">String</span><span class="sxs-lookup"><span data-stu-id="f1d86-132">String</span></span>| <span data-ttu-id="f1d86-133">Microsoft-Onlinedienst oder Feature mit Abhängigkeit von diesem DNS-Eintrag.</span><span class="sxs-lookup"><span data-stu-id="f1d86-133">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="f1d86-134">Kann einer der folgenden Werte sein: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="f1d86-134">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="f1d86-135">ttl</span><span class="sxs-lookup"><span data-stu-id="f1d86-135">ttl</span></span>|<span data-ttu-id="f1d86-136">Int32</span><span class="sxs-lookup"><span data-stu-id="f1d86-136">Int32</span></span>| <span data-ttu-id="f1d86-p105">Wert, der beim Konfigurieren der Eigenschaft für die Gültigkeitsdauer (time-to-live (ttl)) des DNS-Eintrags auf dem DNS-Host verwendet werden soll. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="f1d86-p105">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="f1d86-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f1d86-139">Relationships</span></span>
<span data-ttu-id="f1d86-140">Keine</span><span class="sxs-lookup"><span data-stu-id="f1d86-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1d86-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f1d86-141">JSON representation</span></span>
<span data-ttu-id="f1d86-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f1d86-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
