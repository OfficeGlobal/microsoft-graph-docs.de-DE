---
title: domainDnsMxRecord-Ressourcentyp
description: Stellt einen MX-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität DomainDnsRecord.
author: lleonard-msft
ms.openlocfilehash: e06b3c405f4ad5e2e561e57876ef010bddb1068d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345836"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="1dffe-104">domainDnsMxRecord-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1dffe-104">domainDnsMxRecord resource type</span></span>

<span data-ttu-id="1dffe-p102">Stellt einen MX-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="1dffe-p102">Represents a MX record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="1dffe-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="1dffe-107">Methods</span></span>
<span data-ttu-id="1dffe-p103">Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).</span><span class="sxs-lookup"><span data-stu-id="1dffe-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="1dffe-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1dffe-110">Properties</span></span>
| <span data-ttu-id="1dffe-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1dffe-111">Property</span></span>     | <span data-ttu-id="1dffe-112">Typ</span><span class="sxs-lookup"><span data-stu-id="1dffe-112">Type</span></span>   |<span data-ttu-id="1dffe-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1dffe-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1dffe-114">id</span><span class="sxs-lookup"><span data-stu-id="1dffe-114">id</span></span>|<span data-ttu-id="1dffe-115">String</span><span class="sxs-lookup"><span data-stu-id="1dffe-115">String</span></span>| <span data-ttu-id="1dffe-p104">Eindeutiger Bezeichner, der dieser Entität zugewiesen ist. Lässt keine Nullwerte zu, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1dffe-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="1dffe-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="1dffe-118">isOptional</span></span>|<span data-ttu-id="1dffe-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="1dffe-119">Boolean</span></span>| <span data-ttu-id="1dffe-120">Wenn „false“, muss der MX-Eintrag vom Kunden auf dem DNS-Host konfiguriert werden, damit Microsoft-Onlinedienste ordnungsgemäß mit der Domäne funktionieren.</span><span class="sxs-lookup"><span data-stu-id="1dffe-120">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="1dffe-121">label</span><span class="sxs-lookup"><span data-stu-id="1dffe-121">label</span></span>|<span data-ttu-id="1dffe-122">String</span><span class="sxs-lookup"><span data-stu-id="1dffe-122">String</span></span>| <span data-ttu-id="1dffe-123">Wert, der beim Konfigurieren der *alias/host/name*-Eigenschaft des MX-Eintrags auf dem DNS-Host verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="1dffe-123">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="1dffe-124">mailExchange</span><span class="sxs-lookup"><span data-stu-id="1dffe-124">mailExchange</span></span>|<span data-ttu-id="1dffe-125">String</span><span class="sxs-lookup"><span data-stu-id="1dffe-125">String</span></span>| <span data-ttu-id="1dffe-126">Wert, der beim Konfigurieren der *answer/destination/value*-Eigenschaft des MX-Eintrags auf dem DNS-Host verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="1dffe-126">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="1dffe-127">preference</span><span class="sxs-lookup"><span data-stu-id="1dffe-127">preference</span></span>|<span data-ttu-id="1dffe-128">Int32</span><span class="sxs-lookup"><span data-stu-id="1dffe-128">Int32</span></span>| <span data-ttu-id="1dffe-129">Wert, der beim Konfigurieren der *Preference/Priority*-Eigenschaft des MX-Eintrags auf dem DNS-Host verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="1dffe-129">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="1dffe-130">recordType</span><span class="sxs-lookup"><span data-stu-id="1dffe-130">recordType</span></span>|<span data-ttu-id="1dffe-131">String</span><span class="sxs-lookup"><span data-stu-id="1dffe-131">String</span></span>| <span data-ttu-id="1dffe-p105">Typ des DNS-Eintrags. Der Wert ist immer *MX*. Schlüssel</span><span class="sxs-lookup"><span data-stu-id="1dffe-p105">Type of DNS record. The value is always *Mx*. Key</span></span> |
|<span data-ttu-id="1dffe-135">supportedService</span><span class="sxs-lookup"><span data-stu-id="1dffe-135">supportedService</span></span>|<span data-ttu-id="1dffe-136">String</span><span class="sxs-lookup"><span data-stu-id="1dffe-136">String</span></span>| <span data-ttu-id="1dffe-137">Microsoft-Onlinedienst oder Feature mit Abhängigkeit von diesem MX-Eintrag.</span><span class="sxs-lookup"><span data-stu-id="1dffe-137">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="1dffe-138">Kann einer der folgenden Werte sein: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="1dffe-138">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="1dffe-139">ttl</span><span class="sxs-lookup"><span data-stu-id="1dffe-139">ttl</span></span>|<span data-ttu-id="1dffe-140">Int32</span><span class="sxs-lookup"><span data-stu-id="1dffe-140">Int32</span></span>| <span data-ttu-id="1dffe-p106">Wert, der beim Konfigurieren der Eigenschaft für die Gültigkeitsdauer (*time-to-live (ttl)*) des DNS-Eintrags auf dem DNS-Host verwendet werden soll. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="1dffe-p106">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="1dffe-143">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1dffe-143">Relationships</span></span>
<span data-ttu-id="1dffe-144">Keine</span><span class="sxs-lookup"><span data-stu-id="1dffe-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1dffe-145">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1dffe-145">JSON representation</span></span>
<span data-ttu-id="1dffe-146">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1dffe-146">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "mailExchange": "String",
  "preference": 1024,
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsMxRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->