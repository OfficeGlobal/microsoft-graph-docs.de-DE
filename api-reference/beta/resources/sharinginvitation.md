# <a name="sharinginvitation-resource-type"></a>SharingInvitation-Ressourcentyp

Die **SharingInvitation**-Ressource gruppiert Datenelemente im Zusammenhang mit einer Einladung in einer einzelnen Struktur.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sharingInvitation"
}-->

```json
{
  "email": "string",
  "invitedBy": {"@odata.type": "microsoft.graph.identitySet" },
  "signInRequired": true
}

```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname  | Typ                          | Beschreibung                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| E-Mail          | String                        | Die für den Empfänger der Freigabeeinladung angegebene E-Mail-Adresse. Schreibgeschützt.                                          |
| invitedBy      | [identitySet](identityset.md) | Stellt Informationen zum Absender der Einladung bereit, der diese Berechtigung erstellt hat, wenn diese Informationen verfügbar sind. Schreibgeschützt. |
| signInRequired | Boolean                       | Bei `true` muss sich der Empfänger der Einladung anmelden, um auf das freigegebene Element zugreifen zu können. Schreibgeschützt.                     |

## <a name="remarks"></a>Bemerkungen 

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sharingInvitation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
