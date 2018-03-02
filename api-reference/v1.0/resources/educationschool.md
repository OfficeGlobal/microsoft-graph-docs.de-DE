# <a name="educationschool-resource-type"></a>educationSchool-Ressourcentyp

Eine Bildungseinrichtung. Die **educationSchool**-Ressource entspricht derzeit einer [administrativeUnit](../../beta/resources/administrativeunit.md)-Ressource und hat dieselbe ID.  

>**Hinweis:** Die Ressourcen **administrativeUnit** und **educationOrganization** befinden sich aktuell im Betastadium. Wenn Sie diese Ressourcen verwenden, müssen Sie das [Änderungsprotokoll](../../../concepts/changelog.md) in regelmäßigen Abständen überprüfen. Wenn Ressourcen der Microsoft Graph-API im v1.0-Endpunkt veröffentlicht werden, wird dies im Änderungsprotokoll vermerkt. Wenn Ihre App die Ressourcen **administrativeUnit** oder **educationOrganization** nutzt, müssen Sie die Basisanforderungs-URLs wie im folgenden Codeblock deklarieren.  
  ```JavaScript
  var v1BaseUrl = “https://graph.microsoft.com/v1.0/education”;
  var betaBaseUrl = “https://graph.microsoft.com/beta/education”;  // for administrativeUnit and educationOrganization
  ```

Diese Ressource ist ein Untertyp von [educationOrganization](../../beta/resources/educationorganization.md).


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
|[AdministrativeUnit abrufen](../api/educationschool_get_administrativeunit.md) |[administrativeUnit](../../beta/resources/administrativeunit.md)| Abrufen der **administrativeUnit**, die dieser **educationSchool** entspricht.|
|[Aktualisieren](../api/educationschool_update.md) | [educationSchool](educationschool.md) |Aktualisieren eines **educationSchool**-Objekts. |
|[Löschen](../api/educationschool_delete.md) | Keine |Löschen eines **educationSchool**-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|String|GUID dieser Schule|
|displayName| String| Anzeigename der Schule| 
|description| String | Beschreibung der Schule| 
|status| string| Schreibgeschützt. Mögliche Werte: `inactive`, `active`, `expired`, `deleteable`.|
|externalSource| string| Schreibgeschützt.  Mögliche Werte sind: `sis`, `manual` und `unknownFutureValue`.|
|principalEmail| String| Die E-Mail-Adresse des Prinzipals|
|principalName| String | Der Name des Prinzipals|
|externalPrincipalId| String | Die ID des Prinzipals im Synchronisierungssystem |
|highestGrade|String| Höchste unterrichtete Klasse |
|lowestGrade|String| Niedrigste unterrichtete Klasse |
|schoolNumber|String| Schulnummer|
|externalId|String| Die ID der Schule im Synchronisierungssystem |
|phone|String| Die Telefonnummer der Schule |
|fax|String| Die Faxnummer der Schule |
|address|[physicalAddress](physicaladdress.md)| Die Adresse der Schule|
|createdBy|[identitySet](identityset.md)|Entität, die Schule erstellt hat.|


## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|classes|[educationClass](educationclass.md)-Sammlung| In der Schule unterrichtete Klassen. Lässt Nullwerte zu.|
|users|[educationUser](educationuser.md)-Sammlung| Benutzer in der Schule. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
