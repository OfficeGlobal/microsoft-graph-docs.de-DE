---
title: domainDnsTxtRecord-Ressourcentyp
description: Stellt einen TXT-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität DomainDnsRecord.
ms.openlocfilehash: 2c49f42c2044d58855d293d39c0e5110091e4495
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065170"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="8927a-104">domainDnsTxtRecord-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8927a-104">domainDnsTxtRecord resource type</span></span>

> <span data-ttu-id="8927a-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8927a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8927a-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8927a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8927a-p103">Stellt einen TXT-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="8927a-p103">Represents a TXT record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="8927a-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="8927a-109">Methods</span></span>
<span data-ttu-id="8927a-p104">Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).</span><span class="sxs-lookup"><span data-stu-id="8927a-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="8927a-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8927a-112">Properties</span></span>
| <span data-ttu-id="8927a-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8927a-113">Property</span></span>     | <span data-ttu-id="8927a-114">Typ</span><span class="sxs-lookup"><span data-stu-id="8927a-114">Type</span></span>   |<span data-ttu-id="8927a-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8927a-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8927a-116">id</span><span class="sxs-lookup"><span data-stu-id="8927a-116">id</span></span>|<span data-ttu-id="8927a-117">String</span><span class="sxs-lookup"><span data-stu-id="8927a-117">String</span></span>| <span data-ttu-id="8927a-p105">Eindeutiger Bezeichner, der dieser Entität zugewiesen ist. Lässt keine Nullwerte zu, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8927a-p105">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span> |
|<span data-ttu-id="8927a-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="8927a-120">isOptional</span></span>|<span data-ttu-id="8927a-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="8927a-121">Boolean</span></span>| <span data-ttu-id="8927a-122">Wenn „false“, muss der TXT-Eintrag vom Kunden auf dem DNS-Host konfiguriert werden, damit Microsoft-Onlinedienste ordnungsgemäß mit der Domäne funktionieren.</span><span class="sxs-lookup"><span data-stu-id="8927a-122">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="8927a-123">label</span><span class="sxs-lookup"><span data-stu-id="8927a-123">label</span></span>|<span data-ttu-id="8927a-124">String</span><span class="sxs-lookup"><span data-stu-id="8927a-124">String</span></span>| <span data-ttu-id="8927a-125">Wert, der beim Konfigurieren der *name*-Eigenschaft des TXT-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="8927a-125">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="8927a-126">recordType</span><span class="sxs-lookup"><span data-stu-id="8927a-126">recordType</span></span>|<span data-ttu-id="8927a-127">String</span><span class="sxs-lookup"><span data-stu-id="8927a-127">String</span></span>| <span data-ttu-id="8927a-p106">Typ des DNS-Eintrags. Der Wert ist immer *Txt*. Schlüssel</span><span class="sxs-lookup"><span data-stu-id="8927a-p106">Type of DNS record. The value is always *Txt*. Key</span></span> |
|<span data-ttu-id="8927a-131">supportedService</span><span class="sxs-lookup"><span data-stu-id="8927a-131">supportedService</span></span>|<span data-ttu-id="8927a-132">String</span><span class="sxs-lookup"><span data-stu-id="8927a-132">String</span></span>| <span data-ttu-id="8927a-133">Microsoft-Onlinedienst oder Feature mit Abhängigkeit von diesem TXT-Eintrag.</span><span class="sxs-lookup"><span data-stu-id="8927a-133">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="8927a-134">Kann einer der folgenden Werte sein: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="8927a-134">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="8927a-135">text</span><span class="sxs-lookup"><span data-stu-id="8927a-135">text</span></span>|<span data-ttu-id="8927a-136">String</span><span class="sxs-lookup"><span data-stu-id="8927a-136">String</span></span>| <span data-ttu-id="8927a-137">Wert, der beim Konfigurieren der *text*-Eigenschaft auf dem DNS-Host verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="8927a-137">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="8927a-138">ttl</span><span class="sxs-lookup"><span data-stu-id="8927a-138">ttl</span></span>|<span data-ttu-id="8927a-139">Int32</span><span class="sxs-lookup"><span data-stu-id="8927a-139">Int32</span></span>| <span data-ttu-id="8927a-p107">Wert, der beim Konfigurieren der Eigenschaft für die Gültigkeitsdauer (*time-to-live (ttl)*) des DNS-Eintrags auf dem DNS-Host verwendet werden soll. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="8927a-p107">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="8927a-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8927a-142">Relationships</span></span>
<span data-ttu-id="8927a-143">Keine</span><span class="sxs-lookup"><span data-stu-id="8927a-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8927a-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8927a-144">JSON representation</span></span>
<span data-ttu-id="8927a-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8927a-145">Here is a JSON representation of the resource.</span></span>

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