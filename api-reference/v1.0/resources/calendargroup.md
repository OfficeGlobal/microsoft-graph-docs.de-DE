# <a name="calendargroup-resource-type"></a>calendarGroup-Ressourcentyp

Eine Gruppe der Benutzerkalender.

## <a name="methods"></a>Methoden

| Methode                                                      | Rückgabetyp                        | Beschreibung                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [Kalendergruppen auflisten](../api/user_list_calendargroups.md)  | [Kalendersammlung](calendar.md) | Dient zum Abrufen der Kalendergruppen des Benutzers.                               |
| [Kalendergruppe erstellen](../api/user_post_calendargroups.md) | [Kalender](calendar.md)            | Erstellt eine neue Kalendergruppe.                                  |
| [Kalendergruppe abrufen](../api/calendargroup_get.md)           | [calendarGroup](calendargroup.md)  | Dient zum Lesen der Eigenschaften und der Beziehungen eines Kalendergruppenobjekts. |
| [Aktualisieren](../api/calendargroup_update.md)                    | [calendarGroup](calendargroup.md)  | Dient zum Aktualisieren des calendarGroup-Objekts.                                  |
| [Löschen](../api/calendargroup_delete.md)                    | Keine                               | Dient zum Löschen des calendarGroup-Objekts.                                  |
| [Kalender auflisten](../api/calendargroup_list_calendars.md)    | [Kalendersammlung](calendar.md) | Listet Kalender in einer Kalendergruppe auf.                           |
| [Kalender erstellen](../api/calendargroup_post_calendars.md)   | [Kalender](calendar.md)            | Erstellt einen neuen Kalender in einer Kalendergruppe.                    |

## <a name="properties"></a>Eigenschaften

| Eigenschaft  | Typ   | Beschreibung                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| name      | Zeichenfolge | Der Gruppenname.                                                                                                                                                                                           |
| changeKey | Zeichenfolge | Gibt die Version der Kalendergruppe an. Jedes Mal, wenn die Kalendergruppe geändert wird, wird auch ChangeKey geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen. Schreibgeschützt. |
| classId   | GUID   | Die Klassen-ID. Schreibgeschützt.                                                                                                                                                                          |
| id        | Zeichenfolge | Eindeutiger Bezeichner für die Gruppe. Schreibgeschützt.                                                                                                                                                                 |

## <a name="relationships"></a>Beziehungen

| Beziehung | Typ                               | Beschreibung                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| Kalender    | [Kalendersammlung](calendar.md) | Die Kalender in Kalendergruppe. Navigation-Eigenschaft Schreibgeschützt. Lässt Nullwerte zu. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "calendars"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.calendarGroup",
  "@odata.annotations": [
    {
      "property": "calendars",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "changeKey": "string",
  "classId": "guid",
  "id": "string (identifier)",
  "name": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "calendarGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
