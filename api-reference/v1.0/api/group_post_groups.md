# <a name="create-group"></a>Gruppe erstellen
Verwenden Sie diese API zum Erstellen einer neuen Gruppe gemäß der Angabe im Anforderungstext. Sie können drei Typen von Gruppen erstellen:

* Office 365-Gruppe (einheitliche Gruppe)
* Dynamische Gruppe
* Sicherheitsgruppe

> **Hinweis**: Microsoft Teams basiert zwar auf Office 365-Gruppen, über diese API kann derzeit aber kein Team erstellt werden. Sie können die anderen Gruppen-APIs verwenden, um ein Team zu verwalten, das in der Microsoft Teams-Benutzeroberfläche erstellt wurde.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Group.ReadWrite.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Group.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:---------------|:--------|:----------|
| Autorisierung  | Zeichenfolge  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Die folgende Tabelle zeigt die Eigenschaften der [Gruppen](../resources/group.md)-Ressource, die Sie angeben müssen, wenn Sie eine Gruppe erstellen. 

| Eigenschaft | Typ | Beschreibung|
|:---------------|:--------|:----------|
| displayName | Zeichenfolge | Der Name der Gruppe, der im Adressbuch angezeigt wird. Erforderlich. |
| mailEnabled | boolesch | **true** für E-Mail-aktivierte Gruppen. Legen Sie dies auf **true** fest, wenn Sie eine Office 365-Gruppe erstellen. Legen Sie dies auf **false** fest, wenn Sie eine dynamische oder eine Sicherheitsgruppe erstellen. Erforderlich. |
| mailNickname | Zeichenfolge | Der E-Mail-Alias für die Gruppe. Erforderlich. |
| securityEnabled | boolesch | Legen Sie dies für Sicherheits-aktivierte Gruppen auf **true** fest. Legen Sie dies auf **true** fest, wenn Sie eine dynamische oder eine Sicherheitsgruppe erstellen. Legen Sie dies auf **false** fest, wenn Sie eine Office 365-Gruppe erstellen. Erforderlich. |
| Besitzer | Zeichenfolgen-Sammlung | Diese Eigenschaft stellt die Besitzer für die Gruppe zum Zeitpunkt der Erstellung dar. Optional. |
| Elemente | Zeichenfolgen-Sammlung | Diese Eigenschaft stellt die Mitglieder der Gruppe zum Zeitpunkt der Erstellung. Optional. |


Geben Sie die **groupTypes** Eigenschaft an, wenn Sie eine Office 365 oder eine dynamische Gruppe erstellen, wie unten beschrieben.

### <a name="grouptypes-options"></a>GroupTypes-Optionen

| Art der Gruppe | **groupTypes**-Eigenschaft |
|:--------------|:------------------------|
| Office 365 (auch einheitliche Gruppe genannt)| „Unified“ |
| Dynamisch | "DynamicMembership" |
| Sicherheit | Nicht festlegen. |


>**Hinweis:** Das programmgesteuerte Erstellen einer Office 365-Gruppe ohne einen Benutzerkontext und ohne Angabe von Besitzer erstellt die Gruppe anonym.  Dies kann dazu führen, dass die zugehörige SharePoint Online-Website nicht automatisch erstellt wird, bis eine zusätzliche manuelle Aktion ausgeführt wird.  

Geben Sie bei Bedarf andere beschreibbare Eigenschaften für Ihre Gruppe an. Weitere Informationen finden Sie in Themen zu Eigenschaften der [group](../resources/group.md)-Ressource.

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [group](../resources/group.md)-Objekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel
#### <a name="request-1"></a>Anforderung 1
Die erste Beispielanforderung erstellt eine Office 365-Gruppe.
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

#### <a name="response-1"></a>Antwort 1
Nachfolgend sehen Sie ein Beispiel der Antwort.
>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mail": "library@contoso.onmicrosoft.com",
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

#### <a name="request-2"></a>Anforderung 2
Die zweite Beispielanforderung erstellt eine Office 365-Gruppe mit angegebenem Besitzer.
<!-- {
  "blockType": "request"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-Type: application/json

{
  "description": "Group with owners",
  "displayName": "Group1",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "group1",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ]
}
```

#### <a name="response-2"></a>Antwort 2
Es folgt ein Beispiel für die erfolgreiche Antwort.
>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "description": "Group with owners",
    "displayName": "Group1",
    "groupTypes": [
        "Unified"
    ],
    "mail": "group1@contoso.onmicrosoft.com",
    "mailEnabled": true,
    "mailNickname": "group1",
    "securityEnabled": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
