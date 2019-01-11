---
title: domainDnsSrvRecord-Ressourcentyp
description: Stellt einen SRV-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität DomainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: c06682753b752980530bf8cfd8f6a32b9bbd569a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810437"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="18ba7-104">domainDnsSrvRecord-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="18ba7-104">domainDnsSrvRecord resource type</span></span>

> <span data-ttu-id="18ba7-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="18ba7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18ba7-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="18ba7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18ba7-p103">Stellt einen SRV-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="18ba7-p103">Represents a SRV record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="18ba7-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="18ba7-109">Methods</span></span>
<span data-ttu-id="18ba7-p104">Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).</span><span class="sxs-lookup"><span data-stu-id="18ba7-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="18ba7-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="18ba7-112">Properties</span></span>
| <span data-ttu-id="18ba7-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="18ba7-113">Property</span></span>     | <span data-ttu-id="18ba7-114">Typ</span><span class="sxs-lookup"><span data-stu-id="18ba7-114">Type</span></span>   |<span data-ttu-id="18ba7-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18ba7-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18ba7-116">id</span><span class="sxs-lookup"><span data-stu-id="18ba7-116">id</span></span>|<span data-ttu-id="18ba7-117">String</span><span class="sxs-lookup"><span data-stu-id="18ba7-117">String</span></span>| <span data-ttu-id="18ba7-p105">Eindeutiger Bezeichner, der dieser Entität zugewiesen ist. Lässt keine Nullwerte zu, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="18ba7-p105">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="18ba7-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="18ba7-120">isOptional</span></span>|<span data-ttu-id="18ba7-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="18ba7-121">Boolean</span></span>| <span data-ttu-id="18ba7-122">Wenn „false“, muss der SRV-Eintrag vom Kunden auf dem DNS-Host konfiguriert werden, damit Microsoft-Onlinedienste ordnungsgemäß mit der Domäne funktionieren.</span><span class="sxs-lookup"><span data-stu-id="18ba7-122">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="18ba7-123">label</span><span class="sxs-lookup"><span data-stu-id="18ba7-123">label</span></span>|<span data-ttu-id="18ba7-124">String</span><span class="sxs-lookup"><span data-stu-id="18ba7-124">String</span></span>| <span data-ttu-id="18ba7-125">Wert, der beim Konfigurieren der *name*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="18ba7-125">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="18ba7-126">nameTarget</span><span class="sxs-lookup"><span data-stu-id="18ba7-126">nameTarget</span></span>|<span data-ttu-id="18ba7-127">String</span><span class="sxs-lookup"><span data-stu-id="18ba7-127">String</span></span>| <span data-ttu-id="18ba7-128">Wert, der beim Konfigurieren der *target*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="18ba7-128">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="18ba7-129">port</span><span class="sxs-lookup"><span data-stu-id="18ba7-129">port</span></span>|<span data-ttu-id="18ba7-130">Int32</span><span class="sxs-lookup"><span data-stu-id="18ba7-130">Int32</span></span>| <span data-ttu-id="18ba7-131">Wert, der beim Konfigurieren der *port*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="18ba7-131">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="18ba7-132">priority</span><span class="sxs-lookup"><span data-stu-id="18ba7-132">priority</span></span>|<span data-ttu-id="18ba7-133">Int32</span><span class="sxs-lookup"><span data-stu-id="18ba7-133">Int32</span></span>| <span data-ttu-id="18ba7-134">Wert, der beim Konfigurieren der *priority*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="18ba7-134">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="18ba7-135">protocol</span><span class="sxs-lookup"><span data-stu-id="18ba7-135">protocol</span></span>|<span data-ttu-id="18ba7-136">String</span><span class="sxs-lookup"><span data-stu-id="18ba7-136">String</span></span>| <span data-ttu-id="18ba7-137">Wert, der beim Konfigurieren der *protocol*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="18ba7-137">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="18ba7-138">recordType</span><span class="sxs-lookup"><span data-stu-id="18ba7-138">recordType</span></span>|<span data-ttu-id="18ba7-139">String</span><span class="sxs-lookup"><span data-stu-id="18ba7-139">String</span></span>|  <span data-ttu-id="18ba7-p106">Typ des DNS-Eintrags. Der Wert ist immer *Srv*. Schlüssel</span><span class="sxs-lookup"><span data-stu-id="18ba7-p106">Type of DNS record. The value is always *Srv*. Key</span></span> |
|<span data-ttu-id="18ba7-143">service</span><span class="sxs-lookup"><span data-stu-id="18ba7-143">service</span></span>|<span data-ttu-id="18ba7-144">String</span><span class="sxs-lookup"><span data-stu-id="18ba7-144">String</span></span>| <span data-ttu-id="18ba7-145">Wert, der beim Konfigurieren der *service*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="18ba7-145">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="18ba7-146">supportedService</span><span class="sxs-lookup"><span data-stu-id="18ba7-146">supportedService</span></span>|<span data-ttu-id="18ba7-147">String</span><span class="sxs-lookup"><span data-stu-id="18ba7-147">String</span></span>| <span data-ttu-id="18ba7-148">Microsoft-Onlinedienst oder Feature mit Abhängigkeit von diesem SRV-Eintrag.</span><span class="sxs-lookup"><span data-stu-id="18ba7-148">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="18ba7-149">Kann einer der folgenden Werte sein: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="18ba7-149">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="18ba7-150">ttl</span><span class="sxs-lookup"><span data-stu-id="18ba7-150">ttl</span></span>|<span data-ttu-id="18ba7-151">Int32</span><span class="sxs-lookup"><span data-stu-id="18ba7-151">Int32</span></span>| <span data-ttu-id="18ba7-p107">Wert, der beim Konfigurieren der Eigenschaft für die Gültigkeitsdauer (*time-to-live (ttl)*) des SRV-Eintrags auf dem DNS-Host verwendet werden soll. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="18ba7-p107">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span> |
|<span data-ttu-id="18ba7-154">weight</span><span class="sxs-lookup"><span data-stu-id="18ba7-154">weight</span></span>|<span data-ttu-id="18ba7-155">Int32</span><span class="sxs-lookup"><span data-stu-id="18ba7-155">Int32</span></span>| <span data-ttu-id="18ba7-156">Wert, der beim Konfigurieren der *weight*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="18ba7-156">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="18ba7-157">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="18ba7-157">Relationships</span></span>
<span data-ttu-id="18ba7-158">Keine</span><span class="sxs-lookup"><span data-stu-id="18ba7-158">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="18ba7-159">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="18ba7-159">JSON representation</span></span>
<span data-ttu-id="18ba7-160">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="18ba7-160">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "nameTarget": "String",
  "port": 1024,
  "priority": 1024,
  "protocol": "String",
  "recordType": "String",
  "service": "String",
  "supportedService": "String",
  "ttl": 1024,
  "weight": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
