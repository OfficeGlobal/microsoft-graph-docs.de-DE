# <a name="educationclass-resource-type"></a>educationClass-Ressourcentyp

Stellt eine Klasse in einer Schule dar. Die **educationClass**-Ressource entspricht der Office 365-Gruppe und hat die gleiche ID. Kursteilnehmer sind reguläre Mitglieder der Klasse, Lehrer sind Besitzer und verfügen über entsprechende Rechte. Damit Office-Benutzeroberflächen ordnungsgemäß funktionieren, müssen Lehrer Mitglieder der Sammlungen der Lehrkräfte wie auch der Mitglieder sein.  


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[EducationClass abrufen](../api/educationclass_get.md) | [educationClass](educationclass.md) |Lesen von Eigenschaften und Beziehungen eines **educationClass**-Objekts.|
|[Mitglied hinzufügen](../api/educationclass_post_members.md) |[educationUser](educationuser.md)| Hinzufügen eines neuen **educationUser** für die Klasse durch Bereitstellen in der Navigationseigenschaft „members“.|
|[Mitglieder auflisten](../api/educationclass_list_members.md) |[educationUser](educationuser.md)-Sammlung| Abrufen einer **educationUser**-Objektsammlung.|
|[Kursteilnehmer entfernen](../api/educationclass_delete_members.md) |[educationUser](educationuser.md)| Entfernen eines **educationUser** aus der Klasse über die Navigationseigenschaft „members“.|
|[Schulen auflisten](../api/educationclass_list_schools.md) |[educationSchool](educationschool.md)-Sammlung| Abrufen einer **educationSchool**-Objektsammlung.|
|[Lehrer hinzufügen](../api/educationclass_post_teachers.md) |[educationUser](educationuser.md)| Hinzufügen eines neuen **educationUser** für die Klasse durch Bereitstellen in der Navigationseigenschaft „teachers“.|
|[Lehrer auflisten](../api/educationclass_list_teachers.md) |[educationUser](educationuser.md)-Sammlung| Abrufen einer Liste der Lehrer für die Klasse|
|[Lehrer entfernen](../api/educationclass_delete_teachers.md) |[educationUser](educationuser.md)| Entfernen eines **educationUser** aus der Klasse über die Navigationseigenschaft „teachers“.|
|[Gruppe abrufen](../api/educationclass_get_group.md) |[Gruppe](group.md)| Abrufen der Office 365-**Gruppe**, die dieser **educationClass** entspricht.|
|[Aktualisieren](../api/educationclass_update.md) | [educationClass](educationclass.md)    |Aktualisieren eines **educationClass**-Objekts. |
|[Löschen](../api/educationclass_delete.md) | Keine |Löschen eines **educationClass**-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id| Zeichenfolge| Eindeutiger Bezeichner für die Klasse|
|Beschreibung|Zeichenfolge| Beschreibung der Klasse|
|displayName|Zeichenfolge| Der Name der Klasse|
|mailNickname|Zeichenfolge| E-Mail-Name zum Senden von E-Mails an alle Mitglieder, wenn diese Option aktiviert ist. |
|createdBy|[identitySet](identityset.md)| Entität, die die Klasse erstellt hat. |
|classCode|Zeichenfolge| Von der Schule verwendeter Klassencode zum Identifizieren der Klasse|
|externalId|Zeichenfolge| ID der Klasse aus dem Synchronisierungssystem |
|externalName|Zeichenfolge|Der Name der Klasse im Synchronisierungssystem|
|externalSource|educationExternalSource| Quelle, aus der diese Klasse erstellt wurde. Mögliche Werte sind `sis`, `manual`,`unknownFutureValue`.|
|Zeitraum|[educationTerm](educationterm.md)|Der Zeitraum für diese Klasse.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Mitglieder|[educationUser](../resources/educationuser.md)-Sammlung| Alle Benutzer in der Klasse. Lässt Nullwerte zu.|
|Schulen|[educationSchool](../resources/educationschool.md)-Sammlung| Alle Schulen, denen dieser Klasse zugeordnet ist. Lässt Nullwerte zu.|
|Lehrer|[educationUser](../resources/educationuser.md)-Sammlung|  Alle Lehrer in der Klasse. Lässt Nullwerte zu.|
|Gruppe|[Gruppe](../resources/group.md)| Die Directory-Gruppe, die dieser Klasse entspricht.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationClass"
}-->

```json
{
  "id": "String",
  "description": "String",
  "classCode": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "string",
  "mailNickname": "String",
  "term": {"@odata.type": "microsoft.graph.educationTerm"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationClass resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
