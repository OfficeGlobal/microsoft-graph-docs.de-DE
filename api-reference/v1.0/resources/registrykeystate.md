# <a name="registrykeystate-resource-type"></a>Ressourcentyp registryKeyState

Enthält Informationen zu Änderungen am Registrierungsschlüssel im Zusammenhang mit der Warnung und dem Prozess, der den Registrierungsschlüssel geändert hat.

## <a name="properties"></a>Eigenschaften

| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|hive|registryHive|Ein [Windows-Registry-Hive](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives): <ul><li>HKEY_CURRENT_CONFIG</li> <li>HKEY_CURRENT_USER</li> <li>HKEY_LOCAL_MACHINE\SAM</li> <li>HKEY_LOCAL_MACHINE\Security</li> <li>HKEY_LOCAL_MACHINE\Software</li> <li>HKEY_LOCAL_MACHINE\System</li> <li>HKEY_USERS\\.Default.</li></ul> Mögliche Werte sind: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSamSoftware`, `localMachineSystem` und `usersDefault`.|
|Key|Zeichenfolge|Aktueller (d.h. geänderten) Registrierungsschlüssel (ohne HIVE).|
|oldKey|Zeichenfolge|Früherer (d.h., vor Änderung) Registrierungsschlüssel (ohne HIVE).|
|oldValueData|Zeichenfolge|Früherer (d.h., vor Änderung) Wertdaten des Registrierungsschlüssels (Inhalte).|
|oldValueName|Zeichenfolge|Früherer (d.h., vor Änderung) Wertname des Registrierungsschlüssels.|
|Operation|registryOperation|Der Vorgang, der den Namen des Registrierungsschlüssels und/oder den Wert geändert hat. Mögliche Werte: `unknown`, `create`, `modify`, `delete`.|
|processId|Int32|Prozess-ID (PID) des Prozesses, der den Registrierungsschlüssel geändert hat (Prozessdetails werden in der Sammlung der 'Prozesse'-Warnungen angezeigt).|
|valueData|Zeichenfolge|Aktuelle (d.h. geänderte) Wertdaten des Registrierungsschlüssels (Inhalte).|
|valueName|Zeichenfolge|Aktueller (d.h. geänderter) Wertname des Registrierungsschlüssels|
|valueType|registryValueType|[Werttyp des Registrierungsschlüssels](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li>REG_BINARY</li> <li>REG_DWORD</li> <li>REG_DWORD_LITTLE_ENDIAN</li> <li>REG_DWORD_BIG_ENDIAN</li><li>REG_EXPAND_SZ</li> <li>REG_LINK</li> <li>REG_MULTI_SZ</li> <li>REG_NONE</li> <li>REG_QWORD</li> <li>REG_QWORD_LITTLE_ENDIAN</li> <li>REG_SZ</li></ul> Mögliche Werte sind: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian` und `sz`.|

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