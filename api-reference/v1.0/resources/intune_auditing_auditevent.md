# <a name="auditevent-resource-type"></a>auditEvent-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Eine Klasse, die die Eigenschaften für das Audit-Ereignis enthält.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[auditEvents auflisten](../api/intune_auditing_auditevent_list.md)|[auditEvent](../resources/intune_auditing_auditevent.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [auditEvent](../resources/intune_auditing_auditevent.md)-Objekte.|
|[auditEvent abrufen](../api/intune_auditing_auditevent_get.md)|[auditEvent](../resources/intune_auditing_auditevent.md)|Lesen von Eigenschaften und Beziehungen des [auditEvent](../resources/intune_auditing_auditevent.md)-Objekts.|
|[auditEvent erstellen](../api/intune_auditing_auditevent_create.md)|[auditEvent](../resources/intune_auditing_auditevent.md)|Erstellen eines neuen [auditEvent](../resources/intune_auditing_auditevent.md)-Objekts.|
|[auditEvent löschen](../api/intune_auditing_auditevent_delete.md)|Keine|Löscht ein [auditEvent](../resources/intune_auditing_auditevent.md)-Objekt.|
|[auditEvent aktualisieren](../api/intune_auditing_auditevent_update.md)|[auditEvent](../resources/intune_auditing_auditevent.md)|Aktualisieren der Eigenschaften eines [auditEvent](../resources/intune_auditing_auditevent.md)-Objekts.|
|[getAuditCategories-Funktion](../api/intune_auditing_auditevent_getauditcategories.md)|String-Sammlung|Noch nicht dokumentiert|
|[getAuditActivityTypes-Funktion](../api/intune_auditing_auditevent_getauditactivitytypes.md)|String-Sammlung|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität.|
|displayName|String|Anzeigename des Ereignisses|
|componentName|String|Komponentenname|
|actor|[auditActor](../resources/intune_auditing_auditactor.md)|AAD-Benutzer und -Anwendung, die dem Audit-Ereignis zugeordnet sind.|
|activity|String|Anzeigename der Aktivität|
|activityDateTime|DateTimeOffset|Datum und Uhrzeit in UTC, zu der die Aktivität ausgeführt wurde.|
|activityType|String|Der Typ der Aktivität, die ausgeführt wurde.|
|activityOperationType|String|Der HTTP-Vorgangstyp der Aktivität|
|activityResult|String|Das Ergebnis der Aktivität|
|correlationId|Guid|Die Clientanforderungs-ID, die zum Korrelieren der Aktivität innerhalb des Systems verwendet wird.|
|resources|[auditResource](../resources/intune_auditing_auditresource.md)-Sammlung|Ressourcen, die geändert werden.|
|category|String|Audit-Kategorie|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "String (identifier)",
  "displayName": "String",
  "componentName": "String",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "String",
    "userPermissions": [
      "String"
    ],
    "applicationId": "String",
    "applicationDisplayName": "String",
    "userPrincipalName": "String",
    "servicePrincipalName": "String",
    "ipAddress": "String",
    "userId": "String"
  },
  "activity": "String",
  "activityDateTime": "String (timestamp)",
  "activityType": "String",
  "activityOperationType": "String",
  "activityResult": "String",
  "correlationId": "<Unknown Primitive Type Edm.Guid>",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "String",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "String",
          "oldValue": "String",
          "newValue": "String"
        }
      ],
      "type": "String",
      "resourceId": "String"
    }
  ],
  "category": "String"
}
```



