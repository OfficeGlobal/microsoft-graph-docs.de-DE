---
title: Ressourcentyp Abonnement
description: 'Ein Abonnement ermöglicht eine Client-app zum Empfangen von Benachrichtigungen zu Änderungen an Daten in Microsoft Graph. Abonnements werden derzeit für die folgenden Ressourcen aktiviert:'
ms.openlocfilehash: 5ece39954d661c6b7ef948d0ed7d514782fbceae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019839"
---
# <a name="subscription-resource-type"></a>Ressourcentyp Abonnement

Ein Abonnement ermöglicht eine Client-app zum Empfangen von Benachrichtigungen zu Änderungen an Daten in Microsoft Graph. Abonnements werden derzeit für die folgenden Ressourcen aktiviert:

- E-Mail-Nachrichten, Ereignisse und Kontakte aus Outlook.
- Unterhaltungen aus Office-Gruppen.
- Laufwerk Stammelemente aus OneDrive.
- Benutzer und Gruppen aus dem Azure Active Directory.
- Benachrichtigungen über die Microsoft Graph-Sicherheit API.

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
| changeType | string | Erforderlich. Gibt den Typ der Änderung in der abonnierten Ressource an, die eine Benachrichtigung auslöst. Unterstützte Werte sind: `created`, `updated`, `deleted`. Es können mehrere Werte mithilfe einer durch Trennzeichen getrennten Liste zusammen verwendet werden.<br><br>Hinweis: Laufwerk Root Element Benachrichtigungen unterstützen nur die `updated` ChangeType. Unterstützung von Benutzer- und Benachrichtigungen `updated` und `deleted` ChangeType.|
| notificationUrl | string | Erforderlich. Die URL des Endpunkts, die Benachrichtigungen erhalten werden. Diese URL muss nutzen Sie die HTTPS Protokoll. |
| resource | string | Erforderlich. Gibt die Ressource, die für Änderungen überwacht werden. Die base-URL nicht einschließen (`https://graph.microsoft.com/v1.0/`). |
| expirationDateTime | [dateTime](https://tools.ietf.org/html/rfc3339) | Erforderlich. Gibt Datum und Uhrzeit für das Ablaufen des Webhook-Abonnements an. Die Zeit wird in UTC angegeben und kann eine Dauer aus der Erstellung des Abonnements sein, die von der abonnierten Ressource abweicht.  In der folgenden Tabelle finden Sie die maximale Dauer unterstützter Abonnements. |
| clientState | string | Optional. Gibt den Wert der `clientState`-Eigenschaft an, die in jeder Benachrichtigung vom Dienst gesendet wird. Die Höchstlänge beträgt 128 Zeichen. Der Client kann prüfen, ob die Benachrichtigung vom Dienst stammt, indem er den Wert der mit dem Abonnement gesendeten `clientState`-Eigenschaft mit dem Wert der mit jeder Benachrichtigung empfangenen `clientState`-Eigenschaft vergleicht. |
| id | string | Eindeutige ID für das Abonnement. Schreibgeschützt. |
| applicationId | string | Bezeichner der Anwendung verwendet, um das Abonnement zu erstellen. Schreibgeschützt. |
| creatorId | string | Bezeichner des Benutzers oder der Dienstprinzipalnamen, die das Abonnement erstellt. Wenn die app verwendet Berechtigungen zum Erstellen des Abonnements delegiert, enthält dieses Feld die Id des angemeldeten Benutzers an, den die app im Auftrag von aufgerufen. Wenn die app Anwendungsberechtigungen verwendet wird, enthält dieses Feld die Id des Prinzipals Service für die app. Schreibgeschützt. |

## <a name="maximum-length-of-subscription-per-resource-type"></a>Maximale Abonnementdauer pro Ressourcentyp

| Ressource            | Maximal zulässige Ablaufzeit  |
|:--------------------|:-------------------------|
| Mail                | 4230 Minuten (unter 3 Tage)    |
| Kalender            | 4230 Minuten (unter 3 Tage)    |
| Kontakte            | 4230 Minuten (unter 3 Tage)    |
| Gruppenunterhaltungen | 4230 Minuten (unter 3 Tage)    |
| Laufwerkstammelemente    | 4230 Minuten (unter 3 Tage)    |
| Sicherheitshinweise     | 43200 Minuten (unter 30 Tage)  |

> **Hinweis:** Vorhandene Anwendungen und neuen Anwendungen sollte den unterstützten Wert nicht überschreiten. In der Zukunft fehl alle Anforderungen zum Erstellen oder erneuern Sie ein Abonnement über den Höchstwert hinaus.

## <a name="relationships"></a>Beziehungen

Keine

## <a name="methods"></a>Methoden

| Methode | Rückgabetyp | Beschreibung |
|:-------|:------------|:------------|
| [Create subscription](../api/subscription-post-subscriptions.md) | [Abonnement](subscription.md) | Abonniert eine Listener-Anwendung zum Empfangen von Benachrichtigungen, wenn Microsoft Graph-Daten geändert werden. |
| [Update subscription](../api/subscription-update.md) | [Abonnement](subscription.md) | Erneuert ein Abonnement durch Aktualisierung der Ablaufzeit. |
| [Liste von Abonnements](../api/subscription-list.md) | [subscription](subscription.md) | Listen aktiver Abonnements. |
| [Get subscription](../api/subscription-get.md) | [Abonnement](subscription.md) | Dient zum Lesen der Eigenschaften und der Beziehungen des subscription-Objekts. |
| [Delete subscription](../api/subscription-delete.md) | Keine |Löscht ein subscription-Objekt. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
