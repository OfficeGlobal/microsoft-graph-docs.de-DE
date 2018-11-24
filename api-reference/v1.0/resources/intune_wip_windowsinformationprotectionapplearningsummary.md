# <a name="windowsinformationprotectionapplearningsummary-resource-type"></a>windowsInformationProtectionAppLearningSummary-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Windows Information Protection App Learning – Zusammenfassungsentität.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[windowsInformationProtectionAppLearningSummaries auflisten](../api/intune_wip_windowsinformationprotectionapplearningsummary_list.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)-Objekte.|
|[windowsInformationProtectionAppLearningSummary abrufen](../api/intune_wip_windowsinformationprotectionapplearningsummary_get.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)|Lesen von Eigenschaften und Beziehungen des [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)-Objekts.|
|[windowsInformationProtectionAppLearningSummary erstellen](../api/intune_wip_windowsinformationprotectionapplearningsummary_create.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)|Erstellen eines neuen [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)-Objekts.|
|[windowsInformationProtectionAppLearningSummary löschen](../api/intune_wip_windowsinformationprotectionapplearningsummary_delete.md)|Keine|Löscht ein [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)-Objekt.|
|[windowsInformationProtectionAppLearningSummary aktualisieren](../api/intune_wip_windowsinformationprotectionapplearningsummary_update.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)|Aktualisieren der Eigenschaften eines [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für die WindowsInformationProtectionAppLearningSummary.|
|applicationName|String|Name der Anwendung|
|applicationType|[applicationType](../resources/intune_wip_applicationtype.md)|Anwendungstyp. Mögliche Werte sind: `universal` und `desktop`.|
|deviceCount|Int32|Geräteanzahl|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionAppLearningSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "String (identifier)",
  "applicationName": "String",
  "applicationType": "String",
  "deviceCount": 1024
}
```



