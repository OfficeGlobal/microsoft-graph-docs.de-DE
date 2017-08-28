# <a name="update-open-extension"></a>Datenerweiterung aktualisieren

Aktualisieren Sie eine offene Erweiterung ([openTypeExtension](../resources/openTypeExtension.md)-Objekt) mit den Eigenschaften im Anforderungsheader:

- Wenn eine Eigenschaft im Anforderungsheader mit dem Name einer vorhandenen Eigenschaft in der Erweiterung übereinstimmt, werden die Daten in die Erweiterung aktualisiert.
- Andernfalls werden die Eigenschaft und die entsprechenden Daten zur Erweiterung hinzugefügt. 

Die Daten in einer Erweiterung können Grundtypen oder Arrays von Grundtypen sein.

## <a name="permissions"></a>Berechtigungen

Zum Aufrufen dieser API ist eine der folgenden Berechtigungen erforderlich (je nach dem Typ der Ressource, in der die Erweiterung erstellt wurde): Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|**Unterstützte Ressource**|**Berechtigung**|**Unterstützte Ressource**|**Berechtigung** |
|:-----|:-----|:-----|:-----|
| [device](../resources/device.md) | Device.ReadWrite.All | [event](../resources/event.md) | Calendars.ReadWrite |
| [group](../resources/group.md) | Group.ReadWrite.All | [group event](../resources/event.md) | Group.ReadWrite.All |
| [group post](../resources/post.md) | Group.ReadWrite.All | [message](../resources/message.md) | Mail.ReadWrite |
| [organization](../resources/organization.md) | Directory.AccessAsUser.All | [personal contact](../resources/contact.md) | Contacts.ReadWrite |
| [user](../resources/user.md) | Directory.AccessAsUser.All | | |

## <a name="http-request"></a>HTTP-Anforderung
In der Anforderung geben Sie die Ressourceninstanz an, spezifizieren in der Navigationseigenschaft **extensions** dieser Instanz die Erweiterung und wenden anschließend den Befehl `PATCH` auf diese Erweiterungsinstanz an.

<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{Id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
PATCH /groups/{id}/extensions/{extensionId}
PATCH /groups/{id}/events/{id}/extensions/{extensionId}
PATCH /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
PATCH /organization/{Id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/extensions/{extensionId}
```

>**Hinweis:** Die obige Syntax zeigt mehrere häufig verwendete Möglichkeiten zum Identifizieren einer Ressourceninstanz, um eine Erweiterung darin zu aktualisieren. Alle anderen Syntaxen, mit denen Sie diese Ressourceninstanzen identifizieren können, unterstützen das Aktualisieren offener Erweiterungen darin in einer ähnlichen Weise.

Im Abschnitt [Anforderungstext](#request-body) wird beschrieben, wie Sie benutzerdefinierte Daten zur Änderung oder Ergänzung der Erweiterung in den Anforderungstext einschließen können.


## <a name="parameters"></a>Parameter
|**Parameter**|**Typ**|**Beschreibung**|
|:-----|:-----|:-----|
|_URL parameters_|
|id|string|Ein eindeutiger Bezeichner für eine Instanz der entsprechenden Sammlung. Erforderlich. |
|extensionId|string|Dies kann ein Erweiterungsname sein. Der Erweiterungsname ist ein eindeutiger Textbezeichner einer Erweiterung oder ein vollqualifizierter Name, der den Erweiterungstyp und den eindeutigen Textbezeichner verkettet. Der vollqualifizierte Name wird beim Erstellen der Erweiterung in der `id`-Eigenschaft zurückgegeben. Erforderlich. |

## <a name="request-headers"></a>Anforderungsheader
| Name       | Wert |
|:---------------|:----------|
| Authorization | Bearer {token}. Erforderlich. |
| Content-Type | application/json |

## <a name="request-body"></a>Anforderungstext

Stellen Sie den JSON-Text eines [openTypeExtension](../resources/openTypeExtension.md)-Objekts mit den folgenden erforderlichen Name-Wert-Paaren und allen benutzerdefinierten Daten bereit, die geändert oder zu dieser Erweiterung hinzugefügt werden sollen. Die Daten in der JSON-Nutzlast können Grundtypen oder Arrays von Grundtypen sein.

| Name       | Wert |
|:---------------|:----------|
| @odata.type | Microsoft.Graph.OpenTypeExtension |
| extensionName | %unique_string% |

## <a name="response"></a>Antwort

Bei Erfolg gibt diese Methode den Antwortcode `200 OK` und das aktualisierte [openTypeExtension](../resources/openTypeExtension.md)-Objekt zurück.


## <a name="example"></a>Beispiel
#### <a name="request-1"></a>Anforderung 1

Im ersten Beispiel wird gezeigt, wie eine Erweiterung in einer Nachricht aktualisiert wird. Die Erweiterung wird anfänglich durch die folgende JSON-Nutzlast dargestellt:

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00Z"
}
```

Sie können anhand des Namens auf die Erweiterung verweisen:

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

Sie können auch anhand des vollqualifizierten Namens auf die Erweiterung verweisen:

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```

Sie können die Beispielanforderung und den folgenden Anforderungstext verwenden, um die oben genannte Erweiterung auf folgende Weise zu aktualisieren:
- Durch Ändern des `companyName` von `Wingtip Toys` zu `Wingtip Toys (USA)`
- Durch Ändern des `dealValue` von `500050` zu `500100`
- Durch Hinzufügen neuer Daten als die benutzerdefinierte `updated`-Eigenschaft

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.type": "Microsoft.Graph.OpenTypeExtension",
    "extensionName": "Com.Contoso.Referral",
    "companyName": "Wingtip Toys (USA)",
    "dealValue": "500100",
    "expirationDate": "2015-12-03T10:00:00.000Z",
    "updated": "2015-10-29T11:00:00.000Z"
} 
```


#### <a name="response-1"></a>Antwort 1

Es wird unabhängig von der zur Referenzierung der Erweiterung verwendeten Methode jeweils die gleiche Antwort zurückgegeben.

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "extensionName": "Com.Contoso.Referral",
    "companyName": "Wingtip Toys (USA)",
    "dealValue": 500100,
    "expirationDate": "2015-12-03T10:00:00Z",
    "updated": "2015-10-29T11:00:00.000Z"
}
```

****

#### <a name="request-2"></a>Anforderung 2

Im zweiten Beispiel wird gezeigt, wie eine Erweiterung in einem Gruppenbeitrag aktualisiert wird. Die Erweiterung wird anfänglich durch die folgende JSON-Nutzlast mit einem `expirationDate`-Wert von `2015-07-03T13:04:00Z` dargestellt:

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2015-07-03T13:04:00Z",
    "DealValue": 1010100,
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```

Im Folgenden werden die Anforderung und Anforderungstext zum Ändern von `expirationDate` zu `2016-07-30T11:00:00Z` dargestellt:

<!-- {
  "blockType": "request",
  "name": "update_opentypeextension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA==')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate')
Content-type: application/json

{
   "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
   "extensionName": "Com.Contoso.Estimate",
   "companyName": "Contoso",
   "expirationDate": "2016-07-30T11:00:00.000Z",
   "DealValue": 1010100,
   "topPicks": [
       "Employees only",
       "Add spouse or guest",
       "Add family"
    ]
}
```

#### <a name="response-2"></a>Antwort 2

Im Folgenden wird die Antwort des zweiten Beispiels dargestellt, welche das aktualisierte `expirationDate`-Element in die Erweiterung zeigt.

<!-- {  
  "blockType": "response",  
  "truncated": true,  
  "@odata.type": "microsoft.graph.opentypeextension"  
} --> 
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2016-07-30T11:00:00Z",
    "DealValue": 1010100,
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
} -->
