---
title: SynchronizationJob löschen
description: Beenden Sie den Synchronisierungsauftrag und löschen Sie den zugeordneten Zustand endgültig. Synchronisierte Konten werden als Links-ist.
localization_priority: Normal
ms.openlocfilehash: 29083413c5b24a5ed07b671adfa048f58d437f0d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521684"
---
# <a name="delete-synchronizationjob"></a>SynchronizationJob löschen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Beenden Sie den Synchronisierungsauftrag und löschen Sie den zugeordneten Zustand endgültig. Synchronisierte Konten werden als Links-ist.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)     |Directory.ReadWrite.All  |
|Delegiert (persönliches Microsoft-Konto) |Nicht unterstützt  |
|Anwendung                            |Nicht unterstützt | 

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a>Anforderungsheader

| Name           | Typ    | Beschreibung|
|:---------------|:--------|:-----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext

Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Bei erfolgreicher gibt eine `204 No Content` Antwort. Es gibt keine Suchzeichenfolge im Antworttext zurück.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung
Es folgt ein Beispiel für eine Anforderung.
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
