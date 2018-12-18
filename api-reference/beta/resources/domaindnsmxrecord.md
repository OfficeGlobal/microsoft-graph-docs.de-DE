---
title: domainDnsMxRecord-Ressourcentyp
description: Stellt einen MX-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität DomainDnsRecord.
author: lleonard-msft
ms.openlocfilehash: 562afbd6998ad1678f4f055dacf89af9b1ed4446
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320650"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="32372-104">domainDnsMxRecord-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="32372-104">domainDnsMxRecord resource type</span></span>

> <span data-ttu-id="32372-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="32372-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32372-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="32372-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="32372-p103">Stellt einen MX-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="32372-p103">Represents a MX record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="32372-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="32372-109">Methods</span></span>
<span data-ttu-id="32372-p104">Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).</span><span class="sxs-lookup"><span data-stu-id="32372-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="32372-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="32372-112">Properties</span></span>
| <span data-ttu-id="32372-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="32372-113">Property</span></span>     | <span data-ttu-id="32372-114">Typ</span><span class="sxs-lookup"><span data-stu-id="32372-114">Type</span></span>   |<span data-ttu-id="32372-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="32372-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32372-116">id</span><span class="sxs-lookup"><span data-stu-id="32372-116">id</span></span>|<span data-ttu-id="32372-117">String</span><span class="sxs-lookup"><span data-stu-id="32372-117">String</span></span>| <span data-ttu-id="32372-p105">Eindeutiger Bezeichner, der dieser Entität zugewiesen ist. Lässt keine Nullwerte zu, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="32372-p105">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="32372-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="32372-120">isOptional</span></span>|<span data-ttu-id="32372-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="32372-121">Boolean</span></span>| <span data-ttu-id="32372-122">Wenn „false“, muss der MX-Eintrag vom Kunden auf dem DNS-Host konfiguriert werden, damit Microsoft-Onlinedienste ordnungsgemäß mit der Domäne funktionieren.</span><span class="sxs-lookup"><span data-stu-id="32372-122">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="32372-123">label</span><span class="sxs-lookup"><span data-stu-id="32372-123">label</span></span>|<span data-ttu-id="32372-124">String</span><span class="sxs-lookup"><span data-stu-id="32372-124">String</span></span>| <span data-ttu-id="32372-125">Wert, der beim Konfigurieren der *alias/host/name*-Eigenschaft des MX-Eintrags auf dem DNS-Host verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="32372-125">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="32372-126">mailExchange</span><span class="sxs-lookup"><span data-stu-id="32372-126">mailExchange</span></span>|<span data-ttu-id="32372-127">String</span><span class="sxs-lookup"><span data-stu-id="32372-127">String</span></span>| <span data-ttu-id="32372-128">Wert, der beim Konfigurieren der *answer/destination/value*-Eigenschaft des MX-Eintrags auf dem DNS-Host verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="32372-128">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="32372-129">preference</span><span class="sxs-lookup"><span data-stu-id="32372-129">preference</span></span>|<span data-ttu-id="32372-130">Int32</span><span class="sxs-lookup"><span data-stu-id="32372-130">Int32</span></span>| <span data-ttu-id="32372-131">Wert, der beim Konfigurieren der *Preference/Priority*-Eigenschaft des MX-Eintrags auf dem DNS-Host verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="32372-131">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="32372-132">recordType</span><span class="sxs-lookup"><span data-stu-id="32372-132">recordType</span></span>|<span data-ttu-id="32372-133">String</span><span class="sxs-lookup"><span data-stu-id="32372-133">String</span></span>| <span data-ttu-id="32372-p106">Typ des DNS-Eintrags. Der Wert ist immer *MX*. Schlüssel</span><span class="sxs-lookup"><span data-stu-id="32372-p106">Type of DNS record. The value is always *Mx*. Key</span></span> |
|<span data-ttu-id="32372-137">supportedService</span><span class="sxs-lookup"><span data-stu-id="32372-137">supportedService</span></span>|<span data-ttu-id="32372-138">String</span><span class="sxs-lookup"><span data-stu-id="32372-138">String</span></span>| <span data-ttu-id="32372-139">Microsoft-Onlinedienst oder Feature mit Abhängigkeit von diesem MX-Eintrag.</span><span class="sxs-lookup"><span data-stu-id="32372-139">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="32372-140">Kann einer der folgenden Werte sein: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="32372-140">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="32372-141">ttl</span><span class="sxs-lookup"><span data-stu-id="32372-141">ttl</span></span>|<span data-ttu-id="32372-142">Int32</span><span class="sxs-lookup"><span data-stu-id="32372-142">Int32</span></span>| <span data-ttu-id="32372-p107">Wert, der beim Konfigurieren der Eigenschaft für die Gültigkeitsdauer (*time-to-live (ttl)*) des DNS-Eintrags auf dem DNS-Host verwendet werden soll. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="32372-p107">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="32372-145">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="32372-145">Relationships</span></span>
<span data-ttu-id="32372-146">Keine</span><span class="sxs-lookup"><span data-stu-id="32372-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32372-147">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="32372-147">JSON representation</span></span>
<span data-ttu-id="32372-148">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="32372-148">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
  "canonicalName": "String",
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