---
title: Erstellen von accessReview
description: Zugriff auf in Azure AD Bewertungen Feature, Erstellen eines neuen AccessReview-Objekts.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2bb8db52dd3e5086ba9559ef318a94b8ac3a3918
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942269"
---
# <a name="create-accessreview"></a>Erstellen von accessReview

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Erstellen Sie ein neues [AccessReview](../resources/accessreview.md) -Objekt in Azure AD [Access überprüft](../resources/accessreviews-root.md) Feature.

Vor dieser Anforderung ausführenden, der Anrufer benötigen zuvor [die Liste der Vorlagen für Unternehmen Fluss abgerufen](businessflowtemplate-list.md), auf dem Wert der `businessFlowTemplateId` in der Anforderung enthalten.

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
| Authorization | string | Bearer \{token\}. Erforderlich. |

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
| `reviewerType`            |`String`                                                        | Die Beziehungstyp des Reviewer über die Zugriffsrechte des überarbeiteten-Objekts, eines `self`, `delegate` oder `entityOwners`. | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | Das Objekt, für das eine Überprüfung Access, wie eine Mitgliedschaft in einer Gruppe oder die Zuweisung von Benutzern zu einer Anwendung erstellt wird. | 


Wenn die ReviewerType gesendet wird den Wert `delegate`, und klicken Sie dann der Anrufer auch umfassen muss die `reviewers` -Eigenschaft, mit einer Auflistung von [Benutzeridentität](../resources/useridentity.md) der Bearbeiter.

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
    "reviewerType" : "delegate",
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
        "justificationRequiredOnApproval": true,
        "activityHistoryInDays":30,
        "mailNotificationsEnabled":true,
        "remindersEnabled":true
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
    "reviewerType": "delegate",
    "description": "Sample description"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Create accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
