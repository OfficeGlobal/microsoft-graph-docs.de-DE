# <a name="windowsinformationprotectionnetworklearningsummary-resource-type"></a>windowsInformationProtectionNetworkLearningSummary-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Windows Information Protection – Netzwerk-Schulungszusammenfassungsentität
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[windowsInformationProtectionNetworkLearningSummaries auflisten](../api/intune_wip_windowsinformationprotectionnetworklearningsummary_list.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)-Objekte.|
|[WindowsInformationProtectionNetworkLearningSummary abrufen](../api/intune_wip_windowsinformationprotectionnetworklearningsummary_get.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)|Lesen von Eigenschaften und Beziehungen des [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)-Objekts.|
|[windowsInformationProtectionNetworkLearningSummary erstellen](../api/intune_wip_windowsinformationprotectionnetworklearningsummary_create.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)|Erstellen eines neuen [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)-Objekts.|
|[windowsInformationProtectionNetworkLearningSummary löschen](../api/intune_wip_windowsinformationprotectionnetworklearningsummary_delete.md)|Keine|Löscht ein [windowsInformationProtectionNetworkLearningSummary löschen](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)-Objekt.|
|[windowsInformationProtectionNetworkLearningSummary aktualisieren](../api/intune_wip_windowsinformationprotectionnetworklearningsummary_update.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)|Aktualisieren der Eigenschaften eines [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für die WindowsInformationProtectionNetworkLearningSummary.|
|url|String|Website-URL|
|deviceCount|Int32|Geräteanzahl|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.windowsInformationProtectionNetworkLearningSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "String (identifier)",
  "url": "String",
  "deviceCount": 1024
}
```



