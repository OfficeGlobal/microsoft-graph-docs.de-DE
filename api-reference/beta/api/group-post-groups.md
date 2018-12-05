---
title: Gruppe erstellen
description: 'Verwenden Sie diese API zum Erstellen einer neuen Gruppe gemäß der Angabe im Anforderungstext. Sie können drei Typen von Gruppen erstellen:'
ms.openlocfilehash: a43ce33d71493d01a53a6d357937a10e29810230
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058458"
---
# <a name="create-group"></a>Gruppe erstellen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Verwenden Sie diese API zum Erstellen einer neuen [Gruppe](../resources/group.md) wie im Textkörper Anforderung angegeben. Sie können eine der drei Arten von Gruppen erstellen:

* Office 365-Gruppe (einheitliche Gruppe)
* Dynamische Gruppe
* Sicherheitsgruppe

> **Hinweis**: zum Erstellen ein [Team](../resources/team.md), zuerst erstellen Sie eine Gruppe, dann fügen Sie ein Team hinzu, finden Sie unter [Team erstellen](../api/team-put-teams.md).

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
Die folgende Tabelle zeigt die Eigenschaften des [Group](../resources/group.md) -Ressource angeben, wenn Sie eine Gruppe zu erstellen. 

| Eigenschaft | Typ | Beschreibung|
|:---------------|:--------|:----------|
| displayName | string | Der Name der Gruppe, der im Adressbuch angezeigt wird. Erforderlich. |
| mailEnabled | boolean | **true** für E-Mail-aktivierte Gruppen. Legen Sie dies auf **true** fest, wenn eine Office 365-Gruppe zu erstellen. Festlegen Sie diese Eigenschaft auf **"false"** Wenn dynamische Erstellen oder Sicherheitsgruppe. Erforderlich. |
| mailNickname | string | Der E-Mail-Alias für die Gruppe. Erforderlich. |
| securityEnabled | boolean | Festgelegt auf **true** für Sicherheit-aktivierte Gruppen. Legen Sie dies auf **true** fest, wenn eine dynamische oder eine Sicherheitsgruppe an erstellen. Legen Sie dies auf **false fest** , wenn eine Office 365-Gruppe zu erstellen. Erforderlich. |
| owners | string collection | Diese Eigenschaft stellt den Besitzer für die Gruppe zum Zeitpunkt der Erstellung. Optional. |
| Elemente | string collection | Diese Eigenschaft stellt die Mitglieder der Gruppe zum Zeitpunkt der Erstellung. Optional. |

Geben Sie die **groupTypes** Eigenschaft an, wenn Sie eine Office 365 oder eine dynamische Gruppe erstellen, wie unten beschrieben.

| Art der Gruppe | **groupTypes**-Eigenschaft |
|:--------------|:------------------------|
| Office 365 (auch einheitliche Gruppe genannt)| „Unified“ |
| Dynamisch | "DynamicMembership" |
| Sicherheit | Nicht festlegen. |

Da die **Group** -Ressource [Extensions](/graph/extensibility-overview)unterstützt, können Sie die `POST` Vorgang und benutzerdefinierte Eigenschaften mit Ihren eigenen Daten beim Erstellen der Gruppe hinzufügen.

>**Hinweis:** Erstellen einer Office 365-Gruppe programmgesteuert ohne einen Benutzerkontext und ohne Angabe von Besitzer erstellt die Gruppe anonym.  Dies kann führen, dass in der zugehörigen SharePoint Online-Website nicht automatisch erstellt werden, bis eine zusätzliche manuelle Aktion ausgeführt wird.  

Geben Sie bei Bedarf andere beschreibbare Eigenschaften für Ihre Gruppe an. Weitere Informationen finden Sie in Themen zu Eigenschaften der [group](../resources/group.md)-Ressource.

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [group](../resources/group.md)-Objekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel
#### <a name="request-1"></a>Anforderung 1
Die erste beispielanforderung erstellt eine Office 365-Gruppe.
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups
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

#### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort.
>**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.
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
Die zweite beispielanforderung erstellt eine Office 365-Gruppe mit Besitzer angegeben.
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