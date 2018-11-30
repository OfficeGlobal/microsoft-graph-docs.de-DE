---
title: Berechtigungen
description: 'Ruft eine Liste der kürzlich gelöschter Objekte Besitz des angegebenen Benutzers.  '
ms.openlocfilehash: affdd67d48056c4459e651fd5c64168d8356abe8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016578"
---
# <a name="list-deleted-items-owned-by-a-user"></a>**Gelöschte Listenelemente Besitz eines Benutzers**

Ruft eine Liste der kürzlich gelöschter Objekte Besitz des angegebenen Benutzers.  

Liste gelöschter Elemente Funktionalität ist derzeit nur für Ressourcen der [Gruppe](../resources/group.md) Besitz des Benutzers unterstützt.

Dies ist eine Service-Aktion, was bedeutet, dass es keine Paginierung unterstützt.  Die API gibt bis zu 1.000 Gelöschte Objekte Besitz des Benutzers, sortiert nach ID zurück.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).

| Berechtigungstyp | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten) |
| --- | --- |
| Delegiert (Geschäfts-, Schul- oder Unikonto) | Group.Read.All, Group.ReadWrite.All |
| Delegiert (persönliches Microsoft-Konto) |  Nicht unterstützt |
| Anwendung | Group.Read.All, Group.ReadWrite.All  |

## <a name="http-request"></a>HTTP-Anforderung

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a>Anforderungsheader

| Name          | Beschreibung               |
| ------------- | ------------------------- |
| Authorization | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext

```json
{
  "userId":"{id}",
  "type":"Group"
}
```

Textkörper der Anforderung erfordert die folgenden Parameter:

| Parameter    | Typ |Beschreibung|
|:---------------|:--------|:----------|
|userId|String|ID des Besitzers.|
|Typ|String|Art der Objekte zurückgegeben. `Group` ist derzeit der einzige unterstützte Wert.|


## <a name="response"></a>Antwort

Zurückgeben der erfolgreiche Anforderungen `200 OK` Antwortcodes; Response-Objekt enthält die Eigenschaften des [Verzeichnisses (Gelöschte Objekte)](../resources/directory.md) .

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.

``` http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/getUserOwnedObjects
Content-type: application/json
```

``` json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

###### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Dieses Antwortobjekt der Kürze halber werden möglicherweise abgeschnitten. Alle unterstützte Eigenschaften werden von tatsächlichen Anrufe zurückgegeben.

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": 2018-04-01T12:39:16Z,
              "classification": null,
              "createdDateTime": "2017-03-22T12:39:16Z",
              "description": null,
              "displayName": "Test",
              "groupTypes": [
                  "Unified"
              ],
              "mail": "Test@contoso.com",
              "mailEnabled": true,
              "mailNickname": "Test",
              "membershipRule": null,
              "membershipRuleProcessingState": null,
              "preferredDataLocation": null,
              "preferredLanguage": null,
              "proxyAddresses": [
                  "SMTP:Test@contoso.com"
              ],
              "renewedDateTime": "2017-09-22T22:30:39Z",
              "securityEnabled": false,
              "theme": null,
              "visibility": "Public"
          } 
        ]
 }
```


