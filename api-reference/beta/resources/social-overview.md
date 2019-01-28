---
title: Verwenden der Microsoft Graph-API, um soziale Intelligenz in eine App zu integrieren
description: Microsoft Graph unterstützt soziale Gesten im sozialen Kontext des Benutzers und bietet Zugriff auf hilfreiche Personen- und soziale Daten.
localization_priority: Priority
author: simonhult
ms.prod: insights
ms.openlocfilehash: b5a89f46c8480fb90cd019e5b4fb370e0a6592bf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509595"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-intelligence-in-an-app"></a>Verwenden der Microsoft Graph-API, um soziale Intelligenz in eine App zu integrieren

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph unterstützt soziale Gesten im sozialen Kontext des Benutzers und bietet Zugriff auf hilfreiche Personen- und soziale Daten.

## <a name="aggregate-and-extract-specific-information-about-people"></a>Sammeln und Extrahieren von spezifischen Informationen zu Personen

Sie können die [person](../resources/person.md)-Ressource und die Personen-API zum Aggregieren von Informationen über eine Person aus E-Mails, Kontakten und sozialen Netzwerken verwenden. Die Ergebnisse werden nach ihrer Relevanz basierend auf Mustern bei der Kommunikation und Zusammenarbeit sowie auf Geschäftsbeziehungen sortiert. Mit der API können Sie Personen durchsuchen, sortieren, auswählen, filtern oder anhand eigener Kriterien nach Personen suchen.

- [Personen auflisten](../api/user-list-people.md)

## <a name="manage--mentions"></a>Verwalten von @-Erwähnungen

Es ist eine häufige soziale Geste, einen Empfänger zu benachrichtigen und die Aufmerksamkeit des Empfängers auf eine Nachricht zu lenken.
Die [mention](../resources/mention.md)-Ressource und die Erwähnungs-API bieten eine einfache Methode, um einen Empfänger in einer [Nachricht](../resources/message.md) zu benachrichtigen, alle Nachrichten mithilfe einer @-Erwähnung abzurufen, in denen ein Benutzer benachrichtigt wird, oder alle Erwähnungen in einer Nachricht abzurufen.

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- Erstellen von Erwähnungen in einer neuen Nachricht

  - [Erstellen und Senden von Erwähnungen als Teil einer neuen Nachricht](../api/user-sendmail.md#request-2)
  - [Erstellen von Erwähnungen als Teil eines E-Mail-Entwurfs](../api/user-post-messages.md#request-2)

- Abrufen von Informationen zu Erwähnungen in einer Nachricht

  - [Abrufen aller Nachrichten im Postfach des angemeldeten Benutzers, in denen der Benutzer erwähnt wird](../api/user-list-messages.md#request-2)
  - [Abrufen von Details zu den einzelnen Erwähnungen in einer Nachricht](../api/message-get.md#request-2)

- [Löschen einer Erwähnung](../api/message-delete.md#request-2) in einer Nachricht

## <a name="access-social-data-around-and-about-a-user"></a>Zugriff auf Daten aus sozialen Netzwerken und über einen Benutzer

Office Graph fasst die Beziehungen zwischen unterschiedlichen Entitäten in Office 365 zusammen. Verwenden Sie Office Graph, um soziale Einblicke zu einzelnen Benutzern in Office 365 zu erhalten.

- Auflisten der Elemente, die bei einem Benutzer [beliebt sind](../api/insights-list-trending.md)
- Auflisten der Benutzer, die [mit einem Benutzer gearbeitet haben](../api/user-list-people.md)
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/social-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
