---
title: domainDnsRecord-Ressourcentyp
description: Für jede Domäne im Mandanten möglicherweise erforderliche DNS-Einträge in die DNS-Zonendatei der Domäne hinzufügen, bevor die Domäne von Microsoft Online Services verwendet werden kann. Die Entität **DomainDnsRecord** wird verwendet, um diese DNS-Einträge vorhanden. Basis Entität für DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord und DomainDnsSrvRecord-Entitäten.
ms.openlocfilehash: 766e3b241550ac1b0c7abdecaa22fe010955d05a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058872"
---
# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="9807b-105">domainDnsRecord-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9807b-105">domainDnsRecord resource type</span></span>

> <span data-ttu-id="9807b-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9807b-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9807b-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9807b-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9807b-p103">Möglicherweise müssen Sie für jede Domäne im Mandanten DNS-Einträge zur DNS-Zonendatei der Domäne hinzufügen, bevor die Domäne von Microsoft-Onlinediensten verwendet werden kann. Die **DomainDnsRecord**-Entität wird verwendet, um eine solche DNS-Einträge darzustellen. Basisentität für [DomainDnsCnameRecord](domaindnscnamerecord.md)-, [DomainDnsMxRecord](domaindnsmxrecord.md)-, [DomainDnsSrvRecord](domaindnssrvrecord.md)- und [DomainDnsSrvRecord](domaindnssrvrecord.md)-Entitäten.</span><span class="sxs-lookup"><span data-stu-id="9807b-p103">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services. The **DomainDnsRecord** entity is used to present such DNS records. Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsSrvRecord](domaindnssrvrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="9807b-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="9807b-111">Methods</span></span>
<span data-ttu-id="9807b-p104">Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).</span><span class="sxs-lookup"><span data-stu-id="9807b-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="9807b-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9807b-114">Properties</span></span>
| <span data-ttu-id="9807b-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9807b-115">Property</span></span>     | <span data-ttu-id="9807b-116">Typ</span><span class="sxs-lookup"><span data-stu-id="9807b-116">Type</span></span>   |<span data-ttu-id="9807b-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9807b-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9807b-118">id</span><span class="sxs-lookup"><span data-stu-id="9807b-118">id</span></span>|<span data-ttu-id="9807b-119">String</span><span class="sxs-lookup"><span data-stu-id="9807b-119">String</span></span>| <span data-ttu-id="9807b-p105">Eindeutiger Bezeichner, der dieser Entität zugewiesen ist. Lässt keine Nullwerte zu, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9807b-p105">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="9807b-122">isOptional</span><span class="sxs-lookup"><span data-stu-id="9807b-122">isOptional</span></span>|<span data-ttu-id="9807b-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="9807b-123">Boolean</span></span>| <span data-ttu-id="9807b-124">Wenn „false“, muss dieser Eintrag vom Kunden auf dem DNS-Host konfiguriert werden, damit Microsoft-Onlinedienste ordnungsgemäß mit der Domäne funktionieren.</span><span class="sxs-lookup"><span data-stu-id="9807b-124">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="9807b-125">label</span><span class="sxs-lookup"><span data-stu-id="9807b-125">label</span></span>|<span data-ttu-id="9807b-126">String</span><span class="sxs-lookup"><span data-stu-id="9807b-126">String</span></span>| <span data-ttu-id="9807b-127">Wert, der beim Konfigurieren des Namens des DNS-Eintrags auf dem DNS-Host verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="9807b-127">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="9807b-128">recordType</span><span class="sxs-lookup"><span data-stu-id="9807b-128">recordType</span></span>|<span data-ttu-id="9807b-129">String</span><span class="sxs-lookup"><span data-stu-id="9807b-129">String</span></span>| <span data-ttu-id="9807b-130">Gibt an, welche Art von DNS-Eintrag diese Entität darstellt.</span><span class="sxs-lookup"><span data-stu-id="9807b-130">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="9807b-131">Folgende Werte sind möglich: *CName*, *Mx*, *Srv*, *Txt*</span><span class="sxs-lookup"><span data-stu-id="9807b-131">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="9807b-132">Schlüssel</span><span class="sxs-lookup"><span data-stu-id="9807b-132">Key</span></span> |
|<span data-ttu-id="9807b-133">supportedService</span><span class="sxs-lookup"><span data-stu-id="9807b-133">supportedService</span></span>|<span data-ttu-id="9807b-134">String</span><span class="sxs-lookup"><span data-stu-id="9807b-134">String</span></span>| <span data-ttu-id="9807b-135">Microsoft-Onlinedienst oder Feature mit Abhängigkeit von diesem DNS-Eintrag.</span><span class="sxs-lookup"><span data-stu-id="9807b-135">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="9807b-136">Kann einer der folgenden Werte sein: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="9807b-136">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="9807b-137">ttl</span><span class="sxs-lookup"><span data-stu-id="9807b-137">ttl</span></span>|<span data-ttu-id="9807b-138">Int32</span><span class="sxs-lookup"><span data-stu-id="9807b-138">Int32</span></span>| <span data-ttu-id="9807b-p106">Wert, der beim Konfigurieren der Eigenschaft für die Gültigkeitsdauer (time-to-live (ttl)) des DNS-Eintrags auf dem DNS-Host verwendet werden soll. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="9807b-p106">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="9807b-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9807b-141">Relationships</span></span>
<span data-ttu-id="9807b-142">Keine</span><span class="sxs-lookup"><span data-stu-id="9807b-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9807b-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9807b-143">JSON representation</span></span>
<span data-ttu-id="9807b-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9807b-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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