---
title: Benutzer abrufen
description: Dient zum Abrufen der Eigenschaften und der Beziehungen des Benutzerobjekts.
author: dkershaw10
ms.openlocfilehash: f26b77ccb21c4b25cc3d869582ce1d4064b16f53
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304662"
---
# <a name="get-a-user"></a>Benutzer abrufen

Dient zum Abrufen der Eigenschaften und der Beziehungen des Benutzerobjekts.

> Hinweis: Durch das Auflisten eines Benutzers wird nur ein standardmäßiger Satz von Eigenschaften zurückgegeben (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Verwenden Sie `$select`, um die anderen Eigenschaften und Beziehungen für das [user](../resources/user.md)-Objekt abzurufen.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegiert (persönliches Microsoft-Konto) | User.Read, User.ReadWrite    |
|Anwendung | User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
Für einen bestimmten Benutzer:<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}
```

Für den angemeldeten Benutzer:<!-- { "blockType": "ignored" } -->
```http
GET /me
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.

Standardmäßig wird nur ein begrenzter Satz von Eigenschaften zurückgegeben (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_). 

Um einen alternativen Eigenschaftensatz zurückzugeben, müssen Sie den gewünschten Satz von [user](../resources/user.md)-Eigenschaften mithilfe des Odata-Abfrageparameters `$select` angeben. Um zum Beispiel _displayName_, _givenName_ und _postalCode_ zurückzugeben, fügen Sie Folgendes zur Abfrage hinzu: `$select=displayName,givenName,postalCode`.

## <a name="request-headers"></a>Anforderungsheader
| Header       | Wert|
|:-----------|:------|
| Authorization  | Bearer {token}. Erforderlich. |
| Content-Type   | application/json |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [user](../resources/user.md)-Objekt im Antworttext zurückgegeben.

## <a name="examples"></a>Beispiele

### <a name="example-1-standard-users-request"></a>Beispiel 1: Standard-Benutzeranforderung

Standardmäßig wird nur ein begrenzter Satz von Eigenschaften zurückgegeben (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_). Dieses Beispiel zeigt die standardmäßige Anforderung und Antwort. 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}
```

##### <a name="response"></a>Antwort

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "businessPhones": [
       "businessPhones-value"
   ],
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "jobTitle": "jobTitle-value",
   "mail": "mail-value",
   "mobilePhone": "mobilePhone-value",
   "officeLocation": "officeLocation-value",
   "preferredLanguage": "preferredLanguage-value",
   "surname": "surname-value",
   "userPrincipalName": "userPrincipalName-value",
   "id": "id-value"
}
```


### <a name="example-2-signed-in-user-request"></a>Beispiel 2: Anforderung des angemeldeten Benutzers

Sie können die Benutzerinformationen des angemeldeten Benutzers abrufen, indem Sie `/users/{id | userPrincipalName}` durch `/me` ersetzen.

##### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/me
```
##### <a name="response"></a>Antwort

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "businessPhones": [
       "businessPhones-value"
   ],
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "jobTitle": "jobTitle-value",
   "mail": "mail-value",
   "mobilePhone": "mobilePhone-value",
   "officeLocation": "officeLocation-value",
   "preferredLanguage": "preferredLanguage-value",
   "surname": "surname-value",
   "userPrincipalName": "userPrincipalName-value",
   "id": "id-value"
}
```

### <a name="example-3-users-request-using-select"></a>Beispiel 3: Benutzeranforderung mit $select

Wenn Sie einen anderen Eigenschaftensatz benötigen, können Sie den OData-Abfrageparameter `$select` verwenden. Um zum Beispiel _displayName_, _givenName_ und _postalCode_ zurückzugeben, fügen Sie Folgendes zur Abfrage hinzu: `$select=displayName,givenName,postalCode`.

##### <a name="request"></a>Anforderung
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}?$select=displayName,givenName,postalCode
```
##### <a name="response"></a>Antwort
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "postalCode": "postalCode-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
