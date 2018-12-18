---
title: domainDnsSrvRecord-Ressourcentyp
description: Stellt einen SRV-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität DomainDnsRecord.
author: lleonard-msft
ms.openlocfilehash: d8fbdb6a99e2a4c88b38d350ace3976842eb7f92
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318823"
---
# <a name="domaindnssrvrecord-resource-type"></a>domainDnsSrvRecord-Ressourcentyp

Stellt einen SRV-Eintrag dar, der der DNS-Zonendatei einer bestimmten Domäne im Mandanten hinzugefügt wird. Geerbt von der Entität [DomainDnsRecord](domaindnsrecord.md).

## <a name="methods"></a>Methoden
Direkte Abfragen dieser Ressource werden nicht unterstützt. Informationen zum Abfragen von Domänendiensteinträgen finden Sie im Thema [Domäne](domain.md).

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|String| Eindeutiger Bezeichner, der dieser Entität zugewiesen ist. Lässt keine Nullwerte zu, schreibgeschützt.|
|isOptional|Boolean| Wenn „false“, muss der SRV-Eintrag vom Kunden auf dem DNS-Host konfiguriert werden, damit Microsoft-Onlinedienste ordnungsgemäß mit der Domäne funktionieren. |
|label|String| Wert, der beim Konfigurieren der *name*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet wird. |
|nameTarget|String| Wert, der beim Konfigurieren der *target*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll. |
|port|Int32| Wert, der beim Konfigurieren der *port*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll. |
|priority|Int32| Wert, der beim Konfigurieren der *priority*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll. |
|protocol|String| Wert, der beim Konfigurieren der *protocol*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll. |
|recordType|String|  Typ des DNS-Eintrags. Der Wert ist immer *Srv*. Schlüssel |
|service|String| Wert, der beim Konfigurieren der *service*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll. |
|supportedService|String| Microsoft-Onlinedienst oder Feature mit Abhängigkeit von diesem SRV-Eintrag.</br></br>Kann einer der folgenden Werte sein: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune* |
|ttl|Int32| Wert, der beim Konfigurieren der Eigenschaft für die Gültigkeitsdauer (*time-to-live (ttl)*) des SRV-Eintrags auf dem DNS-Host verwendet werden soll. Lässt keine Nullwerte zu. |
|weight|Int32| Wert, der beim Konfigurieren der *weight*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll. |

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

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