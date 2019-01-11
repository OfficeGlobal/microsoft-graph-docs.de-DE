---
title: LogonUser Ressourcentyp
description: Enthält Statusinformationen zu der angemeldete Benutzer auf diesem host
localization_priority: Normal
ms.openlocfilehash: 3b7862555c62eb16aaceaa53d4df58541426e08a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855594"
---
# <a name="logonuser-resource-type"></a>LogonUser Ressourcentyp

Enthält Statusinformationen zu der angemeldete Benutzer auf diesem host

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ |Beschreibung|
|:---------------|:--------|:----------|
|accountDomain|String|Domäne des Benutzerkontos verwendet für die Anmeldung.|
|accountName|String|Kontoname des verwendete Benutzerkonto für die Anmeldung.|
|accountType|String|Benutzerkontotyp pro Windows-Definition. Mögliche Werte: sind `unknown`, `standard`, `power` und `administrator`.|
|firstSeenDateTime|DateTimeOffset|DateTime, an dem die früheste Anmeldung durch dieses Benutzerkonto stattgefunden hat (Punkt Anbieter bestimmt). Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|lastSeenDateTime|DateTimeOffset|DateTime, an dem die aktuelle Anmeldung durch dieses Benutzerkonto aufgetreten ist. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.|
|logonId|String|Benutzer-Anmelde-ID|
|logonTypes|Collection von Objekten des Typs „String“|Auflistung der Anmeldetypen beobachtet aus der angemeldete Benutzer beim ersten bis zum letzten angezeigt. Mögliche Werte sind: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch` und `service`.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.logonUser"
}-->

```json
{
  "accountDomain": "String",
  "accountName": "String",
  "accountType": "String",
  "firstSeenDateTime": "String (timestamp)",
  "lastSeenDateTime": "String (timestamp)",
  "logonId": "String",
  "logonTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "logonUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
