---
title: 'group: checkMemberGroups'
description: Überprüfen Sie die Mitgliedschaft in der angegebenen Liste von Gruppen. Diese Gruppen, denen zurückgegeben aus der Liste
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 838ea805f6732965029690a05e8d3294fdd62c26
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514901"
---
# <a name="group-checkmembergroups"></a>group: checkMemberGroups

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Sucht nach einer Mitgliedschaft in der angegebenen Liste von Gruppen. Gibt aus der Liste diejenigen Gruppen zurück, bei denen die angegebene Gruppe über eine direkte oder transitive Mitgliedschaft verfügt.

Sie können maximal 20 Gruppen pro Anforderung überprüfen. Diese Funktion unterstützt Office 365 und andere Typen von Gruppen, die in Azure AD bereitgestellt werden. Beachten Sie, dass Office 365-Gruppen keine Gruppen enthalten kann. Die Mitgliedschaft in einer Office 365-Gruppe ist also immer direkt.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| Delegiert (Geschäfts-, Schul- oder Unikonto)     | ~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All |
| Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt                                                                              |
| Anwendung                            | ~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All                             |

> **Hinweis:** Diese API erfordert derzeit mindestens die Berechtigung `Directory.Read.All`. Mithilfe der `Group.Read.All` Berechtigung gibt einen Fehler zurück. Dies ist ein bekanntes Problem.

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a>Anforderungsheader

| Name          | Typ   | Beschreibung               |
| :------------ | :----- | :------------------------ |
| Authorization | string | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.

| Parameter | Typ   | Beschreibung           |
| :-------- | :----- | :-------------------- |
| groupIds  | String | Ein Array von Gruppen-IDs |

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel

Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.

##### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.

<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-checkmembergroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
