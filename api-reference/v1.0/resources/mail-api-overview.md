---
title: Verwenden Sie die Outlook-Mail-REST-API
description: Microsoft Graph können Ihre app autorisierten Zugriff auf Outlook-Mail-Daten des Benutzers in einem persönlichen oder Organisation Konto zu erhalten.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: dc7f1a0fc4ffb26986e3b1adc6b672749b24f27d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956402"
---
# <a name="use-the-outlook-mail-rest-api"></a>Verwenden Sie die Outlook-Mail-REST-API

Mit Microsoft Graph kann Ihre App autorisierten Zugriff auf die E-Mail-Daten eines Benutzers in einem persönlichen oder Organisationskonto in Outlook erhalten. Mit den [entsprechenden delegierten Berechtigungen oder Anwendungsberechtigungen](/graph/permissions-reference) kann die App auf die E-Mail-Daten des angemeldeten Benutzers oder eines beliebigen Benutzers in einem Mandanten zugreifen. Die E-Mail-Daten können sich in der Cloud in Exchange Online als Teil von Office 365 oder in einer lokalen Exchange-Installation in einer [Hybridbereitstellung](/graph/hybrid-rest-support) befinden.

## <a name="using-the-mail-rest-api"></a>Verwenden der E-Mail-REST-API

E-Mail-API-Anforderungen werden im Auftrag eines [Benutzers](../resources/user.md) ausgeführt, der durch die Eigenschaft **ID** des Benutzers (eine eindeutige GUID), die E-Mail-Adresse oder die Aliasverknüpfung `me` für den angemeldeten Benutzer identifiziert werden kann.

E-Mail-Nachrichten werden durch die Ressource [message](../resources/message.md) dargestellt und in einem [mailFolder](../resources/mailfolder.md) organisiert. Nachrichten und E-Mail-Ordner werden durch ihre Eigenschaft **ID** identifiziert, die mit `GET`-Operationen abgerufen werden kann.

>**Hinweis:** Gehen Sie im Allgemeinen nicht davon aus, dass die IDs von **message** und **mailfolder** in einem Postfach eindeutig und unveränderlich sind. Sie können sich nach bestimmten Aktionen wie z. B. Kopieren, Verschieben oder Senden ändern.

Nachrichtentext kann im HTML- oder Textformat vorliegen.

Sie verwenden die bekannte Ordnernamen wie `Inbox`, `Drafts`, `SentItems`, oder `DeletedItems` um bestimmte e-Mail-Ordner zu identifizieren, die standardmäßig für alle Benutzer vorhanden sind. Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](../resources/mailfolder.md).

Beispielsweise können Sie Nachrichten im Ordner "Outlook **Gesendete Elemente** " des angemeldeten Benutzers abrufen, ohne die erste Abrufen der Ordner-ID:

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
| Automatische Antwort, Gebietsschema, Zeitzone oder Arbeitszeiten eines Benutzers abrufen oder aktualisieren | [mailboxSettings](../resources/mailboxsettings.md), <br> [automaticRepliesSetting](../resources/automaticrepliessetting.md), <br> [localeInfo](../resources/localeinfo.md), <br> [workingHours](../resources/workinghours.md) | [Postfacheinstellungen des Benutzers abrufen](../api/user-get-mailboxsettings.md) <br> [Postfacheinstellungen des Benutzers aktualisieren](../api/user-update-mailboxsettings.md) |
| Abrufen von anderen Empfänger spezielle Status, z. B. Abwesenheits e-Mail-Infos | [Benutzer](../resources/user.md), <br> [e-Mail-Infos](../resources/mailtips.md) | [Abrufen von e-Mail-Infos](../api/user-getmailtips.md) |
| **E-Mail- und Ordnerverwaltung** | | |
| Nachrichten in einer E-Mail-Ordnerhierarchie organisieren | [mailFolder](../resources/mailfolder.md)  | [Methoden von „mailFolder“](../resources/mailfolder.md#methods) |
| Nachrichten suchen und filtern | [message](../resources/message.md) | [Abfrageparameter](/graph/query-parameters)  |
| Benachrichtigung über Änderungen an Nachrichten in einem Ordner erhalten | [subscription](../resources/subscription.md) | [Arbeiten mit Webhooks in Microsoft Graph](../resources/webhooks.md) |
| Nachrichten oder eine E-Mail-Ordnerhierarchie synchronisieren | [message](../resources/message.md) | [Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen](/graph/delta-query-messages) |
| **App-Entwicklung** | | |
| Hinzufügen von benutzerdefinierten app-Daten als Internet Nachrichtenkopfzeilen einer Nachricht | [message](../resources/message.md) | Hinzufügen von benutzerdefinierten Daten an die **InternetMessageHeaders** -Eigenschaft der Nachricht. |
| Benutzerdefinierte App-Daten mithilfe von Erweiterungen zu einer Nachricht hinzufügen | [openTypeExtension](../resources/opentypeextension.md), <br>[schemaExtension](../resources/schemaextension.md) | [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](/graph/extensibility-overview) |
| Auf benutzerdefinierte Daten für nicht ausreichend verfügbare Outlook-MAPI-Eigenschaften zugreifen | [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), <br> [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) | [Übersicht über erweiterte Outlook-Eigenschaften](../resources/extended-properties-overview.md) |

## <a name="next-steps"></a>Nächste Schritte

Die E-Mail-API kann Ihnen neue Möglichkeiten für die Interaktion mit Benutzern eröffnen:

- [Übersicht über die Outlook-Mail-API](/graph/outlook-mail-concept-overview)
- Führen Sie einen Drilldown für die [Methoden](../resources/message.md#methods), [Eigenschaften](../resources/message.md#properties) und [Beziehungen](../resources/message.md#relationships) der Ressourcen [message](../resources/message.md) und [mailFolder](../resources/mailfolder.md) aus.
- Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus.

Benötigen Sie weitere Ideen? Dann sehen Sie sich an, [wie unsere Partner Microsoft Graph verwenden](https://developer.microsoft.com/graph/graph/examples#partners).
