---
title: Senden von Outlook-Nachrichten von einem anderen Benutzer
description: Verwenden Sie die Berechtigungen „Senden als“ und „Senden im Auftrag von“, um Outlook-Nachrichten als anderer Benutzer oder als freigegebenes Postfach in Microsoft Graph zu senden.
author: jasonjoh
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: d384e060060804ddbafb03ea054b7609bbccd71b
ms.sourcegitcommit: d9d8b908061b3680e8a52790a6c9aaf8e51ceea0
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/17/2019
ms.locfileid: "28685681"
---
# <a name="send-outlook-messages-from-another-user"></a>Senden von Outlook-Nachrichten von einem anderen Benutzer

Exchange Online bietet [Postfachberechtigungen](/Exchange/recipients/mailbox-permissions), über die ein Benutzer E-Mails senden kann, bei denen es so aussieht, als würden diese von einem anderen Benutzer, einer Verteilerliste, einer Gruppe, einer Ressource oder von einem freigegebenen Postfach gesendet werden. Microsoft Graph unterstützt dieses Feature auch, das Endergebnis variiert aber in Abhängigkeit von den genauen Berechtigungen, die in Exchange Online gewährt wurden, und von der API, die Sie zum Senden der E-Mail verwenden.

## <a name="permissions"></a>Berechtigungen

Zwei Arten von Berechtigungen gelten für das Senden von Nachrichten von einem anderen Benutzer: [Microsoft Graph-Berechtigungen](permissions-reference.md) und Berechtigungen.

### <a name="microsoft-graph-permissions"></a>Microsoft Graph-Berechtigungen

Um Nachrichten von einem anderen Benutzer zu senden, verwenden Anwendungen, die Benutzertoken verwenden, die Berechtigung **Mail.Send.Shared**.

> [!NOTE]
> Anwendungen, die Anwendungstoken anstelle von Benutzertoken verwenden und bei denen die **Mail.Send**-Berechtigung von einem Administrator genehmigt wurde, können E-Mails als beliebiger Benutzer in der Organisation senden, indem die E-Mails normal über das Postfach des Benutzers gesendet werden.

### <a name="mailbox-permissions"></a>Postfachberechtigungen

Zwei Berechtigungen haben Auswirkungen auf das Endergebnis des Sendens einer Nachricht von einem anderen Benutzer: **Senden im Auftrag von** und **Senden als**. Der Benutzer, der bei der Anwendung mit der Berechtigung **Mail.Send.Shared** angemeldet ist, MUSS mindestens eine dieser Berechtigungen für das Postfach, die Gruppe oder die Verteilerliste besitzen, von der die E-Mail stammt.

#### <a name="send-on-behalf"></a>Senden im Auftrag von

Bei dieser Berechtigung gibt es für den Empfänger der E-Mail einen Hinweis im E-Mail-Client, dass die Nachricht von dem Benutzer Ihrer Anwendung im Auftrag eines anderen Benutzers gesendet wurde.

![Screenshot von Outlook im Web, in dem angegeben wird, dass eine Nachricht von einem Benutzer im Auftrag eines anderen Benutzers gesendet wurde](images/outlook-sent-on-behalf.png)

Dies wird in Microsoft Graph als `sender`-Eigenschaft (Benutzer, der die Nachricht tatsächlich gesendet hat) und als `from`-Eigenschaft verfügbar gemacht (Benutzer/Gruppe/usw., von dem bzw. der die Nachricht zu sein scheint).

```json
{
  "id": "AAMkAGE1...",
  "subject": "Send mail test",
  "sender": {
    "emailAddress": {
      "name": "Adele Vance",
      "address": "AdeleV@contoso.com"
    }
  },
  "from": {
    "emailAddress": {
      "name": "Pradeep Gupta",
      "address": "PradeepG@contoso.com"
    }
  }
}
```

Ein Benutzer kann diese Berechtigung für das eigene Postfach einem anderen Benutzer [mithilfe von Outlook](https://support.office.com/article/Allow-someone-else-to-manage-your-mail-and-calendar-41C40C04-3BD1-4D22-963A-28EAFEC25926) erteilen. Administratoren können diese Berechtigung für ein beliebiges Postfach, eine beliebige Gruppe oder eine beliebige Verteilerliste im [Office 365 Admin Center](/office365/admin/add-users/give-mailbox-permissions-to-another-user?view=o365-worldwide) erteilen.

#### <a name="send-as"></a>Senden als

Bei dieser Berechtigung gibt es keinen Hinweis darauf, dass die Nachricht als ein anderer Benutzer gesendet wurde. Die `sender`-Eigenschaft und die `from`-Eigenschaft weisen denselben Wert auf.

Benutzer können diese Berechtigung nicht für ihre Postfächer erteilen. Administratoren können diese Berechtigung im Office 365 Admin Center erteilen.

## <a name="sending-with-microsoft-graph"></a>Senden mit Microsoft Graph

Sie können Nachrichten von einem anderen Benutzer senden, indem Sie die Nachricht [direkt senden](/graph/api/user-sendmail?view=graph-rest-1.0) oder [einen Entwurf erstellen](/graph/api/user-post-messages?view=graph-rest-1.0) und diesen dann [senden](/graph/api/message-send?view=graph-rest-1.0).

Um Nachrichten von einem anderen Benutzer zu senden, legen Sie die `from`-Eigenschaft in der [Nachricht](/graph/api/resources/message?view=graph-rest-1.0), die an die E-Mail-Adresse des Benutzers gesendet wird, auf „Senden von“ fest. Sie müssen die `sender`-Eigenschaft nicht festlegen: Microsoft Graph legt sie basierend auf den Postfachberechtigungen, die dem angemeldeten Benutzer erteilt wurden, entsprechend fest.

Konfigurieren Sie die Nachricht wie folgt, um beispielsweise E-Mails von der Gruppe `sales@contoso.com` zu senden.

```json
{
  "subject": "January sales report",
  "toRecipients": [
    {
      "emailAddress": {
        "address": "MeganB@contoso.com"
      }
    }
  ],
  "from": [
    {
      "emailAddress": {
        "address": "sales@contoso.com"
      }
    }
  ]
}
```

## <a name="sent-items-behavior"></a>Verhalten von gesendeten Elementen

Nachdem die Nachricht gesendet wurde, kann sie im Ordner „Gesendete Elemente“ des sendenden Benutzers, im Ordner „Gesendete Elemente“ des ursprünglichen Benutzers oder in beiden Ordnern gespeichert werden. Sie müssen die Nachricht aber nicht speichern.

> [!NOTE]
> Wenn die Nachricht von einer Adresse gesendet wird, die nicht über ein Postfach verfügt (z. B. eine Verteilerliste), gibt es für den Benutzer, von dem die Nachricht stammt, keinen Ordner „Gesendete Elemente“.

- Wenn Ihre Anwendung die Nachricht über den `/me`-Endpunkt sendet (oder über `/users/{user-id}`, wobei `user-id` dem angemeldeten Benutzer entspricht), so wird die Nachricht standardmäßig im Ordner „Gesendete Elemente“ des sendenden Benutzers gespeichert.
- Wenn Ihre Anwendung die Nachricht über `/users/{user-id}` sendet, wobei `user-id` dem Benutzer entspricht, von dem die Nachricht stammt, so wird die Nachricht standardmäßig im Ordner „Gesendete Elemente“ des Benutzers gespeichert, von dem die Nachricht stammt.
    > [!IMPORTANT]
    > Um eine Nachricht auf diese Weise zu senden, muss der sendende Benutzer zusätzlich zur Berechtigung **Senden im Auftrag von** oder **Senden als** über die Postfachberechtigung **Vollzugriff** verfügen.

Das Standardverhalten kann durch andere externe Faktoren geändert werden:

- Administratoren können das Postfach des Benutzers, von dem die Nachricht stammt, so ändern, [dass im Ordner „Gesendete Elemente“ immer eine Kopie von Nachrichten gespeichert wird, die von einem Stellvertreter gesendet werden](/exchange/recipients-in-exchange-online/manage-user-mailboxes/automatically-save-sent-items-in-delegator-s-mailbox).
- Durch Festlegen der `saveToSentItems`-Eigenschaft auf `true` in einer Anforderung zum [Senden von E-Mails](/graph/api/user-sendmail?view=graph-rest-1.0) können Sie verhindern, dass die Nachricht im Ordner „Gesendete Elemente“ gespeichert wird. Wenn ein Administrator aber die Einstellung „immer eine Kopie speichern“ konfiguriert hat, wird die Nachricht dennoch im Ordner „Gesendete Elemente“ des Benutzers gespeichert, von dem die Nachricht stammt.

## <a name="examples"></a>Beispiele

### <a name="example-1-successful-send-through-me-endpoint"></a>Beispiel 1: Erfolgreiches Senden über /me-Endpunkt

In diesem Beispiel wurde Adele Vance die Berechtigung **Senden im Auftrag von** für das Postfach von Allan Deyoung erteilt.

#### <a name="request"></a>Anforderung

```http
POST /me/sendmail
Content-Type: application/json

{
  "message": {
    "subject": "Expense reports",
    "body": {
      "contentType": "text",
      "content": "Have you submitted your expense reports yet?"
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "MeganB@contoso.com"
        }
      }
    ],
    "from": [
      {
        "emailAddress": {
          "address": "AllanD@contoso.com"
        }
      }
    ]
  }
}
```

#### <a name="response"></a>Antwort

```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-unsuccessful-attempt-to-send-without-permissions"></a>Beispiel 2: Fehlgeschlagener Sendeversuch ohne Berechtigungen

In diesem Beispiel versucht Adele Vance, eine E-Mail von Patti Fernandez zu senden, ihr wurde aber weder die Berechtigung **Senden im Auftrag von** noch die Berechtigung **Senden als** erteilt. Die Antwort enthält einen `ErrorSendAsDenied`-Fehler.

<!-- markdownlint-disable MD024 -->

#### <a name="request"></a>Anforderung

```http
POST /me/sendmail
Content-Type: application/json

{
  "message": {
    "subject": "Support ticket",
    "body": {
      "contentType": "text",
      "content": "I noticed you opened a support ticket yesterday..."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "MeganB@contoso.com"
        }
      }
    ],
    "from": [
      {
        "emailAddress": {
          "address": "PattiF@contoso.com"
        }
      }
    ]
  }
}
```

#### <a name="response"></a>Antwort

```http
HTTP/1.1 403 Forbidden
Content-Type: application/json

{
  "error": {
    "code": "ErrorSendAsDenied",
    "message": "The user account which was used to submit this request does not have the right to send mail on behalf of the specified sending account., Cannot submit message.",
    "innerError": {
      "request-id": "24e7991e-01ae-4cc2-8e06-532a96fd8948",
      "date": "2019-01-16T18:53:25"
    }
  }
}
```

## <a name="next-steps"></a>Nächste Schritte

Weitere Informationen:

- [Gründe für die Integration in Outlook-Mail](outlook-mail-concept-overview.md)
- [Verwenden der Mail-API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) und [Anwendungsfälle](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) für die Mail-API in Microsoft Graph v1.0.

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error: /concepts/outlook-send-mail-from-other-user.md:
      Exception processing links.
    System.ArgumentException: Link Definition was null. Link text: !NOTE
      at ApiDoctor.Validation.DocFile.get_LinkDestinations()
      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}-->
