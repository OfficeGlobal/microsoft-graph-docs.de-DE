# <a name="educationschool-resource-type"></a>educationSchool-Ressourcentyp

Eine Ressource, eine Schule darstellt und zum Verwalten der Klassen, Lehrkräfte und Schüler der repräsentierten Schule verwendet wird.  


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Get](../api/educationschool_get.md) | [educationSchool](educationschool.md) |Lesen von Eigenschaften und Beziehungen eines **educationSchool**-Objekts.|
|[Klasse hinzufügen](../api/educationschool_post_classes.md) |[educationClass](educationclass.md)| Hinzufügen einer neuen **educationClass** für die Schule durch Bereitstellen in der Navigationseigenschaft „classes“.|
|[Klassen auflisten](../api/educationschool_list_classes.md) |[educationClass](educationclass.md)-Sammlung| Abrufen der **educationClass**-Objektsammlung.|
|[Klasse entfernen](../api/educationschool_delete_classes.md) |[educationClass](educationclass.md)| Entfernen einer **educationClass** von der Schule über die Navigationseigenschaft „classes“.|
|[Benutzer hinzufügen](../api/educationschool_post_users.md) |[educationUser](educationuser.md)| Hinzufügen eines neuen **educationUser** für die Schule durch Bereitstellen in der Navigationseigenschaft **users**.|
|[Benutzer auflisten](../api/educationschool_list_users.md) |[educationUser](educationuser.md)-Sammlung| Abrufen der **educationUser**-Objektsammlung.|
|[Benutzer entfernen](../api/educationschool_delete_users.md) |[educationUser](educationuser.md)| Entfernen eines **educationUser** von der Schule über die Navigationseigenschaft **users**.|
|[Aktualisieren](../api/educationschool_update.md) | [educationSchool](educationschool.md) |Aktualisieren eines **educationSchool**-Objekts. |
|[Löschen](../api/educationschool_delete.md) | Keine |Löschen eines **educationSchool**-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|ID|Zeichenfolge|GUID dieser Schule|
|displayName| Zeichenfolge| Anzeigename der Schule| 
|Beschreibung| Zeichenfolge | Beschreibung der Schule| 
|Zustand| Zeichenfolge| Schreibgeschützt. Die möglichen Werte sind: `inactive`, `active`, `expired`, `deleteable`.|
|externalSource| educationExternalSource| Schreibgeschützt.  Die möglichen Werte sind: `sis`, `manual`, `unknownFutureValue`.|
|principalEmail| Zeichenfolge| Die E-Mail-Adresse des Prinzipals|
|principalName| Zeichenfolge | Der Name des Prinzipals|
|externalPrincipalId| Zeichenfolge | Die ID des Prinzipals im Synchronisierungssystem |
|highestGrade|Zeichenfolge| Höchste unterrichtete Klasse |
|lowestGrade|Zeichenfolge| Niedrigste unterrichtete Klasse |
|schoolNumber|Zeichenfolge| Schulnummer|
|externalId|Zeichenfolge| Die ID der Schule im Synchronisierungssystem |
|Telefon|Zeichenfolge| Die Telefonnummer der Schule |
|Fax|Zeichenfolge| Die Faxnummer der Schule |
|Adresse|[physicalAddress](physicaladdress.md)| Die Adresse der Schule|
|createdBy|[identitySet](identityset.md)|Entität, die Schule erstellt hat.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Klassen|[educationClass](educationclass.md)-Sammlung| In der Schule unterrichtete Klassen. Lässt Nullwerte zu.|
|users|[educationUser](educationuser.md)-Sammlung| Benutzer in der Schule. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.educationOrganization",
  "@odata.type": "microsoft.graph.educationSchool"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "description": "String",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "highestGrade": "String",
  "lowestGrade": "String",
  "schoolNumber": "String",
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalId": "String",
  "fax": "String",
  "phone": "String",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
