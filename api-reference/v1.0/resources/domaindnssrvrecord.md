---
title: domainDnsSrvRecord-Ressourcentyp
description: Stellt einen SRV-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität DomainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 655dc6fcbccdcb6e1794c94d97dd8e7fc4837f04
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835791"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="5753f-104">domainDnsSrvRecord-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5753f-104">domainDnsSrvRecord resource type</span></span>

<span data-ttu-id="5753f-p102">Stellt einen SRV-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="5753f-p102">Represents a SRV record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="5753f-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="5753f-107">Methods</span></span>
<span data-ttu-id="5753f-p103">Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).</span><span class="sxs-lookup"><span data-stu-id="5753f-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="5753f-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5753f-110">Properties</span></span>
| <span data-ttu-id="5753f-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5753f-111">Property</span></span>     | <span data-ttu-id="5753f-112">Typ</span><span class="sxs-lookup"><span data-stu-id="5753f-112">Type</span></span>   |<span data-ttu-id="5753f-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5753f-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5753f-114">id</span><span class="sxs-lookup"><span data-stu-id="5753f-114">id</span></span>|<span data-ttu-id="5753f-115">String</span><span class="sxs-lookup"><span data-stu-id="5753f-115">String</span></span>| <span data-ttu-id="5753f-p104">Eindeutiger Bezeichner, der dieser Entität zugewiesen ist. Lässt keine Nullwerte zu, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5753f-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="5753f-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="5753f-118">isOptional</span></span>|<span data-ttu-id="5753f-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="5753f-119">Boolean</span></span>| <span data-ttu-id="5753f-120">Wenn „false“, muss der SRV-Eintrag vom Kunden auf dem DNS-Host konfiguriert werden, damit Microsoft-Onlinedienste ordnungsgemäß mit der Domäne funktionieren.</span><span class="sxs-lookup"><span data-stu-id="5753f-120">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="5753f-121">label</span><span class="sxs-lookup"><span data-stu-id="5753f-121">label</span></span>|<span data-ttu-id="5753f-122">String</span><span class="sxs-lookup"><span data-stu-id="5753f-122">String</span></span>| <span data-ttu-id="5753f-123">Wert, der beim Konfigurieren der *name*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="5753f-123">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="5753f-124">nameTarget</span><span class="sxs-lookup"><span data-stu-id="5753f-124">nameTarget</span></span>|<span data-ttu-id="5753f-125">String</span><span class="sxs-lookup"><span data-stu-id="5753f-125">String</span></span>| <span data-ttu-id="5753f-126">Wert, der beim Konfigurieren der *target*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="5753f-126">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="5753f-127">port</span><span class="sxs-lookup"><span data-stu-id="5753f-127">port</span></span>|<span data-ttu-id="5753f-128">Int32</span><span class="sxs-lookup"><span data-stu-id="5753f-128">Int32</span></span>| <span data-ttu-id="5753f-129">Wert, der beim Konfigurieren der *port*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="5753f-129">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="5753f-130">priority</span><span class="sxs-lookup"><span data-stu-id="5753f-130">priority</span></span>|<span data-ttu-id="5753f-131">Int32</span><span class="sxs-lookup"><span data-stu-id="5753f-131">Int32</span></span>| <span data-ttu-id="5753f-132">Wert, der beim Konfigurieren der *priority*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="5753f-132">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="5753f-133">protocol</span><span class="sxs-lookup"><span data-stu-id="5753f-133">protocol</span></span>|<span data-ttu-id="5753f-134">String</span><span class="sxs-lookup"><span data-stu-id="5753f-134">String</span></span>| <span data-ttu-id="5753f-135">Wert, der beim Konfigurieren der *protocol*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="5753f-135">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="5753f-136">recordType</span><span class="sxs-lookup"><span data-stu-id="5753f-136">recordType</span></span>|<span data-ttu-id="5753f-137">String</span><span class="sxs-lookup"><span data-stu-id="5753f-137">String</span></span>|  <span data-ttu-id="5753f-p105">Typ des DNS-Eintrags. Der Wert ist immer *Srv*. Schlüssel</span><span class="sxs-lookup"><span data-stu-id="5753f-p105">Type of DNS record. The value is always *Srv*. Key</span></span> |
|<span data-ttu-id="5753f-141">service</span><span class="sxs-lookup"><span data-stu-id="5753f-141">service</span></span>|<span data-ttu-id="5753f-142">String</span><span class="sxs-lookup"><span data-stu-id="5753f-142">String</span></span>| <span data-ttu-id="5753f-143">Wert, der beim Konfigurieren der *service*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="5753f-143">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="5753f-144">supportedService</span><span class="sxs-lookup"><span data-stu-id="5753f-144">supportedService</span></span>|<span data-ttu-id="5753f-145">String</span><span class="sxs-lookup"><span data-stu-id="5753f-145">String</span></span>| <span data-ttu-id="5753f-146">Microsoft-Onlinedienst oder Feature mit Abhängigkeit von diesem SRV-Eintrag.</span><span class="sxs-lookup"><span data-stu-id="5753f-146">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="5753f-147">Kann einer der folgenden Werte sein: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="5753f-147">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="5753f-148">ttl</span><span class="sxs-lookup"><span data-stu-id="5753f-148">ttl</span></span>|<span data-ttu-id="5753f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="5753f-149">Int32</span></span>| <span data-ttu-id="5753f-p106">Wert, der beim Konfigurieren der Eigenschaft für die Gültigkeitsdauer (*time-to-live (ttl)*) des SRV-Eintrags auf dem DNS-Host verwendet werden soll. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="5753f-p106">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span> |
|<span data-ttu-id="5753f-152">weight</span><span class="sxs-lookup"><span data-stu-id="5753f-152">weight</span></span>|<span data-ttu-id="5753f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="5753f-153">Int32</span></span>| <span data-ttu-id="5753f-154">Wert, der beim Konfigurieren der *weight*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="5753f-154">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5753f-155">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5753f-155">Relationships</span></span>
<span data-ttu-id="5753f-156">Keine</span><span class="sxs-lookup"><span data-stu-id="5753f-156">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5753f-157">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5753f-157">JSON representation</span></span>
<span data-ttu-id="5753f-158">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5753f-158">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
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
