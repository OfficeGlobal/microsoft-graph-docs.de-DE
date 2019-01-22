---
title: Gruppe erstellen
description: 'Verwenden Sie diese API zum Erstellen einer neuen Gruppe gemäß der Angabe im Anforderungstext. Sie können drei Typen von Gruppen erstellen:'
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: de304cc4faaa6e4b64992ba0d7b2af35e8b5900a
ms.sourcegitcommit: 7d94b581f7c6dc1995efecf6ee21b604c0b80998
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/19/2019
ms.locfileid: "29353069"
---
# <a name="create-group"></a>Gruppe erstellen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Verwenden Sie diese API zum Erstellen einer neuen [Gruppe](../resources/group.md) gemäß der Angabe im Anforderungstext. Sie können drei Typen von Gruppen erstellen:

* Office 365-Gruppe (einheitliche Gruppe)
* Dynamische Gruppe
* Sicherheitsgruppe

Dieser Vorgang gibt standardmäßig nur eine Teilmenge der Eigenschaften für jede Gruppe zurück. Diese Standardeigenschaften werden im Abschnitt [Eigenschaften](../resources/group.md#properties) aufgeführt.

Um Eigenschaften abzurufen, die _nicht_ standardmäßig zurückgegeben werden, führen Sie eine GET-Operation aus, und geben Sie die Eigenschaften in einer OData-Abfrageoption `$select` an. Sehen Sie sich das [Beispiel](group-get.md#request-2) an.

> **Hinweis**: Zum Erstellen eines [Teams](../resources/team.md) erstellen Sie zuerst eine Gruppe und fügen ihr dann ein Team hinzu (siehe [Team erstellen](../api/team-put-teams.md)).

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

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
| Authorization  | string  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Die folgende Tabelle enthält die Eigenschaften der [group](../resources/group.md)-Ressource, die Sie beim Erstellen einer Gruppe angeben müssen. 

| Eigenschaft | Typ | Beschreibung|
|:---------------|:--------|:----------|
| displayName | string | Der Name der Gruppe, der im Adressbuch angezeigt wird. Erforderlich. |
| mailEnabled | boolean | **true** für E-Mail-aktivierte Gruppen. **true**, wenn eine Office 365-Gruppe erstellt wird. **false**, wenn eine dynamische oder eine Sicherheitsgruppe erstellt wird. Erforderlich. |
| mailNickname | string | Der E-Mail-Alias für die Gruppe. Erforderlich. |
| securityEnabled | Boolescher Wert | **true** für Gruppen mit aktivierter Sicherheit. **true**, wenn eine dynamische oder eine Sicherheitsgruppe erstellt wird. **false**, wenn eine Office 365-Gruppe erstellt wird. Erforderlich. |
| owners | Zeichenfolgenauflistung | Diese Eigenschaft stellt die Besitzer für die Gruppe zum Zeitpunkt der Erstellung dar. Optional. |
| members | Zeichenfolgenauflistung | Diese Eigenschaft stellt die Mitglieder der Gruppe zum Zeitpunkt der Erstellung dar. Optional. |

Geben Sie die **groupTypes**-Eigenschaft an, wenn Sie eine Office 365- oder eine dynamische Gruppe erstellen, wie unten beschrieben.

| Art der Gruppe | **groupTypes**-Eigenschaft |
|:--------------|:------------------------|
| Office 365 (auch einheitliche Gruppe genannt)| „Unified“ |
| Dynamisch | "DynamicMembership" |
| Sicherheit | Nicht festlegen. |

Da die **group**-Ressource [Erweiterungen](/graph/extensibility-overview) unterstützt, können Sie den `POST`-Vorgang verwenden und beim Erstellen der Gruppe benutzerdefinierte Eigenschaften mit Ihren eigenen Daten hinzufügen.

>**Hinweis:** Beim programmgesteuerten Erstellen einer Office 365-Gruppe ohne Benutzerkontext und ohne Angabe von Besitzern wird die Gruppe anonym erstellt.  Dies kann dazu führen, dass die zugehörige SharePoint Online-Website nicht automatisch erstellt wird und weitere manuelle Aktionen nötig sind.  

Geben Sie bei Bedarf andere beschreibbare Eigenschaften für Ihre Gruppe an. Weitere Informationen finden Sie in Themen zu Eigenschaften der [group](../resources/group.md)-Ressource.

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [group](../resources/group.md)-Objekt im Antworttext zurückgegeben. Die Antwort enthält nur die Standardeigenschaften der Gruppe.

## <a name="example"></a>Beispiel
#### <a name="request-1"></a>Anforderung 1
Die erste Beispielanfrage erstellt eine Office 365-Gruppe.
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for golf",
  "displayName": "Golf Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "golfassist",
  "securityEnabled": false
}
```

#### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort.
>**Hinweis:**  Das hier gezeigte Antwortobjekt ist möglicherweise zur besseren Lesbarkeit gekürzt worden. Von einem tatsächlichen Aufruf werden alle Standardeigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
     "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
     "deletedDateTime": null,
     "classification": null,
     "createdDateTime": "2018-12-22T02:21:05Z",
     "description": "Self help community for golf",
     "displayName": "Golf Assist",
     "expirationDateTime": null,
     "groupTypes": [
         "Unified"
     ],
     "mail": "golfassist@contoso.com",
     "mailEnabled": true,
     "mailNickname": "golfassist",
     "membershipRule": null,
     "membershipRuleProcessingState": null,
     "onPremisesLastSyncDateTime": null,
     "onPremisesSecurityIdentifier": null,
     "onPremisesSyncEnabled": null,
     "preferredDataLocation": "CAN",
     "preferredLanguage": null,
     "proxyAddresses": [
         "SMTP:golfassist@contoso.onmicrosoft.com"
     ],
     "renewedDateTime": "2018-12-22T02:21:05Z",
     "resourceBehaviorOptions": [],
     "resourceProvisioningOptions": [],
     "securityEnabled": false,
     "theme": null,
     "visibility": "Public",
     "onPremisesProvisioningErrors": []
}
```

#### <a name="request-2"></a>Anforderung 2
Die zweite Beispielanfrage erstellt eine Office 365-Gruppe mit einem angegebenen Besitzer.
<!-- {
  "blockType": "request",
  "name": "create_group_with_owner"
}-->
```http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
  "description": "Group with designated owner",
  "displayName": "Operations group",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "operations2019",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ]
}
```

 #### <a name="response-2"></a>Antwort 2
Es folgt ein Beispiel für eine erfolgreiche Antwort. Es enthält nur Standardeigenschaften. Sie können anschließend die **owners**-Navigationseigenschaft der Gruppe abrufen, um die Details des Besitzers zu überprüfen. 
>**Hinweis:**  Das hier gezeigte Antwortobjekt ist möglicherweise zur besseren Lesbarkeit gekürzt worden. Von einem tatsächlichen Aufruf werden alle Standardeigenschaften zurückgegeben.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group_with_owner"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
     "id": "502df398-d59c-469d-944f-34a50e60db3f",
     "deletedDateTime": null,
     "classification": null,
     "createdDateTime": "2018-12-27T22:17:07Z",
     "description": "Group with designated owner",
     "displayName": "Operations group",
     "expirationDateTime": null,
     "groupTypes": [
         "Unified"
     ],
     "mail": "operations2019@contoso.com",
     "mailEnabled": true,
     "mailNickname": "operations2019",
     "membershipRule": null,
     "membershipRuleProcessingState": null,
     "onPremisesLastSyncDateTime": null,
     "onPremisesSecurityIdentifier": null,
     "onPremisesSyncEnabled": null,
     "preferredDataLocation": "CAN",
     "preferredLanguage": null,
     "proxyAddresses": [
         "SMTP:operations2019@contoso.com"
     ],
     "renewedDateTime": "2018-12-27T22:17:07Z",
     "resourceBehaviorOptions": [],
     "resourceProvisioningOptions": [],
     "securityEnabled": false,
     "theme": null,
     "visibility": "Public",
     "onPremisesProvisioningErrors": []
}
```

## <a name="see-also"></a>Siehe auch

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](/graph/extensibility-overview)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)](/graph/extensibility-open-users)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
