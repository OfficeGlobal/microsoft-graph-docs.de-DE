---
title: Subscription-Ressourcentyp
description: 'Ein Abonnement ermöglicht eine Client-app zum Empfangen von Benachrichtigungen zu Änderungen an Daten in Microsoft Graph. Abonnements werden derzeit für die folgenden Ressourcen aktiviert:'
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 265ea807330f833edf0d7b1f6a640e0a1f6f4634
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517267"
---
# <a name="subscription-resource-type"></a>Abonnementressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ein Abonnement ermöglicht eine Client-app zum Empfangen von Benachrichtigungen zu Änderungen an Daten in Microsoft Graph. Abonnements werden derzeit für die folgenden Ressourcen aktiviert:

- E-Mail, Ereignisse und Kontakte aus Outlook
- Unterhaltungen aus Office-Gruppen.
- Laufwerkstammelemente aus OneDrive
- Benutzer und Gruppen aus dem Azure Active Directory.
- Benachrichtigungen über die Microsoft Graph-Sicherheit API.

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
| changeType | string | Erforderlich. Gibt den Typ der Änderung in der abonnierten Ressource an, die eine Benachrichtigung auslöst. Unterstützte Werte sind: `created`, `updated`, `deleted`. Es können mehrere Werte mithilfe einer durch Trennzeichen getrennten Liste zusammen verwendet werden. <br><br>Hinweis: Laufwerk Root Element Benachrichtigungen unterstützen nur die `updated` ChangeType. Unterstützung von Benutzer- und Benachrichtigungen `updated` und `deleted` ChangeType. |
| notificationUrl | string | Erforderlich. Die URL des Endpunkts, die Benachrichtigungen erhalten werden. Diese URL muss nutzen Sie die HTTPS Protokoll. |
| resource | Die Ressource, auf die Sie zugreifen möchten. | Erforderlich. Gibt die Ressource, die für Änderungen überwacht werden. Die base-URL nicht einschließen (`https://graph.microsoft.com/beta/`). |
| expirationDateTime | DateTimeOffset | Erforderlich. Gibt Datum und Uhrzeit für das Ablaufen des Webhook-Abonnements an. Die Zeit wird in UTC angegeben und kann eine Dauer aus der Erstellung des Abonnements sein, die von der abonnierten Ressource abweicht.  In der folgenden Tabelle finden Sie die maximale Dauer unterstützter Abonnements. |
| clientState | string | Optional. Gibt den Wert der `clientState`-Eigenschaft an, die in jeder Benachrichtigung vom Dienst gesendet wird. Die maximale Länge ist 255 Zeichen. Der Client kann prüfen, ob die Benachrichtigung vom Dienst stammt, indem er den Wert der mit dem Abonnement gesendeten `clientState`-Eigenschaft mit dem Wert der mit jeder Benachrichtigung empfangenen `clientState`-Eigenschaft vergleicht. |
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
| Sicherheitswarnungen     | 43200 Minuten (unter 30 Tage)  |

> **Hinweis:** Vorhandene Anwendungen und neuen Anwendungen sollte den unterstützten Wert nicht überschreiten. In der Zukunft fehl alle Anforderungen zum Erstellen oder erneuern Sie ein Abonnement über den Höchstwert hinaus.

## <a name="relationships"></a>Beziehungen

Keine

## <a name="methods"></a>Methoden

| Methode | Rückgabetyp | Beschreibung |
|:-------|:------------|:------------|
| [Create subscription](../api/subscription-post-subscriptions.md) | [Abonnement](subscription.md) | Abonniert eine Listener-Anwendung zum Empfangen von Benachrichtigungen, wenn Microsoft Graph-Daten geändert werden. |
| [Update subscription](../api/subscription-update.md) | [subscription](subscription.md) | Erneuern eines Abonnements durch den Ablaufzeitpunkt aktualisieren. |
| [Liste von Abonnements](../api/subscription-list.md) | [subscription](subscription.md) | Listen aktiver Abonnements. |
| [Get subscription](../api/subscription-get.md) | [Abonnement](subscription.md) | Lesen Sie Eigenschaften und Beziehungen Abonnement-Objekts. |
| [Delete subscription](../api/subscription-delete.md) | Keine | Löscht ein Abonnementobjekt. |

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
