---
title: Erstellen von synchronizationJob
description: Erstellen Sie neue Synchronisierungsauftrag mit ein Standardschema für die Synchronisierung aus. Der Auftrag wird in deaktiviertem Zustand erstellt. Rufen Sie Start Auftrag zur Synchronisierung starten.
localization_priority: Normal
ms.openlocfilehash: f41ebe87d8ca935a355c37ea53d1c7bd62b1652e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507915"
---
# <a name="create-synchronizationjob"></a>Erstellen von synchronizationJob

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Erstellen Sie neue Synchronisierungsauftrag mit ein Standardschema für die Synchronisierung aus. Der Auftrag wird in deaktiviertem Zustand erstellt. Rufen Sie [Auftrag starten](synchronization-synchronizationjob-start.md) , um die Synchronisierung starten.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)     |Directory.ReadWrite.All  |
|Delegiert (persönliches Microsoft-Konto) |Nicht unterstützt|
|Anwendung                            |Nicht unterstützt  | 

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a>Anforderungsheader

| Name           | Typ    | Beschreibung|
|:---------------|:--------|:-----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [SynchronizationJob](../resources/synchronization-synchronizationjob.md) -Objekts erstellt werden soll. Ist die einzige erforderliche Eigenschaft `templateId`. Die `templateId` Eigenschaft muss eine der Vorlagen erstellt für diese Anwendung/Dienstprinzipal übereinstimmen. Verwenden Sie verfügbare Vorlagen, um [Listenvorlagen](synchronization-synchronizationtemplate-list.md).

## <a name="response"></a>Antwort

Bei erfolgreicher gibt eine `201 Created` Antwortcode und eines [SynchronizationJob](../resources/synchronization-synchronizationjob.md) -Objekts in der Antworttext.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung
Es folgt ein Beispiel für eine Anforderung.
<!-- {
  "blockType": "request",
  "name": "create_synchronizationjob_from_synchronization"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
Content-type: application/json

{ 
    "templateId": "BoxOutDelta"
}
```

##### <a name="response"></a>Antwort
Es folgt ein Beispiel für eine Antwort. 

>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "{jobId}",
    "templateId": "BoxOutDelta",
    "schedule": {
        "expiration": null,
        "interval": "P10675199DT2H48M5.4775807S",
        "state": "Disabled"
    },
    "status": {
        "countSuccessiveCompleteFailures": 0,
        "escrowsPruned": false,
        "synchronizedEntryCountByType": [],
        "code": "NotConfigured",
        "lastExecution": null,
        "lastSuccessfulExecution": null,
        "lastSuccessfulExecutionWithExports": null,
        "steadyStateFirstAchievedTime": "0001-01-01T00:00:00Z",
        "steadyStateLastAchievedTime": "0001-01-01T00:00:00Z",
        "quarantine": null,
        "troubleshootingUrl": null
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
