---
title: SynchronizationJob starten
description: Starten Sie eine vorhandene Synchronisierungsauftrag. Wenn der Auftrag angehalten ist, wird Verarbeitung Änderungen an der Stelle fortgesetzt, in dem er angehalten wurde. Wenn der Auftrag in Quarantäne befindet, wird der Quarantänestatus gelöscht.
localization_priority: Normal
ms.openlocfilehash: 4648d9d3d889adf2cd7ec06e4fcf79b761c77132
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515370"
---
# <a name="start-synchronizationjob"></a>SynchronizationJob starten

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Starten Sie eine vorhandene Synchronisierungsauftrag. Wenn der Auftrag angehalten ist, wird Verarbeitung Änderungen an der Stelle fortgesetzt, in dem er angehalten wurde. Wenn der Auftrag in Quarantäne befindet, wird der Quarantänestatus gelöscht.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)     |Directory.ReadWrite.All  |
|Delegiert (persönliches Microsoft-Konto) |Nicht unterstützt |
|Anwendung                            |Nicht unterstützt | 

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
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
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

##### <a name="response"></a>Antwort
Es folgt ein Beispiel für eine Antwort.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob: start",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-start.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
