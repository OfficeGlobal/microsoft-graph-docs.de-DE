# <a name="fileencryptioninfo-resource-type"></a>fileEncryptionInfo-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften für Dateiverschlüsselungsinformationen für die Inhaltsversion einer branchenspezifischen App.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|encryptionKey|Binary|Der Schlüssel, der zum Verschlüsseln des Inhalts der Datei verwendet wurde.|
|initializationVector|Binary|Der Initialisierungsvektor, der für den Verschlüsselungsalgorithmus verwendet wurde.|
|mac|Binary|Der Hash aus dem verschlüsselten Dateiinhalt + IV (Inhaltshash).|
|macKey|Binary|Der Schlüssel, der für den Abruf von mac verwendet wurde.|
|profileIdentifier|String|Die Bezeichner des Profils.|
|fileDigest|Binary|Der Digest der Datei vor der Verschlüsselung.|
|fileDigestAlgorithm|String|Der Dateidigestalgorithmus.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.fileEncryptionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileEncryptionInfo",
  "encryptionKey": "binary",
  "initializationVector": "binary",
  "mac": "binary",
  "macKey": "binary",
  "profileIdentifier": "String",
  "fileDigest": "binary",
  "fileDigestAlgorithm": "String"
}
```



