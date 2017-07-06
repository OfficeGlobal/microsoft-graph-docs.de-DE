# <a name="traverse-microsoft-graph"></a>Durchqueren von Microsoft Graph

Zusätzlich zur Verwendung der Microsoft Graph-API zum Lesen und Schreiben von Daten können Sie eine Reihe von Anforderungsmustern verwenden, um die Ressourcen in Microsoft Graph zu durchlaufen. Mithilfe des Metadatendokuments erhalten Sie auch einen Einblick in die Datenmodelle der Ressourcen und Beziehungen in Microsoft Graph.

## <a name="microsoft-graph-api-metadata"></a>Microsoft Graph-API-Metadaten

Das Metadatendokument ($metadata) wird im Dienststamm veröffentlicht. Über die folgenden URLs können Sie das Dienstdokument für v1.0 und die Betaversionen der Microsoft Graph-API anzeigen.

**Metadaten für Microsoft Graph-API v1.0**
```
    https://graph.microsoft.com/v1.0/$metadata
```

**Metadaten für Microsoft Graph-API Beta**

```
    https://graph.microsoft.com/beta/$metadata
```

Mithilfe der Metadaten können Sie das Datenmodell von Microsoft Graph sehen und verstehen, einschließlich Entitätstypen, komplexen Typen und Aufzählungen, aus denen Ressourcen bestehen, die in den Anforderungs- und Antwortpaketen dargestellt sind.

Die Metadaten können Sie verwenden, um die Beziehungen zwischen Entitäten in Microsoft Graph zu verstehen und URLs einzurichten, die zwischen diesen Entitäten navigieren.

Bei den Pfad-URL-Ressourcennamen, Abfrageparametern sowie den Aktionsparametern und -werten wird nicht nach Groß-/Kleinschreibung unterschieden. Bei zugewiesenen Werten, Entitäts-IDs und anderen base64-codierten Werten wird nach Groß-/Kleinschreibung unterschieden.

## <a name="view-a-collection-of-resources"></a>Anzeigen einer Sammlung von Ressourcen

Mit Microsoft Graph können Sie Ressourcen in einem Mandanten mithilfe von HTTP-GET-Abfragen anzeigen. Die Abfrageantwort umfasst Eigenschaften jeder Ressource, wobei jede Ressource von ihrer ID identifiziert wird. Das Format einer Ressourcen-ID kann eine GUID sein und ist in der Regel je nach Ressourcentyp unterschiedlich. 

Sie können die Sammlung von in einem Mandanten definierten Benutzern beispielsweise folgendermaßen abrufen:

```no-highlight 
GET https://graph.microsoft.com/v1.0/users HTTP/1.1
Authorization : Bearer {access_token}
```

Wenn der Vorgang erfolgreich ist, erhalten Sie die Antwort 200 OK mit der Auflistung der [user](..\api-reference\v1.0\resources\user.md)-Ressourcen in der Nutzlast. Jeder Benutzer wird anhand der **id**-Eigenschaft und seinen Standardeigenschaften identifiziert. Die nachfolgend dargestellte Arbeitslast ist aus Platzgründen abgeschnitten.

```no-highlight 
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "value":[
    {
      "id":"f71f1f74-bf1f-4e6b-b266-c777ea76e2c7",
      "businessPhones":[

      ],
      "displayName":"CIE Administrator",
      "givenName":"CIE",
      "jobTitle":null,
      "mail":"admin@contoso.onmicrosoft.com",
      "mobilePhone":"+1 3528700812",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Administrator",
      "userPrincipalName":"admin@contoso.onmicrosoft.com"
    },
    {
      "id":"d66f2902-9d12-4ff8-ab01-21ec6706079f",
      "businessPhones":[

      ],
      "displayName":"Alan Steiner",
      "givenName":"Alan",
      "jobTitle":"VP Corporate Marketing",
      "mail":"alans@contoso.onmicrosoft.com",
      "mobilePhone":null,
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Steiner",
      "userPrincipalName":"alans@contoso.onmicrosoft.com"
    }
  ]
}
```

Mit Microsoft Graph können Sie auch Websitesammlungen anzeigen, indem Sie in den Beziehungen von einer Ressource zu einer anderen navigieren. Über die **mailFolders**-Navigationseigenschaft eines Benutzers können Sie beispielsweise die Auflistung von [mailFolder](..\api-reference\v1.0\resources\mailfolder.md)-Ressourcen im Benutzerpostfach abfragen:

```no-highlight 
GET https://graph.microsoft.com/v1.0/me/mailfolders HTTP/1.1
Authorization : Bearer {access_token}
```

Wenn der Vorgang erfolgreich ist, erhalten Sie die Antwort 200 OK mit der Auflistung der [mailFolder](..\api-reference\v1.0\resources\user.md)-Ressourcen in der Nutzlast. Jeder **mailFolder** wird anhand der **id**-Eigenschaft und seinen Eigenschaften identifiziert. Die nachfolgend dargestellte Arbeitslast ist aus Platzgründen abgeschnitten.

```no-highlight 
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('16f5a7b6-5a15-4568-aa5a-31bb117e9967')/mailFolders",
  "value":[
    {
      "id":"AAMkADRm9AABDGisXAAA=",
      "displayName":"Archive",
      "parentFolderId":"AQMkADRmZWj0AAAIBCAAAAA==",
      "childFolderCount":0,
      "unreadItemCount":0,
      "totalItemCount":0
    },
    {
      "id":"AQMkADRm0AAAIBXAAAAA==",
      "displayName":"Sales reports",
      "parentFolderId":"AQMkADRmZWj0AAAIBCAAAAA==",
      "childFolderCount":0,
      "unreadItemCount":0,
      "totalItemCount":0
    },
    {
      "id":"AAMkADRCxI9AAAT6CAIAAA=",
      "displayName":"Conversation History",
      "parentFolderId":"AQMkADRmZWj0AAAIBCAAAAA==",
      "childFolderCount":1,
      "unreadItemCount":0,
      "totalItemCount":0
    }
  ]
}
```




## <a name="view-a-specific-resource-from-a-collection-by-id"></a>Anzeigen einer bestimmten Ressource aus einer Sammlung nach ID

Wir verwenden weiterhin **user** als Beispiel. Zum Anzeigen der Informationen zu einem Benutzer verwenden Sie eine HTTPS GET-Anforderung, um einen bestimmten Benutzer anhand der Benutzer-ID abzurufen. Für eine **user**-Entität können Sie entweder die **id**- oder die **userPrincipalName**-Eigenschaft als Bezeichner verwenden. Im folgenden Anforderungsbeispiel wird der **userPrincipalName**-Wert als Benutzer-ID verwendet. 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com HTTP/1.1
Authorization : Bearer {access_token}
```

Wenn der Vorgang erfolgreich ist, erhalten Sie den Statuscode 200 OK mit der Benutzerressourcendarstellung in der Nutzlast, wie im Folgenden dargestellt.

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 982

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id": "c95e3b3a-c33b-48da-a6e9-eb101e8a4205",
    "city": "Redmond",
    "country": "USA",
    "department": "Help Center",
    "displayName": "John Doe",
    "givenName": "John",
    "userPrincipalName": "john.doe@contoso.onmicrosoft.com",

    ... 
}
```

## <a name="read-specific-properties-of-a-resource"></a>Lesen der spezifischen Eigenschaften einer Ressource
Um nur biographische Daten des Benutzers abzurufen, z. B. die vom Benutzer bereitgestellte Beschreibung im Feld _Über mich_ und seine Qualifikationen, können Sie den [select](query_parameters.md)-Abfrageparameter zu der vorherigen Anforderung hinzufügen, wie im folgenden Beispiel dargestellt. 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com?$select=displayName,aboutMe,skills HTTP/1.1
Authorization : Bearer {access_token}
```

Bei erfolgreicher Antwort wird der Statuscode 200 OK und eine Nutzlast zurückgegeben, wie dargestellt. 

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 169

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "aboutMe": "A cool and nice guy.",
    "displayName": "John Doe",
    "skills": [
        "n-Lingual",
        "public speaking",
        "doodling"
    ]
}
```
Statt aller Eigenschaftensätze für die **user**-Entität werden hier nur die grundlegenden **aboutMe**-, **displayName**- und **skills**-Eigenschaften zurückgegeben.

## <a name="read-specific-properties-of-the-resources-in-a-collection"></a>Lesen der spezifischen Eigenschaften der Ressourcen in einer Sammlung
Zusätzlich zum Lesen spezifischer Eigenschaften einer einzelnen Ressource können Sie auch den ähnlichen Abfrageparameter [$select](query_parameters.md) auf eine Sammlung anwenden, um alle Ressourcen in der Sammlung mit nur den spezifischen Eigenschaften zurückzugeben, die jeweils zurückgegeben werden. Senden Sie zum Abfragen des Namens der Laufwerkelemente vom angemeldeten Benutzer die folgende HTTPS-GET-Anforderung:

```no-highlight 
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name HTTP/1.1
Authorization : Bearer {access_token}
```

Bei einer erfolgreichen Antwort werden der Statuscode 200 OK und eine Nutzlast mit den Namen der freigegebenen Dateien zurückgegeben, wie im folgenden Beispiel dargestellt:

```no-highlight 
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('john.doe%40contoso.onmicrosoft.com')/drive/root/children(name,type)",
  "value": [
    {
      "@odata.etag": "\"{896A8E4D-27BF-424B-A0DA-F073AE6570E2},2\"",
      "name": "Shared with Everyone"
    },
    {
      "@odata.etag": "\"{B39D5D2E-E968-491A-B0EB-D5D0431CB423},1\"",
      "name": "Documents"
    },
    {
      "@odata.etag": "\"{9B51EA38-3EE6-4DC1-96A6-230E325EF054},2\"",
      "name": "newFile.txt"
    }
  ]
}
```

## <a name="traverse-from-one-resource-to-another-via-relationship"></a>Durchqueren von einer Ressource zu einer anderen anhand der Beziehung
Ein Vorgesetzter enthält eine **directReports**-Beziehung zu anderen Benutzern, die diesem unterstellt sind. Zum Abfragen der Liste der direkten Mitarbeiter eines Benutzers können Sie die folgende HTTPS-GET-Anforderung zum Navigieren zum gewünschten Ziel über das Durchlaufen von Beziehungen verwenden. 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com/directReports HTTP/1.1
Authorization : Bearer {access_token}
```

Bei erfolgreicher Antwort wird der Statuscode 200 OK und eine Nutzlast zurückgegeben, wie dargestellt. 

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 152
    
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
    "@odata.type": "#microsoft.graph.user",
    "id": "c37b074d-fe9d-4e68-83ad-b4401d3be174",
    "department": "Sales & Marketing",
    "displayName": "Bonnie Kearney",

    ...
}
```

Ebenso können Sie anhand einer Beziehung zu verwandten Ressourcen navigieren. Die user-messages-Beziehung ermöglicht beispielsweise eine Durchquerung von einem Azure Active Directory-Benutzer zu einer Gruppe von Outlook-E-Mail-Nachrichten. Im nachstehenden Beispiel wird gezeigt, wie dies in einem REST-API-Aufruf funktioniert:


```no-highlight 
GET https://graph.microsoft.com/v1.0/me/messages HTTP/1.1
Authorization : Bearer {access_token}
```

    
Bei erfolgreicher Antwort wird der Statuscode 200 OK und eine Nutzlast zurückgegeben, wie dargestellt. 


```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
odata-version: 4.0
content-length: 147
    
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('john.doe%40contoso.onmicrosoft.com')/Messages",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/messages?$top=1&$skip=1",
  "value": [
    {
      "@odata.etag": "W/\"FwAAABYAAABMR67yw0CmT4x0kVgQUH/3AAJL+Kej\"",
      "id": "<id-value>",
      "createdDateTime": "2015-11-14T00:24:42Z",
      "lastModifiedDateTime": "2015-11-14T00:24:42Z",
      "changeKey": "FwAAABYAAABMR67yw0CmT4x0kVgQUH/3AAJL+Kej",
      "categories": [],
      "receivedDateTime": "2015-11-14T00:24:42Z",
      "sentDateTime": "2015-11-14T00:24:28Z",
      "hasAttachments": false,
      "subject": "Did you see last night's game?",
      "body": {
        "ContentType": "HTML",
        "Content": "<content>"
      },
      "BodyPreview": "it was great!",
      "Importance": "Normal",
            
       ...
    }
  ]
}
```
Sie können alle Beziehungen in einer bestimmten Ressource anzeigen, indem Sie zu den Metadaten wechseln, den EntityType suchen und sich alle NavigationProperties für diesen EntityType ansehen.

## <a name="call-functions"></a>Aufruffunktionen
Microsoft Graph unterstützt auch _Funktionen_ zum Bearbeiten von Ressourcen auf andere Art und Weise als einfache CRUD-Vorgänge (Erstellen, Lesen, Aktualisieren und Löschen). Diese liegen häufig in der Form von HTTPS-POST-Anforderungen vor, um Argumente für die Funktion aufzunehmen. Die folgende HTTPS-POST-Anforderung z. B. ermöglicht es dem angemeldeten Benutzer (`me`), eine E-Mail zu senden.

```no-highlight 
POST https://graph.microsoft.com/v1.0/me/sendMail HTTP/1.1
authorization: bearer {access_token}
content-type: application/json
content-length: 96

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "garthf@a830edad9050849NDA1.onmicrosoft.com"
        }
      }
    ],
    "attachments": [
      {
        "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
        "name": "menu.txt",
        "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
      }
    ]
  },
  "saveToSentItems": "false"
}
```

Sie können alle verfügbaren Funktionen in den Metadaten sehen. Sie werden als Funktionen oder Aktionen angezeigt.

## <a name="use-the-microsoft-graph-sdks"></a>Verwendung der Microsoft Graph-SDKs

Sie bevorzugen die Benutzerfreundlichkeit und die leistungsstarken Funktionen von SDKs? Zwar können Sie Microsoft Graph jederzeit über REST-APIs aufrufen; wir stellen jedoch auch SDKs für viele beliebte Plattformen zur Verfügung. Unter [Codebeispiele und SDKs](https://graph.microsoft.io/en-us/code-samples-and-sdks) können Sie die verfügbaren SDKs erkunden.

## <a name="see-also"></a>Siehe auch

- [Verwenden der Microsoft Graph-API](use_the_api.md)
- [Authentifizierungstoken abrufen](auth_overview.md)