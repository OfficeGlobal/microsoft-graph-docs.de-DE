---
title: Directory-Objekte aus einer Liste von IDs abrufen
description: Die select`-Abfrageoption ist für diesen Vorgang nicht verfügbar.
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a209d391c72edd453bbfe9232b7d02121ca98128
ms.sourcegitcommit: 7412dd2f2d5ed66afa2b0759c861ad23b4c6ecdf
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/23/2019
ms.locfileid: "30212389"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a>Directory-Objekte aus einer Liste von IDs abrufen

Gibt die in einer Liste von IDs angegebenen Directory-Objekte zurück.  HINWEIS: Die zurückgegebenen Directory-Objekte sind die vollständigen Objekte mit **allen** Eigenschaften. Die Abfrageoption `$select` ist für diesen Vorgang nicht verfügbar.

Nachfolgend sind einige gängige Verwendungsmöglichkeiten für diese Funktion aufgeführt:

* Auflösen von IDs, die von Funktionen zurückgegeben werden (die Sammlungen von IDs zurückgeben), z. B. [getMemberObjects](directoryobject-getmemberobjects.md) oder [getMemberGroups](directoryobject-getmembergroups.md) in ihre zugrunde liegenden Directory-Objekte.
* Auflösen von durch die Anwendung permanent in einem externen Speicher gespeicherten IDs in ihre zugrunde liegenden Verzeichnisobjekte

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).


|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Directory.Read.All, Directory.AccessAsUser.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Directory.Read.All |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a>Anforderungsheader

| Name       | Typ | Beschreibung|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |
| Content-Type  | string | application/json  |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.

| Parameter   | Typ |Beschreibung|
|:---------------|:--------|:----------|
|ids|String collection| Eine Sammlung von IDs, für die Objekte zurückgegeben werden sollen. Sie können bis zu 1000 IDs angeben. |
|types|String-Sammlung| Eine Sammlung von Ressourcentypen, die den Satz von zu durchsuchenden Ressourcensammlungen angibt. Wenn keine Angabe erfolgt, wird [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) als Standardwert verwendet; dieser enthält alle im Verzeichnis definierten Ressourcentypen. Jedes Objekt, das von [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) abgeleitet wird, kann in der Sammlung angegeben werden; Beispiel: [user](/graph/api/resources/user?view=graph-rest-v1.0), [group](/graph/api/resources/group?view=graph-rest-v1.0), [device](/graph/api/resources/device?view=graph-rest-v1.0) usw. Um nach Referenzen für ein [Cloud Solution Provider](https://partner.microsoft.com/de-DE/cloud-solution-provider)-Partnerunternehmen zu suchen, geben Sie [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0) an. Wenn keine Angabe erfolgt, wird [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) als Standardwert verwendet; dieser enthält alle im Verzeichnis definierten Ressourcentypen, außer bei Referenzen für ein [Cloud Solution Provider](https://partner.microsoft.com/de-DE/cloud-solution-provider)-Partnerunternehmen. Bei den Werten wird nicht zwischen Groß- und Kleinschreibung unterschieden.|

## <a name="response"></a>Reaktion

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "directoryobject_getById"
}-->

```http
POST https://graph.microsoft.com/v1.0/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893874940a3-97b7-68513b600544","5d6059b6368d-45f8-91e18e07d485f1d0"],
    "types":["user"]
}
```

##### <a name="response"></a>Antwort

Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
    "value": [
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Trevor Jones"
      },
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Billy Smith"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
