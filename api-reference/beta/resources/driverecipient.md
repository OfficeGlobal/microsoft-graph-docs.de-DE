# <a name="driverecipient-resource-type"></a>DriveRecipient-Ressourcentyp

Die **DriveRecipient**-Ressource stellt eine Person, eine Gruppe oder einen anderen Empfänger für die Freigabe mit der [Einladen](../api/item_invite.md)-Aktion dar.

## <a name="json-representation"></a>JSON-Darstellung

<!-- { 
  "blockType": "resource", 
  "@odata.type": "microsoft.graph.driveRecipient", 
  "optionalProperties": ["alias", "objectId", "email"] } -->
```json
{
  "email": "string",
  "alias": "string",
  "objectId": "string",
}
```

## <a name="properties"></a>Eigenschaften
Die Empfängerressource besitzt die folgenden Eigenschaften.

| Eigenschaftenname | Typ   | Beschreibung                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| E-Mail         | String | Die E-Mail-Adresse des Empfängers, wenn der Empfänger eine zugehörige E-Mail-Adresse aufweist.                  |
| Alias         | String | Der Alias des Domänenobjekts, für Fälle, in denen keine E-Mail-Adresse verfügbar ist (z. B. bei Sicherheitsgruppen). |
| objectId      | String | Der eindeutige Bezeichner für den Empfänger im Verzeichnis.                                               |

## <a name="remarks"></a>Bemerkungen

Bei Verwendung von [invite](../api/item_invite.md) zum Hinzufügen von Berechtigungen kann im DriveRecipient **email**, **alias** oder **objectId** angegeben sein. Nur einer dieser Werte ist erforderlich.

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation"
} -->
