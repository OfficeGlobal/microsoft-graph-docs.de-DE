---
title: registryKeyState-Ressourcentyp
description: Enthält Informationen zu Registrierungsschlüssel Änderungen im Zusammenhang mit der Warnung und dem Prozess, der die Registrierungsschlüssel geändert hat.
localization_priority: Normal
ms.openlocfilehash: d07b0b6f502794154b400444eaf3854535e04547
ms.sourcegitcommit: a4773239d8559899c3f9433b3073e250a56d2e04
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/13/2019
ms.locfileid: "29994426"
---
# <a name="registrykeystate-resource-type"></a>registryKeyState-Ressourcentyp

Enthält Informationen zu Registrierungsschlüssel Änderungen im Zusammenhang mit der Warnung und dem Prozess, der die Registrierungsschlüssel geändert hat.

## <a name="properties"></a>Eigenschaften

| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|Struktur|registryHive|Eine [Windows-Registrierungsstruktur](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) : <ul><li>HKEY_CURRENT_CONFIG</li> <li>HKEY_CURRENT_USER</li> <li>HKEY_LOCAL_MACHINE\SAM</li> <li>HKEY_LOCAL_MACHINE\Security</li> <li>HKEY_LOCAL_MACHINE\Software</li> <li>HKEY_LOCAL_MACHINE\System</li> <li>HKEY_USERS\\. Standard.</li></ul> Mögliche Werte: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.|
|Schlüssel|String|Aktueller (d.h. Geänderter) Registrierungsschlüssel (schließt HIVE aus).|
|oldKey|String|Vorheriger (d. h. vor geänderter) Registrierungsschlüssel (schließt HIVE aus).|
|oldValueData|String|Frühere (d. h. geänderte) Registrierungsschlüssel Wertdaten (Inhalte).|
|oldValueName|String|Vorheriger (also vor geänderter) Registrierungsschlüssel-Wertname.|
|Vorgang|registryOperation|Vorgang, der den Namen und/oder Wert des Registrierungsschlüssels geändert hat. Mögliche Werte sind: `unknown`, `create`, `modify` und `delete`.|
|processId|Int32|Prozess-ID (PID) des Prozesses, der den Registrierungsschlüssel geändert hat (Prozessdetails werden in der Alert ' Processes '-Auflistung angezeigt).|
|valueData|String|Aktuelle (d.h. geänderte) Registrierungsschlüssel Wertdaten (Inhalte).|
|valueName|String|Aktueller (d.h. Geänderter) Registrierungsschlüssel-Wertname|
|valueType|registryValueType|[Registrierungsschlüssel-Werttyp](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li>REG_BINARY</li> <li>REG_DWORD</li> <li>REG_DWORD_LITTLE_ENDIAN</li> <li>REG_DWORD_BIG_ENDIAN</li><li>REG_EXPAND_SZ</li> <li>REG_LINK</li> <li>REG_MULTI_SZ</li> <li>REG_NONE</li> <li>REG_QWORD</li> <li>REG_QWORD_LITTLE_ENDIAN</li> <li>REG_SZ</li></ul> Mögliche Werte sind: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian` und `sz`.|

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
