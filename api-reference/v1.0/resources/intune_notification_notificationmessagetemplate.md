# <a name="notificationmessagetemplate-resource-type"></a>Ressourcentyp „notificationMessageTemplate“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Benachrichtigungs-E-Mails sind Nachrichten, die an Endbenutzer gesendet werden, die gegen die vom Administrator definierten Konformitätsrichtlinien verstoßen. Auswählen und konfigurieren können Administratoren die Benachrichtigungen in der Intune-Verwaltungskonsole auf der Seite für die Erstellung von Konformitätsrichtlinien, im Abschnitt „Actions for non-compliance“. Mit dem Objekt „notificationMessageTemplate“ können Sie eigene benutzerdefinierte Benachrichtigungen erstellen, aus denen Administratoren wählen können, wenn sie konfigurieren, welche Aktionen bei Verstößen gegen die Konformitätsrichtlinien ausgeführt werden sollen.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „notificationMessageTemplate“](../api/intune_notification_notificationmessagetemplate_list.md)|Sammlung von Objekten des Typs [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) auf.|
|[Abrufen von „notificationMessageTemplate“](../api/intune_notification_notificationmessagetemplate_get.md)|[notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md).|
|[Erstellen von „notificationMessageTemplate“](../api/intune_notification_notificationmessagetemplate_create.md)|[notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md)|Erstellt neue Objekte des Typs [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md).|
|[Löschen von „notificationMessageTemplate“](../api/intune_notification_notificationmessagetemplate_delete.md)|Keiner|Löscht Objekte des Typs [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md).|
|[Aktualisieren von „notificationMessageTemplate“](../api/intune_notification_notificationmessagetemplate_update.md)|[notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md)|Aktualisiert die Eigenschaften von Objekten des Typs [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md).|
|[Aktion „sendTestMessage“](../api/intune_notification_notificationmessagetemplate_sendtestmessage.md)|Keiner|Sendet eine Testnachricht unter Verwendung des für das Standardgebietsschema festgelegten Objekts des Typs „notificationMessageTemplate“.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts|
|displayName|String|Anzeigename für die Benachrichtigungs-E-Mail-Vorlage|
|defaultLocale|String|Standardgebietsschema, das verwendet wird, wenn das angeforderte Gebietsschema nicht verfügbar ist|
|brandingOptions|String|Optionen für das Branding der Nachrichtenvorlage. Das Branding wird in der Intune-Verwaltungskonsole definiert. Mögliche Werte sind: `none`, `includeCompanyLogo`, `includeCompanyName` und `includeContactInformation`.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|localizedNotificationMessages|Sammlung von Objekten des Typs [localizedNotificationMessages](../resources/intune_notification_localizednotificationmessage.md)|Liste der lokalisierten Nachrichten für die Benachrichtigungs-E-Mail-Vorlage|

## <a name="json-representation"></a>JSON-Darstellung
Unten sehen Sie eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.notificationMessageTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "defaultLocale": "String",
  "brandingOptions": "String"
}
```



