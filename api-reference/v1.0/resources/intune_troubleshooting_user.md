# <a name="user-resource-type"></a>user-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Benutzer auflisten](../api/intune_troubleshooting_user_list.md)|[user](../resources/intune_troubleshooting_user.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [user](../resources/intune_troubleshooting_user.md)-Objekte.|
|[user abrufen](../api/intune_troubleshooting_user_get.md)|[user](../resources/intune_troubleshooting_user.md)|Lesen von Eigenschaften und Beziehungen des [user](../resources/intune_troubleshooting_user.md)-Objekts.|
|[user erstellen](../api/intune_troubleshooting_user_create.md)|[user](../resources/intune_troubleshooting_user.md)|Dient zum Erstellen eines neuen [user](../resources/intune_troubleshooting_user.md)-Objekts.|
|[user löschen](../api/intune_troubleshooting_user_delete.md)|Keine|Löscht einen [user](../resources/intune_troubleshooting_user.md).|
|[user aktualisieren](../api/intune_troubleshooting_user_update.md)|[user](../resources/intune_troubleshooting_user.md)|Aktualisieren der Eigenschaften eines [user](../resources/intune_troubleshooting_user.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner des Benutzers|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|deviceManagementTroubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)-Sammlung|Die Liste der Problembehandlungsereignisse für diesen Benutzer.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```



