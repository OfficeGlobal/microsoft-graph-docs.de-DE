---
title: Abonnement Ressourcentyp
description: 'Ein Abonnement ermöglicht einer Client-App, Benachrichtigungen zu Änderungen an Daten in Microsoft Graph zu erhalten. Derzeit werden Abonnements für die folgenden Ressourcen aktiviert:'
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 9de48cc6a3e5dde459673117d9ee00a34477faf6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163938"
---
# <a name="subscription-resource-type"></a>Abonnement Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ein Abonnement ermöglicht einer Client-App, Benachrichtigungen zu Änderungen an Daten in Microsoft Graph zu erhalten. Derzeit werden Abonnements für die folgenden Ressourcen aktiviert:

- [Nachricht][], [Ereignis][]oder [Kontakt][] in Outlook
- Eine unter [Haltung][] einer Office 365-Gruppe
- Inhalt in der Hierarchie eines Stammordners [driveItem][] in OneDrive for Business oder eines Stammordners oder Unterordners [driveItem][] in der persönlichen OneDrive eines Benutzers
- Ein [Benutzer][] oder eine [Gruppe][] in Azure Active Directory
- Eine [Warnung][] aus der Sicherheits-API von Microsoft Graph


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.subscription"
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------|:-----|:------------|
| changeType | Zeichenfolge | Erforderlich. Gibt den Typ der Änderung in der abonnierten Ressource an, die eine Benachrichtigung auslöst. Unterstützte Werte sind: `created`, `updated`, `deleted`. Es können mehrere Werte mithilfe einer durch Trennzeichen getrennten Liste zusammen verwendet werden. <br><br>Hinweis: Drive-Stammelement Benachrichtigungen unterstützen `updated` nur den ChangeType. Unterstützung `updated` von Benutzer-und `deleted` Gruppenbenachrichtigungen und ChangeType. |
| notificationUrl | Zeichenfolge | Erforderlich. Die URL des Endpunkts, der die Benachrichtigungen empfängt. Diese URL muss das HTTPS-Protokoll verwenden. |
| resource | Die Ressource, auf die Sie zugreifen möchten. | Erforderlich. Gibt die Ressource an, die auf Änderungen überwacht wird. Die Basis-URL darf nicht eingeschlossen`https://graph.microsoft.com/beta/`werden (). |
| expirationDateTime | DateTimeOffset | Erforderlich. Gibt Datum und Uhrzeit für das Ablaufen des Webhook-Abonnements an. Die Zeit wird in UTC angegeben und kann eine Dauer aus der Erstellung des Abonnements sein, die von der abonnierten Ressource abweicht.  In der folgenden Tabelle finden Sie die maximale Dauer unterstützter Abonnements. |
| clientState | string | Optional. Gibt den Wert der `clientState`-Eigenschaft an, die in jeder Benachrichtigung vom Dienst gesendet wird. Die maximale Länge ist 255 Zeichen. Der Client kann prüfen, ob die Benachrichtigung vom Dienst stammt, indem er den Wert der mit dem Abonnement gesendeten `clientState`-Eigenschaft mit dem Wert der mit jeder Benachrichtigung empfangenen `clientState`-Eigenschaft vergleicht. |
| id | string | Eindeutige ID für das Abonnement. Schreibgeschützt. |
| applicationId | Zeichenfolge | Der Bezeichner der Anwendung, die zum Erstellen des Abonnements verwendet wird. Schreibgeschützt. |
| Creator-Nr. | Zeichenfolge | Der Bezeichner des Benutzers oder Dienst Prinzipals, der das Abonnement erstellt hat. Wenn die APP Delegierte Berechtigungen zum Erstellen des Abonnements verwendet hat, enthält dieses Feld die ID des signierten Benutzers, für den die app aufgerufen wird. Wenn die APP Anwendungsberechtigungen verwendet, enthält dieses Feld die ID des Dienst Prinzipals, der der APP entspricht. Schreibgeschützt. |

## <a name="maximum-length-of-subscription-per-resource-type"></a>Maximale Abonnementdauer pro Ressourcentyp

| Ressource            | Maximal zulässige Ablaufzeit  |
|:--------------------|:-------------------------|
| Mail                | 4230 Minuten (weniger als 3 Tage)    |
| Kalender            | 4230 Minuten (weniger als 3 Tage)    |
| Kontakte            | 4230 Minuten (weniger als 3 Tage)    |
| Gruppenunterhaltungen | 4230 Minuten (weniger als 3 Tage)    |
| Laufwerkstammelemente    | 4230 Minuten (weniger als 3 Tage)    |
| Sicherheitswarnungen     | 43200 Minuten (weniger als 30 Tage)  |

> **Hinweis:** Vorhandene Anwendungen und neue Anwendungen sollten den unterstützten Wert nicht überschreiten. In Zukunft schlagen alle Anforderungen zum Erstellen oder Erneuern eines Abonnements, die den Maximalwert überschreiten, fehl.

## <a name="relationships"></a>Beziehungen

Keine

## <a name="methods"></a>Methoden

| Methode | Rückgabetyp | Beschreibung |
|:-------|:------------|:------------|
| [Create subscription](../api/subscription-post-subscriptions.md) | [Abonnement](subscription.md) | Abonniert eine Listener-Anwendung zum Empfangen von Benachrichtigungen, wenn Microsoft Graph-Daten geändert werden. |
| [Update subscription](../api/subscription-update.md) | [subscription](subscription.md) | Erneuern Sie ein Abonnement, indem Sie dessen Ablaufzeit aktualisieren. |
| [Listen Abonnements](../api/subscription-list.md) | [subscription](subscription.md) | Listet aktive Abonnements auf. |
| [Get subscription](../api/subscription-get.md) | [Abonnement](subscription.md) | Lesen von Eigenschaften und Beziehungen des Subscription-Objekts. |
| [Delete subscription](../api/subscription-delete.md) | Keine | Löscht ein Subscription-Objekt. |

[Kontakt]: ./contact.md
[Unterhaltung]: ./conversation.md
[driveItem]: ./driveitem.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[Warnung]: ./alert.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/subscription.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
