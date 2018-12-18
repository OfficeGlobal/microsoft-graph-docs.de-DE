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
# <a name="domaindnscnamerecord-resource-type"></a>domainDnsCnameRecord-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt einen CNAME-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität [DomainDnsRecord](domaindnsrecord.md).


## <a name="methods"></a>Methoden
Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|canonicalName|String| Der kanonische Name des CNAME-Eintrags. Wird verwendet, um den CNAME-Eintrag auf dem DNS-Host zu konfigurieren. |
|id|String| Eindeutiger Bezeichner, der dieser Entität zugewiesen ist. Lässt keine Nullwerte zu, schreibgeschützt.|
|isOptional|Boolean| Wenn „false“, muss der CNAME-Eintrag vom Kunden auf dem DNS-Host konfiguriert werden, damit Microsoft-Onlinedienste ordnungsgemäß mit der Domäne funktionieren. Lässt keine Nullwerte zu. |
|label|String| Wert, der beim Konfigurieren der *alias/host/name*-Eigenschaft des CNAME-Eintrags auf dem DNS-Host verwendet wird. |
|recordType|String| Typ des DNS-Eintrags. Der Wert ist immer *CName*. Schlüssel|
|supportedService|String| Microsoft-Onlinedienst oder Feature mit Abhängigkeit von diesem CNAME-Eintrag.</br></br>Kann einer der folgenden Werte sein: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*|
|ttl|Int32| Wert, der beim Konfigurieren der Eigenschaft für die Gültigkeitsdauer (time-to-live (ttl) des CNAME-Eintrags auf dem DNS-Host verwendet werden soll. Lässt keine Nullwerte zu. |

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

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