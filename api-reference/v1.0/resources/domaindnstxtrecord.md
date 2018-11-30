---
title: domainDnsTxtRecord-Ressourcentyp
description: Stellt einen TXT-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität DomainDnsRecord.
ms.openlocfilehash: ed60c15463bd4182049fe3ae8fa32963f8574456
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016226"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="8910d-104">domainDnsTxtRecord-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8910d-104">domainDnsTxtRecord resource type</span></span>

<span data-ttu-id="8910d-p102">Stellt einen TXT-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="8910d-p102">Represents a TXT record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="8910d-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="8910d-107">Methods</span></span>
<span data-ttu-id="8910d-p103">Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).</span><span class="sxs-lookup"><span data-stu-id="8910d-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="8910d-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8910d-110">Properties</span></span>
| <span data-ttu-id="8910d-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8910d-111">Property</span></span>     | <span data-ttu-id="8910d-112">Typ</span><span class="sxs-lookup"><span data-stu-id="8910d-112">Type</span></span>   |<span data-ttu-id="8910d-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8910d-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8910d-114">id</span><span class="sxs-lookup"><span data-stu-id="8910d-114">id</span></span>|<span data-ttu-id="8910d-115">String</span><span class="sxs-lookup"><span data-stu-id="8910d-115">String</span></span>| <span data-ttu-id="8910d-p104">Eindeutiger Bezeichner, der dieser Entität zugewiesen ist. Lässt keine Nullwerte zu, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8910d-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span> |
|<span data-ttu-id="8910d-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="8910d-118">isOptional</span></span>|<span data-ttu-id="8910d-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="8910d-119">Boolean</span></span>| <span data-ttu-id="8910d-120">Wenn „false“, muss der TXT-Eintrag vom Kunden auf dem DNS-Host konfiguriert werden, damit Microsoft-Onlinedienste ordnungsgemäß mit der Domäne funktionieren.</span><span class="sxs-lookup"><span data-stu-id="8910d-120">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="8910d-121">label</span><span class="sxs-lookup"><span data-stu-id="8910d-121">label</span></span>|<span data-ttu-id="8910d-122">String</span><span class="sxs-lookup"><span data-stu-id="8910d-122">String</span></span>| <span data-ttu-id="8910d-123">Wert, der beim Konfigurieren der *name*-Eigenschaft des TXT-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="8910d-123">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="8910d-124">recordType</span><span class="sxs-lookup"><span data-stu-id="8910d-124">recordType</span></span>|<span data-ttu-id="8910d-125">String</span><span class="sxs-lookup"><span data-stu-id="8910d-125">String</span></span>| <span data-ttu-id="8910d-p105">Typ des DNS-Eintrags. Der Wert ist immer *Txt*. Schlüssel</span><span class="sxs-lookup"><span data-stu-id="8910d-p105">Type of DNS record. The value is always *Txt*. Key</span></span> |
|<span data-ttu-id="8910d-129">supportedService</span><span class="sxs-lookup"><span data-stu-id="8910d-129">supportedService</span></span>|<span data-ttu-id="8910d-130">String</span><span class="sxs-lookup"><span data-stu-id="8910d-130">String</span></span>| <span data-ttu-id="8910d-131">Microsoft-Onlinedienst oder Feature mit Abhängigkeit von diesem TXT-Eintrag.</span><span class="sxs-lookup"><span data-stu-id="8910d-131">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="8910d-132">Kann einer der folgenden Werte sein: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="8910d-132">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="8910d-133">text</span><span class="sxs-lookup"><span data-stu-id="8910d-133">text</span></span>|<span data-ttu-id="8910d-134">String</span><span class="sxs-lookup"><span data-stu-id="8910d-134">String</span></span>| <span data-ttu-id="8910d-135">Wert, der beim Konfigurieren der *text*-Eigenschaft auf dem DNS-Host verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="8910d-135">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="8910d-136">ttl</span><span class="sxs-lookup"><span data-stu-id="8910d-136">ttl</span></span>|<span data-ttu-id="8910d-137">Int32</span><span class="sxs-lookup"><span data-stu-id="8910d-137">Int32</span></span>| <span data-ttu-id="8910d-p106">Wert, der beim Konfigurieren der Eigenschaft für die Gültigkeitsdauer (*time-to-live (ttl)*) des DNS-Eintrags auf dem DNS-Host verwendet werden soll. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="8910d-p106">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="8910d-140">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8910d-140">Relationships</span></span>
<span data-ttu-id="8910d-141">Keine</span><span class="sxs-lookup"><span data-stu-id="8910d-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8910d-142">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8910d-142">JSON representation</span></span>
<span data-ttu-id="8910d-143">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8910d-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsTxtRecord"
}-->

```json
{
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
  "description": "domainDnsTxtRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->