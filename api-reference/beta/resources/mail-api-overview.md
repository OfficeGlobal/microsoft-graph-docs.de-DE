---
title: Verwenden der Outlook-Mail-REST-API
description: Mit Microsoft Graph kann Ihre App autorisierten Zugriff auf die E-Mail-Daten eines Benutzers in einem persönlichen oder Organisationskonto in Outlook erhalten.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 6f5d084aa64424500a311577631fa232e8ddf523
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519682"
---
# <a name="use-the-outlook-mail-rest-api"></a>Verwenden der Outlook-Mail-REST-API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Mit Microsoft Graph kann Ihre App autorisierten Zugriff auf die E-Mail-Daten eines Benutzers in einem persönlichen oder Organisationskonto in Outlook erhalten. Mit den [entsprechenden delegierten Berechtigungen oder Anwendungsberechtigungen](/graph/permissions-reference) kann die App auf die E-Mail-Daten des angemeldeten Benutzers oder eines beliebigen Benutzers in einem Mandanten zugreifen. Die E-Mail-Daten können sich in der Cloud in Exchange Online als Teil von Office 365 oder in einer lokalen Exchange-Installation in einer [Hybridbereitstellung](/graph/hybrid-rest-support) befinden.

## <a name="using-the-mail-rest-api"></a>Verwenden der E-Mail-REST-API

E-Mail-API-Anforderungen werden im Auftrag eines [Benutzers](../resources/user.md) ausgeführt, der durch die Eigenschaft **ID** des Benutzers (eine eindeutige GUID), die E-Mail-Adresse oder die Aliasverknüpfung `me` für den angemeldeten Benutzer identifiziert werden kann.

E-Mail-Nachrichten werden durch die Ressource [message](../resources/message.md) dargestellt und in einem [mailFolder](../resources/mailfolder.md) organisiert. Nachrichten und E-Mail-Ordner werden durch ihre Eigenschaft **ID** identifiziert, die mit `GET`-Operationen abgerufen werden kann.

> **Hinweis:** Gehen Sie im Allgemeinen nicht davon aus, dass die IDs von **message** und **mailfolder** in einem Postfach eindeutig und unveränderlich sind. Sie können sich nach bestimmten Aktionen wie z. B. Kopieren, Verschieben oder Senden ändern.

Nachrichtentext kann im HTML- oder Textformat vorliegen.

Sie können bekannte Ordnernamen wie `Inbox`, `Drafts`, `SentItems` oder `DeletedItems` verwenden, um bestimmte E-Mail-Ordner zu identifizieren, die standardmäßig für alle Benutzer vorhanden sind. Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](../resources/mailfolder.md).

Sie können z. B. Nachrichten im Outlook-Ordner **Gesendete Elemente** des angemeldeten Benutzers abrufen, ohne zuerst die Ordner-ID abzurufen:

```http
GET /me/mailFolders('SentItems')/messages?$select=sender,subject
```

## <a name="common-use-cases"></a>Allgemeine Anwendungsfälle

Die Ressource **message** macht Eigenschaften wie **categories**, **conversationId**, **flag** und **importance** verfügbar, die Features in der Benutzeroberfläche entsprechen, sodass Apps die integrierte Outlook-Benutzeroberfläche automatisieren oder integrieren können.

Die Microsoft Graph-API stellt zudem Methoden und Aktionen bereit, die allgemeine Anwendungsfälle von Nachrichten unterstützen.

| Anwendungsfälle | REST-Ressourcen | Siehe auch |
|:----------|:---------------|:---------|
| **Benutzerorientierte Aktionen** | | |
| Nachrichten entwerfen, lesen, beantworten, weiterleiten, senden, aktualisieren oder löschen | [message](../resources/message.md) | [Methoden von „message“](../resources/message.md#methods) |
| Das Versenden von Nachrichten im Auftrag des Postfachbesitzers an einen anderen Benutzer delegieren | [message](../resources/message.md) | Festlegen der Eigenschaften **from** und **sender** in einer [Nachricht](../resources/message.md) |
| Wichtigere Nachrichten zuerst anzeigen | [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) | [Posteingang mit Fokus](../resources/manage-focused-inbox.md) |
| Anlagen einer Nachricht hinzufügen, abrufen oder löschen | [attachment](../resources/attachment.md), <br> [fileAttachment](../resources/fileattachment.md), <br> [itemAttachment](../resources/itemattachment.md), <br> [referenceAttachment](../resources/referenceattachment.md), <br> [message](../resources/message.md) | [Methoden von „attachment“](../resources/attachment.md#methods) |
| Sprach- und Zeitzonenauswahl für einen Benutzer abrufen | [localeInfo](localeinfo.md), <br> [timeZoneInformation](timezoneinformation.md) | [supportedLanguages](../api/outlookuser-supportedlanguages.md), <br> [supportedTimeZones](../api/outlookuser-supportedtimezones.md) |
| Automatische Antwort, Gebietsschema, Zeitzone oder Arbeitszeiten eines Benutzers abrufen oder aktualisieren | [mailboxSettings](../resources/mailboxsettings.md), <br> [automaticRepliesSetting](../resources/automaticrepliessetting.md), <br> [localeInfo](../resources/localeinfo.md), <br> [workingHours](../resources/workinghours.md) | [Postfacheinstellungen des Benutzers abrufen](../api/user-get-mailboxsettings.md) <br> [Postfacheinstellungen des Benutzers aktualisieren](../api/user-update-mailboxsettings.md) |
| E-Mail-Infos über andere besondere Zustände eines Empfängers abrufen, wie z. B. Out-of-Office | [user](../resources/user.md), <br> [mailTips](../resources/mailtips.md) | [MailTips abrufen](../api/user-getmailtips.md) |
| Benutzer warnen, wenn in anderen Nachrichten (Vorschau) erwähnt | [Erwähnung (Vorschau)](../resources/mention.md) | [Abrufen von Details zu @-Erwähnungen in einer Nachricht](../api/message-get.md#request-2) |
| Benutzer von einer E-Mail-Verteilerliste entfernen (Vorschau) | [Nachricht (Vorschau)](../resources/message.md) | [Unsubscribe](../api/message-unsubscribe.md) |
| **E-Mail- und Ordnerverwaltung** | | |
| Nachrichten in einer E-Mail-Ordnerhierarchie organisieren | [mailFolder](../resources/mailfolder.md)  | [Methoden von „mailFolder“](../resources/mailfolder.md#methods) |
| Kategorisieren von Nachrichten | [outlookCategory (Vorschau)](../resources/outlookcategory.md) | [Methoden von outlookCategory](../resources/outlookcategory.md#methods) |
| Verwenden von Posteingangsregeln zum Automatisieren von Aktionen, wie z. B. Weiterleiten bestimmter eingehender Nachrichten | [messageRule (Vorschau)](../resources/messagerule.md) | [Methoden von „messageRule“](../resources/messagerule.md#methods) |
| Internetkopfzeilen einer Nachricht erhalten | [Nachricht (Vorschau)](../resources/message.md) | [Abrufen der **internetMessageHeaders**-Eigenschaft einer Nachricht](../api/message-get.md#request-4). |
| Nachrichten suchen und filtern | [message](../resources/message.md) | [Abfrageparameter](/graph/query-parameters)  |
| Benachrichtigung über Änderungen an Nachrichten in einem Ordner erhalten | [subscription](../resources/subscription.md) | [Arbeiten mit Webhooks in Microsoft Graph](../resources/webhooks.md) |
| Nachrichten oder eine E-Mail-Ordnerhierarchie synchronisieren | [message](../resources/message.md) | [Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen](/graph/delta-query-messages) |
| **App-Entwicklung** | | |
| Benutzerdefinierte App-Daten als Internetkopfzeilen einer Nachricht hinzufügen | [message](../resources/message.md) | Benutzerdefinierte Daten zur **InternetMessageHeaders**-Sammlung der Nachricht hinzufügen |
| Benutzerdefinierte App-Daten mithilfe von Erweiterungen zu einer Nachricht hinzufügen | [openTypeExtension](../resources/opentypeextension.md), <br>[schemaExtension](../resources/schemaextension.md) | [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](/graph/extensibility-overview) |
| Auf benutzerdefinierte Daten für nicht ausreichend verfügbare Outlook-MAPI-Eigenschaften zugreifen | [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), <br> [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) | [Übersicht über erweiterte Outlook-Eigenschaften](../resources/extended-properties-overview.md) |

## <a name="next-steps"></a>Nächste Schritte

Die E-Mail-API kann Ihnen neue Möglichkeiten für die Interaktion mit Benutzern eröffnen:

- [Übersicht über die Outlook-Mail-API](/graph/outlook-mail-concept-overview)
- Führen Sie einen Drilldown für die [Methoden](../resources/message.md#methods), [Eigenschaften](../resources/message.md#properties) und [Beziehungen](../resources/message.md#relationships) der Ressourcen [message](../resources/message.md) und [mailFolder](../resources/mailfolder.md) aus.
- Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus.

Benötigen Sie weitere Ideen? Dann sehen Sie sich an, [wie unsere Partner Microsoft Graph verwenden](https://developer.microsoft.com/graph/graph/examples#partners).
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/mail-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
