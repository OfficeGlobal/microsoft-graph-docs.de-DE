---
title: domainDnsSrvRecord-Ressourcentyp
description: Stellt einen SRV-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität DomainDnsRecord.
ms.openlocfilehash: 1fd1123866d1674aec167de8bec8ef9a45be8d99
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017826"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="b57bc-104">domainDnsSrvRecord-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b57bc-104">domainDnsSrvRecord resource type</span></span>

<span data-ttu-id="b57bc-p102">Stellt einen SRV-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="b57bc-p102">Represents a SRV record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="b57bc-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="b57bc-107">Methods</span></span>
<span data-ttu-id="b57bc-p103">Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).</span><span class="sxs-lookup"><span data-stu-id="b57bc-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="b57bc-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b57bc-110">Properties</span></span>
| <span data-ttu-id="b57bc-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b57bc-111">Property</span></span>     | <span data-ttu-id="b57bc-112">Typ</span><span class="sxs-lookup"><span data-stu-id="b57bc-112">Type</span></span>   |<span data-ttu-id="b57bc-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b57bc-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b57bc-114">id</span><span class="sxs-lookup"><span data-stu-id="b57bc-114">id</span></span>|<span data-ttu-id="b57bc-115">String</span><span class="sxs-lookup"><span data-stu-id="b57bc-115">String</span></span>| <span data-ttu-id="b57bc-p104">Eindeutiger Bezeichner, der dieser Entität zugewiesen ist. Lässt keine Nullwerte zu, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="b57bc-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="b57bc-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="b57bc-118">isOptional</span></span>|<span data-ttu-id="b57bc-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="b57bc-119">Boolean</span></span>| <span data-ttu-id="b57bc-120">Wenn „false“, muss der SRV-Eintrag vom Kunden auf dem DNS-Host konfiguriert werden, damit Microsoft-Onlinedienste ordnungsgemäß mit der Domäne funktionieren.</span><span class="sxs-lookup"><span data-stu-id="b57bc-120">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="b57bc-121">label</span><span class="sxs-lookup"><span data-stu-id="b57bc-121">label</span></span>|<span data-ttu-id="b57bc-122">String</span><span class="sxs-lookup"><span data-stu-id="b57bc-122">String</span></span>| <span data-ttu-id="b57bc-123">Wert, der beim Konfigurieren der *name*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="b57bc-123">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="b57bc-124">nameTarget</span><span class="sxs-lookup"><span data-stu-id="b57bc-124">nameTarget</span></span>|<span data-ttu-id="b57bc-125">String</span><span class="sxs-lookup"><span data-stu-id="b57bc-125">String</span></span>| <span data-ttu-id="b57bc-126">Wert, der beim Konfigurieren der *target*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="b57bc-126">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="b57bc-127">port</span><span class="sxs-lookup"><span data-stu-id="b57bc-127">port</span></span>|<span data-ttu-id="b57bc-128">Int32</span><span class="sxs-lookup"><span data-stu-id="b57bc-128">Int32</span></span>| <span data-ttu-id="b57bc-129">Wert, der beim Konfigurieren der *port*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="b57bc-129">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="b57bc-130">priority</span><span class="sxs-lookup"><span data-stu-id="b57bc-130">priority</span></span>|<span data-ttu-id="b57bc-131">Int32</span><span class="sxs-lookup"><span data-stu-id="b57bc-131">Int32</span></span>| <span data-ttu-id="b57bc-132">Wert, der beim Konfigurieren der *priority*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="b57bc-132">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="b57bc-133">protocol</span><span class="sxs-lookup"><span data-stu-id="b57bc-133">protocol</span></span>|<span data-ttu-id="b57bc-134">String</span><span class="sxs-lookup"><span data-stu-id="b57bc-134">String</span></span>| <span data-ttu-id="b57bc-135">Wert, der beim Konfigurieren der *protocol*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="b57bc-135">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="b57bc-136">recordType</span><span class="sxs-lookup"><span data-stu-id="b57bc-136">recordType</span></span>|<span data-ttu-id="b57bc-137">String</span><span class="sxs-lookup"><span data-stu-id="b57bc-137">String</span></span>|  <span data-ttu-id="b57bc-p105">Typ des DNS-Eintrags. Der Wert ist immer *Srv*. Schlüssel</span><span class="sxs-lookup"><span data-stu-id="b57bc-p105">Type of DNS record. The value is always *Srv*. Key</span></span> |
|<span data-ttu-id="b57bc-141">service</span><span class="sxs-lookup"><span data-stu-id="b57bc-141">service</span></span>|<span data-ttu-id="b57bc-142">String</span><span class="sxs-lookup"><span data-stu-id="b57bc-142">String</span></span>| <span data-ttu-id="b57bc-143">Wert, der beim Konfigurieren der *service*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="b57bc-143">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="b57bc-144">supportedService</span><span class="sxs-lookup"><span data-stu-id="b57bc-144">supportedService</span></span>|<span data-ttu-id="b57bc-145">String</span><span class="sxs-lookup"><span data-stu-id="b57bc-145">String</span></span>| <span data-ttu-id="b57bc-146">Microsoft-Onlinedienst oder Feature mit Abhängigkeit von diesem SRV-Eintrag.</span><span class="sxs-lookup"><span data-stu-id="b57bc-146">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="b57bc-147">Kann einer der folgenden Werte sein: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="b57bc-147">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="b57bc-148">ttl</span><span class="sxs-lookup"><span data-stu-id="b57bc-148">ttl</span></span>|<span data-ttu-id="b57bc-149">Int32</span><span class="sxs-lookup"><span data-stu-id="b57bc-149">Int32</span></span>| <span data-ttu-id="b57bc-p106">Wert, der beim Konfigurieren der Eigenschaft für die Gültigkeitsdauer (*time-to-live (ttl)*) des SRV-Eintrags auf dem DNS-Host verwendet werden soll. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="b57bc-p106">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span> |
|<span data-ttu-id="b57bc-152">weight</span><span class="sxs-lookup"><span data-stu-id="b57bc-152">weight</span></span>|<span data-ttu-id="b57bc-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b57bc-153">Int32</span></span>| <span data-ttu-id="b57bc-154">Wert, der beim Konfigurieren der *weight*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="b57bc-154">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b57bc-155">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b57bc-155">Relationships</span></span>
<span data-ttu-id="b57bc-156">Keine</span><span class="sxs-lookup"><span data-stu-id="b57bc-156">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b57bc-157">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b57bc-157">JSON representation</span></span>
<span data-ttu-id="b57bc-158">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b57bc-158">Here is a JSON representation of the resource.</span></span>

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