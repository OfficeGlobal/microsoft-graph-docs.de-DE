---
title: domainDnsCnameRecord-Ressourcentyp
description: Stellt einen CNAME-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität DomainDnsRecord.
ms.openlocfilehash: 1c8df7148a4d843d5cd6278f5cbcc03358159424
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018503"
---
# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="3ac32-104">domainDnsCnameRecord-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3ac32-104">domainDnsCnameRecord resource type</span></span>

<span data-ttu-id="3ac32-p102">Stellt einen CNAME-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="3ac32-p102">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="3ac32-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="3ac32-107">Methods</span></span>
<span data-ttu-id="3ac32-p103">Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).</span><span class="sxs-lookup"><span data-stu-id="3ac32-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="3ac32-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3ac32-110">Properties</span></span>
| <span data-ttu-id="3ac32-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3ac32-111">Property</span></span>     | <span data-ttu-id="3ac32-112">Typ</span><span class="sxs-lookup"><span data-stu-id="3ac32-112">Type</span></span>   |<span data-ttu-id="3ac32-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ac32-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ac32-114">canonicalName</span><span class="sxs-lookup"><span data-stu-id="3ac32-114">canonicalName</span></span>|<span data-ttu-id="3ac32-115">String</span><span class="sxs-lookup"><span data-stu-id="3ac32-115">String</span></span>| <span data-ttu-id="3ac32-p104">Der kanonische Name des CNAME-Eintrags. Wird verwendet, um den CNAME-Eintrag auf dem DNS-Host zu konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="3ac32-p104">The canonical name of the CNAME record. Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="3ac32-118">id</span><span class="sxs-lookup"><span data-stu-id="3ac32-118">id</span></span>|<span data-ttu-id="3ac32-119">String</span><span class="sxs-lookup"><span data-stu-id="3ac32-119">String</span></span>| <span data-ttu-id="3ac32-p105">Eindeutiger Bezeichner, der dieser Entität zugewiesen ist. Lässt keine Nullwerte zu, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3ac32-p105">Unique identifier assigned to this entity. Not nullable, Read-only</span></span>|
|<span data-ttu-id="3ac32-122">isOptional</span><span class="sxs-lookup"><span data-stu-id="3ac32-122">isOptional</span></span>|<span data-ttu-id="3ac32-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="3ac32-123">Boolean</span></span>| <span data-ttu-id="3ac32-p106">Wenn „false“, muss der CNAME-Eintrag vom Kunden auf dem DNS-Host konfiguriert werden, damit Microsoft-Onlinedienste ordnungsgemäß mit der Domäne funktionieren. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="3ac32-p106">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain. Not nullable</span></span> |
|<span data-ttu-id="3ac32-126">label</span><span class="sxs-lookup"><span data-stu-id="3ac32-126">label</span></span>|<span data-ttu-id="3ac32-127">String</span><span class="sxs-lookup"><span data-stu-id="3ac32-127">String</span></span>| <span data-ttu-id="3ac32-128">Wert, der beim Konfigurieren der *alias/host/name*-Eigenschaft des CNAME-Eintrags auf dem DNS-Host verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="3ac32-128">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="3ac32-129">recordType</span><span class="sxs-lookup"><span data-stu-id="3ac32-129">recordType</span></span>|<span data-ttu-id="3ac32-130">String</span><span class="sxs-lookup"><span data-stu-id="3ac32-130">String</span></span>| <span data-ttu-id="3ac32-p107">Typ des DNS-Eintrags. Der Wert ist immer *CName*. Schlüssel</span><span class="sxs-lookup"><span data-stu-id="3ac32-p107">Type of DNS record. The value is always *CName*. Key</span></span>|
|<span data-ttu-id="3ac32-134">supportedService</span><span class="sxs-lookup"><span data-stu-id="3ac32-134">supportedService</span></span>|<span data-ttu-id="3ac32-135">String</span><span class="sxs-lookup"><span data-stu-id="3ac32-135">String</span></span>| <span data-ttu-id="3ac32-136">Microsoft-Onlinedienst oder Feature mit Abhängigkeit von diesem CNAME-Eintrag.</span><span class="sxs-lookup"><span data-stu-id="3ac32-136">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="3ac32-137">Kann einer der folgenden Werte sein: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="3ac32-137">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="3ac32-138">ttl</span><span class="sxs-lookup"><span data-stu-id="3ac32-138">ttl</span></span>|<span data-ttu-id="3ac32-139">Int32</span><span class="sxs-lookup"><span data-stu-id="3ac32-139">Int32</span></span>| <span data-ttu-id="3ac32-p108">Wert, der beim Konfigurieren der Eigenschaft für die Gültigkeitsdauer (time-to-live (ttl) des CNAME-Eintrags auf dem DNS-Host verwendet werden soll. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="3ac32-p108">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="3ac32-142">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3ac32-142">Relationships</span></span>
<span data-ttu-id="3ac32-143">Keine</span><span class="sxs-lookup"><span data-stu-id="3ac32-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3ac32-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3ac32-144">JSON representation</span></span>
<span data-ttu-id="3ac32-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3ac32-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsCnameRecord"
}-->

```json
{
  "canonicalName": "String",
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
  "description": "domainDnsCnameRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->