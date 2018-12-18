---
title: domainDnsTxtRecord-Ressourcentyp
description: Stellt einen TXT-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität DomainDnsRecord.
author: lleonard-msft
ms.openlocfilehash: caefb97b39219c282c45949b504c3d0b91cdada9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349014"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="656e6-104">domainDnsTxtRecord-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="656e6-104">domainDnsTxtRecord resource type</span></span>

> <span data-ttu-id="656e6-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="656e6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="656e6-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="656e6-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="656e6-p103">Stellt einen TXT-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="656e6-p103">Represents a TXT record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="656e6-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="656e6-109">Methods</span></span>
<span data-ttu-id="656e6-p104">Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).</span><span class="sxs-lookup"><span data-stu-id="656e6-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="656e6-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="656e6-112">Properties</span></span>
| <span data-ttu-id="656e6-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="656e6-113">Property</span></span>     | <span data-ttu-id="656e6-114">Typ</span><span class="sxs-lookup"><span data-stu-id="656e6-114">Type</span></span>   |<span data-ttu-id="656e6-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="656e6-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="656e6-116">id</span><span class="sxs-lookup"><span data-stu-id="656e6-116">id</span></span>|<span data-ttu-id="656e6-117">String</span><span class="sxs-lookup"><span data-stu-id="656e6-117">String</span></span>| <span data-ttu-id="656e6-p105">Eindeutiger Bezeichner, der dieser Entität zugewiesen ist. Lässt keine Nullwerte zu, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="656e6-p105">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span> |
|<span data-ttu-id="656e6-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="656e6-120">isOptional</span></span>|<span data-ttu-id="656e6-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="656e6-121">Boolean</span></span>| <span data-ttu-id="656e6-122">Wenn „false“, muss der TXT-Eintrag vom Kunden auf dem DNS-Host konfiguriert werden, damit Microsoft-Onlinedienste ordnungsgemäß mit der Domäne funktionieren.</span><span class="sxs-lookup"><span data-stu-id="656e6-122">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="656e6-123">label</span><span class="sxs-lookup"><span data-stu-id="656e6-123">label</span></span>|<span data-ttu-id="656e6-124">String</span><span class="sxs-lookup"><span data-stu-id="656e6-124">String</span></span>| <span data-ttu-id="656e6-125">Wert, der beim Konfigurieren der *name*-Eigenschaft des TXT-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="656e6-125">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="656e6-126">recordType</span><span class="sxs-lookup"><span data-stu-id="656e6-126">recordType</span></span>|<span data-ttu-id="656e6-127">String</span><span class="sxs-lookup"><span data-stu-id="656e6-127">String</span></span>| <span data-ttu-id="656e6-p106">Typ des DNS-Eintrags. Der Wert ist immer *Txt*. Schlüssel</span><span class="sxs-lookup"><span data-stu-id="656e6-p106">Type of DNS record. The value is always *Txt*. Key</span></span> |
|<span data-ttu-id="656e6-131">supportedService</span><span class="sxs-lookup"><span data-stu-id="656e6-131">supportedService</span></span>|<span data-ttu-id="656e6-132">String</span><span class="sxs-lookup"><span data-stu-id="656e6-132">String</span></span>| <span data-ttu-id="656e6-133">Microsoft-Onlinedienst oder Feature mit Abhängigkeit von diesem TXT-Eintrag.</span><span class="sxs-lookup"><span data-stu-id="656e6-133">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="656e6-134">Kann einer der folgenden Werte sein: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="656e6-134">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="656e6-135">text</span><span class="sxs-lookup"><span data-stu-id="656e6-135">text</span></span>|<span data-ttu-id="656e6-136">String</span><span class="sxs-lookup"><span data-stu-id="656e6-136">String</span></span>| <span data-ttu-id="656e6-137">Wert, der beim Konfigurieren der *text*-Eigenschaft auf dem DNS-Host verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="656e6-137">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="656e6-138">ttl</span><span class="sxs-lookup"><span data-stu-id="656e6-138">ttl</span></span>|<span data-ttu-id="656e6-139">Int32</span><span class="sxs-lookup"><span data-stu-id="656e6-139">Int32</span></span>| <span data-ttu-id="656e6-p107">Wert, der beim Konfigurieren der Eigenschaft für die Gültigkeitsdauer (*time-to-live (ttl)*) des DNS-Eintrags auf dem DNS-Host verwendet werden soll. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="656e6-p107">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="656e6-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="656e6-142">Relationships</span></span>
<span data-ttu-id="656e6-143">Keine</span><span class="sxs-lookup"><span data-stu-id="656e6-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="656e6-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="656e6-144">JSON representation</span></span>
<span data-ttu-id="656e6-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="656e6-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsTxtRecord"
}-->

```json
{
  "canonicalName": "String",
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