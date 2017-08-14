# <a name="create-group"></a>Gruppe erstellen

Verwenden Sie diese API zum Erstellen einer neuen Gruppe gemäß der Angabe im Anforderungstext. Sie können drei Typen von Gruppen erstellen:

* Office 365-Gruppe (einheitliche Gruppe)
* Dynamische Gruppe
* Sicherheitsgruppe

> **Hinweis**: Microsoft Teams basiert zwar auf Office 365-Gruppen, über diese API kann derzeit aber kein Team erstellt werden. Sie können die anderen Gruppen-APIs verwenden, um ein Team zu verwalten, das in der Microsoft Teams-Benutzeroberfläche erstellt wurde.

## <a name="prerequisites"></a>Voraussetzungen
Der folgende **Bereich** ist erforderlich, um diese API auszuführen: _Group.ReadWrite.All_ 
## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Die folgende Tabelle zeigt die Eigenschaften der [Gruppe](../resources/group.md) Ressource, die Sie zumindest angeben müssen, wenn Sie eine Gruppe erstellen. 

| Eigenschaft | Typ | Beschreibung|
|:---------------|:--------|:----------|
| displayName | string | Der Name der Gruppe, der im Adressbuch angezeigt wird. |
| mailEnabled | Boolescher Wert | **true** für E-Mail-aktivierte Gruppen. **true**, wenn eine Office 365-Gruppe erstellt wird. **false**, wenn dynamische oder Sicherheitsgruppe erstellt wird.|
| mailNickname | string | Der E-Mail-Alias für die Gruppe. |
| securityEnabled | Boolescher Wert | **true** für Gruppen mit aktivierter Sicherheit. **true**, wenn dynamische oder eine Sicherheitsgruppe erstellt wird. **false**, wenn eine Office 365-Gruppe erstellt wird. |

Geben Sie die **groupTypes** Eigenschaft an, wenn Sie eine Office 365 oder eine dynamische Gruppe erstellen, wie unten beschrieben.

| Art der Gruppe | **groupTypes**-Eigenschaft |
|:--------------|:------------------------|
| Office 365 (auch einheitliche Gruppe genannt)| „Unified“ | 
| Dynamisch | "DynamicMembership" | 
| Sicherheit | Nicht festlegen. | 

Geben Sie bei Bedarf andere beschreibbare Eigenschaften für Ihre Gruppe an. Weitere Informationen finden Sie in Themen zu Eigenschaften der [group](../resources/group.md)-Ressource.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und das [group](../resources/group.md)-Objekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Hier ist ein Beispiel für eine Anforderung, die eine Office 365-Gruppe erstellt.
<!-- {
  "blockType": "request",
  "name": "create_group_from_groups"
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

##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden mehr Eigenschaften zurückgegeben.
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
