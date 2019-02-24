---
title: subscription-Ressourcentyp
description: 'Mit einem Abonnement kann eine Client-App Benachrichtigungen zu Datenänderungen in Microsoft Graph erhalten. Für die folgenden Ressourcen sind derzeit Abonnements aktiviert:'
localization_priority: Priority
author: piotrci
ms.openlocfilehash: db3a536395f327115af69f769f37c823013ec7fa
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155762"
---
# <a name="subscription-resource-type"></a>subscription-Ressourcentyp

Mit einem Abonnement kann eine Client-App Benachrichtigungen zu Datenänderungen in Microsoft Graph erhalten. Für die folgenden Ressourcen sind derzeit Abonnements aktiviert:

- [Nachrichten][], [Ereignisse][] oder [Kontakte][] in Outlook
- [Unterhaltungen][] einer Office 365-Gruppe
- Inhalte in der Hierarchie eines [driveItem][]-Stammordners in OneDrive for Business bzw. eines [driveItem][]-Stammordners oder -Unterordners im persönlichen OneDrive eines Benutzers
- [Benutzer][] oder [Gruppen][] in Azure Active Directory
- [Warnungen][] aus der Microsoft Graph-Sicherheits-API

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscription",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false,
        "sortable": false
      }
    }
  ]
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------|:-----|:------------|
| changeType | string | Erforderlich. Gibt den Typ der Änderung in der abonnierten Ressource an, die eine Benachrichtigung auslöst. Unterstützte Werte sind: `created`, `updated`, `deleted`. Es können mehrere Werte mithilfe einer durch Trennzeichen getrennten Liste zusammen verwendet werden.<br><br>Hinweis: Benachrichtigungen für Laufwerkstammelemente unterstützen nur den `updated`-changeType. Benachrichtigungen für Benutzer und Gruppen unterstützen den `updated`- und den `deleted`-changeType.|
| notificationUrl | string | Erforderlich. Die URL des Endpunkts, der die Benachrichtigungen erhält. Diese URL muss das HTTPS-Protokoll verwenden. |
| resource | string | Erforderlich. Gibt die Ressource an, deren Änderungen überwacht werden. Fügen Sie nicht die Basis-URL hinzu (`https://graph.microsoft.com/v1.0/`). |
| expirationDateTime | [dateTime](https://tools.ietf.org/html/rfc3339) | Erforderlich. Gibt Datum und Uhrzeit für das Ablaufen des Webhook-Abonnements an. Die Zeit wird in UTC angegeben und kann eine Dauer aus der Erstellung des Abonnements sein, die von der abonnierten Ressource abweicht.  In der folgenden Tabelle finden Sie die maximale Dauer unterstützter Abonnements. |
| clientState | string | Optional. Gibt den Wert der `clientState`-Eigenschaft an, die in jeder Benachrichtigung vom Dienst gesendet wird. Die Höchstlänge beträgt 128 Zeichen. Der Client kann prüfen, ob die Benachrichtigung vom Dienst stammt, indem er den Wert der mit dem Abonnement gesendeten `clientState`-Eigenschaft mit dem Wert der mit jeder Benachrichtigung empfangenen `clientState`-Eigenschaft vergleicht. |
| id | string | Eindeutige ID für das Abonnement. Schreibgeschützt. |
| applicationId | string | Bezeichner der Anwendung, die zum Erstellen des Abonnements verwendet wird. Schreibgeschützt. |
| creatorId | string | Bezeichner des Benutzers oder Dienstprinzipals, der das Abonnement erstellt hat. Wenn die App delegierte Berechtigungen zum Erstellen des Abonnements verwendet hat, enthält dieses Feld die ID des angemeldeten Benutzers, für den die App den Aufruf ausgeführt hat. Wenn die App Anwendungsberechtigungen verwendet hat, enthält dieses Feld die ID des Dienstprinzipals, der der App entspricht. Schreibgeschützt. |

## <a name="maximum-length-of-subscription-per-resource-type"></a>Maximale Abonnementdauer pro Ressourcentyp

| Ressource            | Maximal zulässige Ablaufzeit  |
|:--------------------|:-------------------------|
| Mail                | 4230 Minuten (unter 3 Tage)    |
| Kalender            | 4230 Minuten (unter 3 Tage)    |
| Kontakte            | 4230 Minuten (unter 3 Tage)    |
| Gruppenunterhaltungen | 4230 Minuten (unter 3 Tage)    |
| Laufwerkstammelemente    | 4230 Minuten (unter 3 Tage)    |
| Sicherheitswarnungen     | 43200 Minuten (unter 30 Tage)  |

> **Hinweis:** Vorhandene Anwendungen und neue Anwendungen sollten den unterstützten Wert nicht überschreiten. In Zukunft schlagen alle Anforderungen zur Erstellung oder Verlängerung eines Abonnements, die über den Maximalwert hinausgehen, fehl.

## <a name="relationships"></a>Beziehungen

Keine

## <a name="methods"></a>Methoden

| Methode | Rückgabetyp | Beschreibung |
|:-------|:------------|:------------|
| [Create subscription](../api/subscription-post-subscriptions.md) | [Abonnement](subscription.md) | Abonniert eine Listener-Anwendung zum Empfangen von Benachrichtigungen, wenn Microsoft Graph-Daten geändert werden. |
| [Update subscription](../api/subscription-update.md) | [Abonnement](subscription.md) | Erneuert ein Abonnement durch Aktualisierung der Ablaufzeit. |
| [Abonnements auflisten](../api/subscription-list.md) | [subscription](subscription.md) | Listet aktive Abonnements auf. |
| [Abonnement abrufen](../api/subscription-get.md) | [Abonnement](subscription.md) | Dient zum Lesen der Eigenschaften und der Beziehungen des subscription-Objekts. |
| [Delete subscription](../api/subscription-delete.md) | Keine |Löscht ein subscription-Objekt. |

[contact]: ./contact.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[alert]: ./alert.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
