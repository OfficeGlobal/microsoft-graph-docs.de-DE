# <a name="remoteassistancepartner-resource-type"></a>remoteAssistancePartner-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die Ressource remoteAssistPartner repräsentiert die Metadaten und den Status eines bestimmten Partnerdienstes für die Remoteunterstützung.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[remoteAssistancePartners auflisten](../api/intune_remoteassistance_remoteassistancepartner_list.md)|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)-Objekte.|
|[remoteAssistancePartner abrufen](../api/intune_remoteassistance_remoteassistancepartner_get.md)|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)|Lesen von Eigenschaften und Beziehungen des [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)-Objekts.|
|[remoteAssistancePartner erstellen](../api/intune_remoteassistance_remoteassistancepartner_create.md)|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)|Erstellen eines neuen [RemoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)-Objekts.|
|[remoteAssistancePartner löschen](../api/intune_remoteassistance_remoteassistancepartner_delete.md)|Keine|Löschen eines [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md).|
|[remoteAssistancePartner aktualisieren](../api/intune_remoteassistance_remoteassistancepartner_update.md)|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)|Aktualisieren der Eigenschaften eines [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)-Objekts.|
|[beginOnboarding-Aktion](../api/intune_remoteassistance_remoteassistancepartner_beginonboarding.md)|Keine|Noch nicht dokumentiert.|
|[disconnect-Aktion](../api/intune_remoteassistance_remoteassistancepartner_disconnect.md)|Keine|Noch nicht dokumentiert.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Der eindeutige Bezeichner des Partners.|
|displayName|Zeichenfolge|Der Anzeigename des Partners.|
|onboardingUrl|Zeichenfolge|Die URL des Onboarding-Portals des Partners, in dem ein Administrator den Remoteunterstützungsdienst konfigurieren kann.|
|onboardingStatus|[remoteAssistanceOnboardingStatus](../resources/intune_remoteassistance_remoteassistanceonboardingstatus.md)|TBD. Mögliche Werte sind: `notOnboarded`, `onboarding` und `onboarded`.|
|lastConnectionDateTime|DateTimeOffset|Zeitstempel der letzten vom TEM-Partner an Intune gesendeten Anforderung|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteAssistancePartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "String (identifier)",
  "displayName": "String",
  "onboardingUrl": "String",
  "onboardingStatus": "String",
  "lastConnectionDateTime": "String (timestamp)"
}
```



