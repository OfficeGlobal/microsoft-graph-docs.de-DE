---
title: Organisieren von Outlook-Nachrichten
description: 'In Outlook können Kunden ihre Nachrichten so organisieren, wie sie möchten: alle Nachrichten im gleichen Posteingangsordner, oder Nachrichten werden in Abhängigkeit von den jeweiligen Anforderungen in einer Ordnerstruktur unter dem Posteingang gespeichert. Sie können Nachrichten des Benutzers bequem filtern, suchen oder sortieren.'
ms.openlocfilehash: 870da6cfed6bc286c0e9869dd98220d260b1e7ad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092287"
---
# <a name="organize-outlook-messages"></a>Organisieren von Outlook-Nachrichten

In Outlook können Kunden ihre Nachrichten so organisieren, wie sie möchten: alle Nachrichten im gleichen Posteingangsordner, oder Nachrichten werden in Abhängigkeit von den jeweiligen Anforderungen in einer Ordnerstruktur unter dem Posteingang gespeichert. Nachrichten im gesamten Postfach des Benutzers oder in speziellen Ordner können ganz praktisch [gefiltert, gesucht oder sortiert](query-parameters.md) werden.

## <a name="accessing-mail-folders"></a>Zugreifen auf E-Mail-Ordner

Nachrichtenordner werden programmgesteuert von der [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0)-Ressource dargestellt, und der Posteingang ist einer der Ordner am Stamm der Ordnerstruktur.

Jeder **mailFolder** wird durch seine Ordner-ID identifiziert und weist eine schreibbare **displayName**-Eigenschaft auf. Outlook erstellt standardmäßig ein paar andere Ordner für Kunden. Sie können auf diese Standardordner anhand ihrer Ordner-IDs oder anhand ihrer bekannten Namen verweisen. Eine Liste der verfügbaren bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](/graph/api/resources/mailfolder?view=graph-rest-1.0).

Wenn Sie bei einem benutzerdefinierten, nicht standardmäßigen Ordner dessen Ordnerpfad kennen, können Sie auf den Ordner zugreifen, indem Sie zuerst die `/users/{id}/mailfolders` -Verknüpfung verwenden, um zur Stammebene zu gelangen, und dann alle Ordner der oberen Ebene abrufen:

```http
GET https://graph.microsoft.com/v1.0/users/{id}/mailFolders
```

Geben Sie dann die entsprechende Ordner-ID (`{folder_id}`) an, wenn Sie durch die einzelnen Ebenen der Ordnerstruktur navigieren:

```http
GET https://graph.microsoft.com/v1.0/users/{id}/mailFolders/{folder_id}/childfolders
```

Wiederholen Sie diese Schritte, bis Sie schließlich zum benutzerdefinierten Ordner in der Struktur gelangen.

## <a name="creating-and-organizing-the-folder-tree"></a>Erstellen und Organisieren der Ordnerstruktur

Sie können [E-Mail-Ordner unter dem Posteingang erstellen](/graph/api/user-post-mailfolders?view=graph-rest-1.0) oder [als untergeordnete Ordner von anderen Ordnern](/graph/api/mailfolder-post-childfolders?view=graph-rest-1.0). Wenn Sie einen Ordner und seine Inhalte erstellen, [kopieren](/graph/api/mailfolder-copy?view=graph-rest-1.0) oder [verschieben](/graph/api/mailfolder-move?view=graph-rest-1.0), aktualisiert Outlook die schreibgeschützten Eigenschaften **parentFolderId** und **childFolderCount** der beteiligten Ordner. Wenn die Inhalte eines Ordners in einen anderen Ordner kopiert oder verschoben werden, ändern sich standardmäßig auch die einzelnen Eintrags-IDs der Inhalte.

Auf der Inhaltsebene erhalten Sie durch **totalItemCount** bzw. **unreadItemCount** die Anzahl der Elemente und die Anzahl der ungelesenen Elemente in einem E-Mail-Ordner.
Auf der Ebene der untergeordneten Ordner können Sie [die untergeordneten Ordner](/graph/api/user-list-mailfolders?view=graph-rest-1.0) unter dem Posteingang oder einem beliebigen anderen Ordner auflisten.
Die **childFolderCount**-Eigenschaft gibt die Anzahl der unmittelbar untergeordneten Ordner an.

Beachten Sie, dass Outlook-E-Mail-Ordner Nachrichtenelemente und Nicht-Nachrichtenelemente wie Ereignisse und Kontakte enthalten können. Im Allgemeinen können Outlook-Ordner heterogene Elemente enthalten.

## <a name="using-rules-to-automate-copying-or-moving-messages"></a>Verwenden von Regel zum Automatisieren des Kopierens oder Verschiebens von Nachrichten

In Outlook können Kunden Regeln einrichten, um bestimmte Aktionen für eingehende Nachrichten zu automatisieren, wenn einige zuvor festgelegten Bedingungen erfüllt sind. Sie können [eine Regel](/graph/api/mailfolder-post-messagerules?view=graph-rest-1.0) für den Posteingang als eine [messageRule](/graph/api/resources/messagerule?view=graph-rest-1.0) erstellen, um eine Nachricht bei bestimmten Bedingungen in einen bestimmten Ordner zu kopieren oder zu verschieben.
Kriterien sind [messageRulePredicates](/graph/api/resources/messagerulepredicates?view=graph-rest-1.0). Sie können den Nachrichtenbetreff oder -text mit bestimmten Formulierungen, die von bestimmten E-Mail-Adressen gesendeten Nachrichten oder eine als wichtig markierte Nachricht enthalten.

## <a name="directing-only-the-messages-you-care-for-to-the-focused-inbox"></a>Weiterleiten der für Sie wichtigen Nachrichten an den Posteingang mit Relevanz

Über den Posteingang mit Relevanz können Kunden Outlook so trainieren, dass nur die eingehenden Nachrichten von Absendern, die Ihnen wichtig sind, auf der Registerkarte **Relevant** und die restlichen Nachrichten auf der Registerkarte **Andere** angezeigt werden. Zu Beginn werden die Posteingangsnachrichten vom Klassifizierungssystem von Outlook standardmäßig organisiert. Im Laufe der Zeit können Sie das System über die Benutzeroberfläche oder programmgesteuert korrigieren oder trainieren. Je mehr Sie den Posteingang mit Relevanz verwenden, umso besser kann das Klassifizierungssystem ableiten, welche eingehenden Nachrichten auf der Registerkarte **Relevant** angezeigt werden sollen.

Sie können die **inferenceClassification**-Eigenschaft einer [Nachricht](/graph/api/resources/message?view=graph-rest-1.0) programmgesteuert so aktualisieren, dass angegeben wird, ob die Nachricht auf der Registerkarte **Relevant** oder **Andere** angezeigt werden soll. Dies ist eine einmalige Bezeichnung für eine bestimmte Nachricht. Wenn Sie andererseits Nachrichten von einem bestimmten Absender immer auf der Registerkarte **Relevant** oder auf der Registerkarte **Sonstige** sehen möchten, können Sie für Outlook eine [Anweisung festlegen](/graph/api/inferenceclassification-post-overrides?view=graph-rest-1.0). Jede Anweisung ist eine [inferenceClassificationOverride](/graph/api/resources/inferenceclassificationoverride?view=graph-rest-1.0)-Instanz, die den Namen des Absenders und Ihre Bezeichnung für Nachrichten von diesem Absender als immer `focused` oder `other` angibt. Die Anweisungen jedes Benutzers für den Posteingang mit Relevanz des Benutzers werden als eine Sammlung von [inferenceClassificationOverride](/graph/api/resources/inferenceclassificationoverride?view=graph-rest-1.0)-Instanzen für das [user](/graph/api/resources/user?view=graph-rest-1.0)-Objekt gespeichert.

## <a name="keeping-messages-and-mail-folders-up-to-date-in-apps"></a>Nachrichten und E-Mail-Ordner in Apps auf dem neuesten Stand halten

Apps müssen häufig synchronisiert werden und die E-Mail-Daten eines Benutzers im lokalen App-Speicher auf dem neuesten Stand halten. Mit Microsoft Graph können Sie Änderungsbenachrichtigungen abonnieren, um eine Benachrichtigung zu erhalten, wenn sich Daten ändern, und tatsächliche Änderungen direkt bei ihrem Auftreten abzufragen.

Benachrichtigungen werden über [Webhooks](/graph/api/resources/webhooks?view=graph-rest-1.0) asynchron gesendet, wenn die Änderungen auftreten, sodass den Apps der Aufwand des häufigen Abfragens erspart bleibt. Sie können [Änderungsbenachrichtigungen](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0) zu Ergänzungen, Updates oder Löschungen im Zusammenhang mit den E-Mail-Daten eines Benutzers abonnieren. Sie können z. B. ein Abonnement für Nachrichten in einem bestimmten Ordner (d. h. `/me/mailFolders('{folderId'}')`) oder auf der Stammebene (d. h. `/me/messages`) erstellen. Das Abonnement gibt eine **notificationUrl** an, unter der Microsoft Graph die App benachrichtigt, wenn die angeforderten Arten von Änderungen auftreten.

Um das Postfach eines Benutzers zum ersten Mal zu synchronisieren, führen Sie zunächst eine [Delta-Abfrage für E-Mail-Ordner, die auf der Stammebene beginnen, aus](/graph/api/mailfolder-delta?view=graph-rest-1.0), um alle E-Mail-Ordner zu synchronisieren. Führen Sie dann eine [Delta-Abfrage für Nachrichten in den einzelnen Ordnern aus](/graph/api/message-delta?view=graph-rest-1.0), um einzelnen Nachrichten zu synchronisieren.

Um die genauen Entitäten zu finden, die geändert wurden, ohne die gesamte Ressource bei jeder Benachrichtigung zu lesen, können Sie die [Delta-Abfrage](delta-query-overview.md) verwenden, um die Änderungen zu verfolgen, die Ihnen wichtig sind, und Ihren lokalen Speicher mit diesen Änderungen zu synchronisieren. Sie können [Änderungen an Nachrichten in einem bestimmten Ordner nachverfolgen](delta-query-messages.md). Es können auch Änderungen an E-Mail-Ordnern auf der Stammebene nachverfolgt werden (d. h. `/me/mailfolders`).

## <a name="next-steps"></a>Nächste Schritte

Weitere Informationen:

- [Gründe für die Integration in Outlook-Mail](outlook-mail-concept-overview.md)
- [Verwenden der Mail-API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) und [Anwendungsfälle](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) für diese in Microsoft Graph v1.0.
