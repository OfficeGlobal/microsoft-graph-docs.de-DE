---
title: Ressourcentyp registryKeyState
description: Enthält Informationen zur Registrierung wichtige Änderungen im Zusammenhang mit der Benachrichtigung, und der Prozess, der die Registrierungsschlüssel geändert.
localization_priority: Normal
ms.openlocfilehash: 688c690083e24dc6c8ee7229498910befd0fdf3e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804676"
---
# <a name="registrykeystate-resource-type"></a>Ressourcentyp registryKeyState

Enthält Informationen zur Registrierung wichtige Änderungen im Zusammenhang mit der Benachrichtigung, und der Prozess, der die Registrierungsschlüssel geändert.

## <a name="properties"></a>Eigenschaften

| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|Struktur|registryHive|Ein [Windows-Registrierungsstruktur](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) : <ul><li>HKEY_CURRENT_CONFIG</li> <li>HKEY_CURRENT_USER</li> <li>HKEY_LOCAL_MACHINE\SAM</li> <li>HKEY_LOCAL_MACHINE\Security</li> <li>HKEY_LOCAL_MACHINE\Software</li> <li>HKEY_LOCAL_MACHINE\SYSTEM</li> <li>HKEY_USERS\\. Die standardmäßigen.</li></ul> Mögliche Werte sind: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSamSoftware`, `localMachineSystem` und `usersDefault`.|
|Key|Zeichenfolge|Aktuelle (d. h. geänderten) Registrierungsschlüssel (schließt die Struktur).|
|oldKey|Zeichenfolge|Frühere (d. h., bevor geändert) Registrierungsschlüssel (schließt die Struktur).|
|oldValueData|Zeichenfolge|Frühere (d. h., bevor geändert) Schlüsselwert Registrierungsdaten (Inhalt).|
|oldValueName|Zeichenfolge|Frühere (d. h., bevor geändert) Registrierung Schlüsselwertname.|
|Operation|registryOperation|Der Vorgang, der der Name des Registrierungsschlüssels und/oder Wert geändert. Mögliche Werte: sind `unknown`, `create`, `modify` und `delete`.|
|processId|Int32|Werden Sie ID (PID) des Prozesses, der den Registrierungsschlüssel (Prozess, der in der Auflistung Warnung 'Prozesse' Details angezeigt werden) geändert.|
|valueData|Zeichenfolge|Aktuelle (d. h. geänderten) Schlüsselwert Registrierungsdaten (Inhalt).|
|Wertname|Zeichenfolge|Aktuelle (d. h. geänderten) Registrierung Schlüsselwertname|
|Werttyp|registryValueType|[Schlüsselwert Registrierungstyp](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li>REG_BINARY</li> <li>REG_DWORD</li> <li>REG_DWORD_LITTLE_ENDIAN</li> <li>REG_DWORD_BIG_ENDIAN</li><li>REG_EXPAND_SZ</li> <li>REG_LINK</li> <li>REG_MULTI_SZ</li> <li>REG_NONE</li> <li>REG_QWORD</li> <li>REG_QWORD_LITTLE_ENDIAN</li> <li>REG_SZ</li></ul> Mögliche Werte sind: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian` und `sz`.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.registryKeyState"
}-->

```json
{
  "hive": "@odata.type: microsoft.graph.registryHive",
  "key": "String",
  "oldKey": "String",
  "oldValueData": "String",
  "oldValueName": "String",
  "operation": "@odata.type: microsoft.graph.registryOperation",
  "processId": 1024,
  "valueData": "String",
  "valueName": "String",
  "valueType": "@odata.type: microsoft.graph.registryValueType"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "registryKeyState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
