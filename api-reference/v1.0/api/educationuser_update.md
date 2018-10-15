# <a name="update-educationuser-properties"></a>EducationUser-Eigenschaften aktualisieren

Aktualisieren der Eigenschaften eines **educationuser**-Objekts.
## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) |  Nicht unterstützt  |
|Delegiert (persönliches Microsoft-Konto) |  Nicht unterstützt  |
|Anwendung | EduRoster.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a>Anforderungsheader
| Kopfzeile       | Wert |
|:---------------|:--------|
| Autorisierung  | Bearer {token}. Erforderlich.  |
| Inhaltstyp  | application/json  |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|displayName| Zeichenfolge| Der Anzeigename des Benutzers|
|givenName| Zeichenfolge | Vorname |
|middleName| Zeichenfolge | Zweiter Vorname des Benutzers|
|surname| Zeichenfolge | Nachname des Benutzers|
|mail| Zeichenfolge| E-Mail-Adresse|
|mobilePhone| Zeichenfolge | Mobiltelefonnummer des Benutzers |
|externalSource|Zeichenfolge| Die möglichen Werte sind: `sis`, `manual`, `enum_sentinel`.|
|externalSource|Zeichenfolge| Quelle, aus der dieser Benutzer erstellt wurde.  Die möglichen Werte sind: `sis`, `manual`, `enum_sentinel`.|
|mailingAddress|[physicalAddress](../resources/physicaladdress.md)| E-Mail-Adresse des Benutzers|
|residenceAddress|[physicalAddress](../resources/physicaladdress.md)| Die Wohnadresse des Benutzers|
|primaryRole|Zeichenfolge| Standardrolle für einen Benutzer.  Die Rolle des Benutzers kann in einer einzelnen Klasse unterschiedlich sein. Die möglichen Werte sind: `student`, `teacher`, `enum_sentinel`.|
|Kursteilnehmer|[educationStudent](../resources/educationstudent.md)| Ist die primäre Rolle Kursteilnehmer, enthält dieser Block spezifische Daten für Kursteilnehmer.|
|Lehrer|[educationTeacher](../resources/educationteacher.md)| Ist die primäre Rolle Lehrer, enthält dieser Block lehrerspezifische Daten.|


## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [educationUser](../resources/educationuser.md)-Objekt im Antworttext zurückgegeben.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "update_educationuser"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/users/{user-id}
Content-type: application/json
Content-length: 508

{
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 508

{
  "id": "13020",
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
  "mail": "rogelioC@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
  },
  "externalSource": "sis",
  "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "primaryRole": "student",
  "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "student": {
      "externalId": "13005",
      "birthDate": "2001-01-01T00:00:00Z"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationuser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->