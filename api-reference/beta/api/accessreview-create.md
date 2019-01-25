---
title: Erstellen von accessReview
description: Zugriff auf in Azure AD Bewertungen Feature, Erstellen eines neuen AccessReview-Objekts.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 669b11a8f3b52e867d6b3e803c9419968924928b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517799"
---
# <a name="create-accessreview"></a>Erstellen von accessReview

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Erstellen Sie ein neues [AccessReview](../resources/accessreview.md) -Objekt in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature.

Vor der Durchführung dieser Anforderung, der Anrufer benötigen zuvor [die Liste der Vorlagen für Unternehmen Fluss abgerufen](businessflowtemplate-list.md), auf dem Wert der `businessFlowTemplateId` in der Anforderung enthalten.

Nach dem Ändern dieser Anforderung, sollte der Aufrufer [eine ProgramControl erstellen](programcontrol-create.md), um die Überprüfung des Zugriffs auf ein Programm verknüpfen.  

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)     | AccessReview.ReadWrite.All, und sollten auch ProgramControl.ReadWrite.All vollständige Szenario mit den nachfolgenden Aufruf einer ProgramControl erstellen |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt |
|Anwendung                            | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a>Anforderungsheader
| Name         | Typ        | Beschreibung |
|:-------------|:------------|:------------|
| Authorization | string | Bearertoken Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [AccessReview](../resources/accessreview.md) -Objekts.

In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie eine AccessReview erstellen.

| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | Der Name des Access überprüfen.  |
| `startDateTime`           |`DateTimeOffset`                                                | Den DateTime-Wert, wenn die Überprüfung geplant ist, gestartet werden.  Dies muss ein Datum in der Zukunft sein.   |
| `endDateTime`             |`DateTimeOffset`                                                | Den DateTime-Wert, wenn die Überprüfung geplant ist, um zu beenden. Dies muss mindestens einen Tag später als das Startdatum sein.   |
| `description`             |`String`                                                        | Die Beschreibung für die Bearbeiter angezeigt. |
| `businessFlowTemplateId`  |`String`                                                        | Der Business-Fluss Vorlagenbezeichner, von einem [BusinessFlowTemplate](../resources/businessflowtemplate.md)abgerufen.  |
| `reviewerType`            |`String`                                                        | Die Beziehungstyp des Reviewer über die Zugriffsrechte des überarbeiteten-Objekts, eines `self`, `delegated`, oder `entityOwners`. | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | Das Objekt, für das eine Überprüfung Access, wie die Mitgliedschaft einer Gruppe oder die Zuweisung von Benutzern zu einer Anwendung erstellt wird. | 


Wenn die ReviewerType gesendet wird den Wert `delegated`, und klicken Sie dann der Anrufer auch umfassen muss die `reviewers` -Eigenschaft, mit einer Auflistung von [Benutzeridentität](../resources/useridentity.md) der Bearbeiter.

Darüber hinaus kann der Aufrufer Einstellungen, zum Erstellen einer Terminserie überprüfen oder So ändern Sie das Standardverhalten für die Überprüfung umfassen. Zum Erstellen einer wiederkehrenden Überprüfung der Anrufer muss sich insbesondere die `accessReviewRecurrenceSettings` überprüfen Sie in die Access-Einstellungen


## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode eine `201, Created` Antwortcode und eines [AccessReview](../resources/accessreview.md) -Objekts in der Antworttext.

## <a name="example"></a>Beispiel

Dies ist ein Beispiel zum Erstellen einer einmaligen (nicht wiederkehrende) Access Überprüfung als Bearbeiter zwei Benutzer explizit angeben.

##### <a name="request"></a>Anforderung
Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [AccessReview](../resources/accessreview.md) -Objekts.

<!-- {
  "blockType": "request",
  "name": "create_accessReview_from_accessReviews"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews
Content-type: application/json

{
    "displayName":"TestReview",
    "startDateTime":"2017-02-10T00:35:53.214Z",
    "endDateTime":"2017-03-12T00:35:53.214Z",
    "reviewedEntity": {
        "id": "99025615-a0b1-47ec-9117-35377b10998b",
    },
    "reviewerType" : "delegated",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "description":"Sample description",
    "reviewers":
    [
        {
            "id":"f260246a-09b1-4fd5-8d18-daed736071ec"
        },
        {
            "id":"5a4e184c-4ee5-4883-96e9-b371f8da88e3"
        }
    ],
    "settings":
    {
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval":true,
        "autoReviewEnabled":false,
        "activityDurationInDays":30,
        "autoApplyReviewResultsEnabled":false,
        "accessRecommendationsEnabled":false,
        "recurrenceSettings":{
            "recurrenceType":"onetime",
            "recurrenceEndType":"endBy",
            "durationInDays":0,
            "recurrenceCount":0
        },
        "autoReviewSettings":{
            "notReviewedResult":"Deny"
        }
    }
}
```

##### <a name="response"></a>Antwort
>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview",
    "startDateTime": "2017-02-10T00:35:53.214Z",
    "endDateTime": "2017-03-12T00:35:53.214Z",
    "status": "Initializing",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "delegated",
    "description": "Sample description"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Create accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-create.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
