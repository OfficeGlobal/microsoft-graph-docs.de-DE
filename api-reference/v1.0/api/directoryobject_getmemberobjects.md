# <a name="get-member-objects"></a>Mitgliedsobjekte abrufen

 Gibt alle Gruppen und Verzeichnisrollen zurück, in denen ein Benutzer-, Gruppen- oder Verzeichnisobjekt Mitglied ist. Diese Funktion ist transitiv. 
 > Hinweis: Nur Benutzer können Verzeichnisrollen angehören.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | User.Read.All und Group.Read.All, Directory.Read.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | User.Read.All und Group.Read.All, Directory.Read.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |
| Content-Type  | application/json  |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.

| Parameter    | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|securityEnabledOnly|Boolean| **true** gibt an, dass nur Sicherheitsgruppen, in denen die Person Mitglied ist, zurückgegeben werden sollen; **falsch** gibt an, dass alle Gruppen und Verzeichnisrollen, in denen die Person ein Mitglied ist, zurückgegeben werden sollen. **Hinweis**: Die Funktion kann nur für einen Benutzer aufgerufen werden, wenn der Parameter **true** lautet. |

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200, OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberObjects
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a>Antwort
Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "c9ee2d50-9e8a-4352-b97c-4c2c99557c22",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
