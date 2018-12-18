---
title: domainDnsCnameRecord-Ressourcentyp
description: Stellt einen CNAME-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität DomainDnsRecord.
author: lleonard-msft
ms.openlocfilehash: 0ce5a748d9a1b558b4ac49e104eb9498efe674aa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315841"
---
# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="f6f99-104">domainDnsCnameRecord-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f6f99-104">domainDnsCnameRecord resource type</span></span>

> <span data-ttu-id="f6f99-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f6f99-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f6f99-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f6f99-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f6f99-p103">Stellt einen CNAME-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="f6f99-p103">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="f6f99-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="f6f99-109">Methods</span></span>
<span data-ttu-id="f6f99-p104">Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).</span><span class="sxs-lookup"><span data-stu-id="f6f99-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="f6f99-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f6f99-112">Properties</span></span>
| <span data-ttu-id="f6f99-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f6f99-113">Property</span></span>     | <span data-ttu-id="f6f99-114">Typ</span><span class="sxs-lookup"><span data-stu-id="f6f99-114">Type</span></span>   |<span data-ttu-id="f6f99-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6f99-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6f99-116">canonicalName</span><span class="sxs-lookup"><span data-stu-id="f6f99-116">canonicalName</span></span>|<span data-ttu-id="f6f99-117">String</span><span class="sxs-lookup"><span data-stu-id="f6f99-117">String</span></span>| <span data-ttu-id="f6f99-p105">Der kanonische Name des CNAME-Eintrags. Wird verwendet, um den CNAME-Eintrag auf dem DNS-Host zu konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="f6f99-p105">The canonical name of the CNAME record. Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="f6f99-120">id</span><span class="sxs-lookup"><span data-stu-id="f6f99-120">id</span></span>|<span data-ttu-id="f6f99-121">String</span><span class="sxs-lookup"><span data-stu-id="f6f99-121">String</span></span>| <span data-ttu-id="f6f99-p106">Eindeutiger Bezeichner, der dieser Entität zugewiesen ist. Lässt keine Nullwerte zu, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f6f99-p106">Unique identifier assigned to this entity. Not nullable, Read-only</span></span>|
|<span data-ttu-id="f6f99-124">isOptional</span><span class="sxs-lookup"><span data-stu-id="f6f99-124">isOptional</span></span>|<span data-ttu-id="f6f99-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6f99-125">Boolean</span></span>| <span data-ttu-id="f6f99-p107">Wenn „false“, muss der CNAME-Eintrag vom Kunden auf dem DNS-Host konfiguriert werden, damit Microsoft-Onlinedienste ordnungsgemäß mit der Domäne funktionieren. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="f6f99-p107">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain. Not nullable</span></span> |
|<span data-ttu-id="f6f99-128">label</span><span class="sxs-lookup"><span data-stu-id="f6f99-128">label</span></span>|<span data-ttu-id="f6f99-129">String</span><span class="sxs-lookup"><span data-stu-id="f6f99-129">String</span></span>| <span data-ttu-id="f6f99-130">Wert, der beim Konfigurieren der *alias/host/name*-Eigenschaft des CNAME-Eintrags auf dem DNS-Host verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="f6f99-130">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="f6f99-131">recordType</span><span class="sxs-lookup"><span data-stu-id="f6f99-131">recordType</span></span>|<span data-ttu-id="f6f99-132">String</span><span class="sxs-lookup"><span data-stu-id="f6f99-132">String</span></span>| <span data-ttu-id="f6f99-p108">Typ des DNS-Eintrags. Der Wert ist immer *CName*. Schlüssel</span><span class="sxs-lookup"><span data-stu-id="f6f99-p108">Type of DNS record. The value is always *CName*. Key</span></span>|
|<span data-ttu-id="f6f99-136">supportedService</span><span class="sxs-lookup"><span data-stu-id="f6f99-136">supportedService</span></span>|<span data-ttu-id="f6f99-137">String</span><span class="sxs-lookup"><span data-stu-id="f6f99-137">String</span></span>| <span data-ttu-id="f6f99-138">Microsoft-Onlinedienst oder Feature mit Abhängigkeit von diesem CNAME-Eintrag.</span><span class="sxs-lookup"><span data-stu-id="f6f99-138">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="f6f99-139">Kann einer der folgenden Werte sein: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="f6f99-139">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="f6f99-140">ttl</span><span class="sxs-lookup"><span data-stu-id="f6f99-140">ttl</span></span>|<span data-ttu-id="f6f99-141">Int32</span><span class="sxs-lookup"><span data-stu-id="f6f99-141">Int32</span></span>| <span data-ttu-id="f6f99-p109">Wert, der beim Konfigurieren der Eigenschaft für die Gültigkeitsdauer (time-to-live (ttl) des CNAME-Eintrags auf dem DNS-Host verwendet werden soll. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="f6f99-p109">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="f6f99-144">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f6f99-144">Relationships</span></span>
<span data-ttu-id="f6f99-145">Keine</span><span class="sxs-lookup"><span data-stu-id="f6f99-145">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f6f99-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f6f99-146">JSON representation</span></span>
<span data-ttu-id="f6f99-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f6f99-147">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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