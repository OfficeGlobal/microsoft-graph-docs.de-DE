# <a name="deviceoperatingsystemsummary-resource-type"></a>deviceOperatingSystemSummary-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Betriebssystem des Geräts – Zusammenfassung.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|androidCount|Int32|Anzahl der Android-Geräte.|
|iosCount|Int32|Anzahl der iOS-Geräte.|
|macOSCount|Int32|Anzahl der Mac OS X-Geräte.|
|windowsMobileCount|Int32|Anzahl der Windows Mobile-Geräte.|
|windowsCount|Int32|Anzahl der Windows-Geräte.|
|unknownCount|Int32|Anzahl von unbekannten Geräten.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCount": 1024,
  "iosCount": 1024,
  "macOSCount": 1024,
  "windowsMobileCount": 1024,
  "windowsCount": 1024,
  "unknownCount": 1024
}
```



