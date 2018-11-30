---
title: Verwenden Sie die Microsoft Graph-API für soziale Netzwerke Intelligence in einer app integrieren
description: Microsoft Graph unterstützt für soziale Netzwerke Gesten in sozialen Kontext des Benutzers und ermöglicht den Zugriff auf nützliche Personen und Daten in sozialen Netzwerken.
ms.openlocfilehash: b83c5ea08c6d66dc800f736717f50324f0e2b4b8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063968"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-intelligence-in-an-app"></a>Verwenden Sie die Microsoft Graph-API für soziale Netzwerke Intelligence in einer app integrieren

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Microsoft Graph unterstützt für soziale Netzwerke Gesten in sozialen Kontext des Benutzers und ermöglicht den Zugriff auf nützliche Personen und Daten in sozialen Netzwerken.

## <a name="aggregate-and-extract-specific-information-about-people"></a>Aggregieren Sie und extrahieren Sie spezifische Informationen zu Personen

Verwenden Sie die [Person](../resources/person.md) -Ressource und die API Personen aggregierte Informationen von einer Person über e-Mail, Kontakte und sozialen Netzwerken. Die Ergebnisse werden nach ihrer Relevanz basierend auf mehreren Kommunikation, Zusammenarbeit und Business Beziehungen sortiert. Die API können Sie durchsuchen, sortieren, auswählen, filtern oder suchen Sie nach Personen basierend auf den angegebenen Suchkriterien.

- [List people](../api/user-list-people.md)

## <a name="manage--mentions"></a>Verwalten von @ Erwähnungen

Aufrufen von einen Empfänger zu benachrichtigen und Aufmerksamkeit des Empfängers in einer Nachricht erhalten möchten, ist eine allgemeine für soziale Netzwerke Eingabeaktion.
Die Ressource [erwähnen](../resources/mention.md) und die API erwähnt bieten einen leicht Mechanismus, rufen Sie einen Empfänger in einer [Nachricht](../resources/message.md), erhalten alle Nachrichten, die in denen ein Benutzer benachrichtigt wird mithilfe der @ Erwähnung oder jede Erwähnung in einer Nachricht erhalten möchten.

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- Erstellen von erwähnungen in einer neuen Nachricht

  - [Erstellen und Senden von erwähnungen im Rahmen einer neuen Nachricht](../api/user-sendmail.md#request-2)
  - [Erstellen von erwähnungen als Teil eines e-Mail-Entwurfs](../api/user-post-messages.md#request-2)

- Abrufen von Informationen über erwähnungen in einer Nachricht

  - [Abrufen Sie aller Nachrichten im Postfach des angemeldeten Benutzers, in denen den Benutzer erwähnt](../api/user-list-messages.md#request-2)
  - [Abrufen von Details der einzelnen Erwähnung in einer Nachricht](../api/message-get.md#request-2)

- [Löschen der Vermerk](../api/message-delete.md#request-2) in einer Nachricht

## <a name="access-social-data-around-and-about-a-user"></a>Zugriff auf Daten in sozialen Netzwerken um sowie zu einem Benutzer

Office-Diagramm kapselt die Beziehungen zwischen verschiedenen Entitäten in Office 365. Verwenden Sie Office-Diagramm um soziale Einsichten in einzelne Benutzer über Office 365 abzurufen.

- Liste der Elemente [Trend, um](../api/insights-list-trending.md) einen Benutzer
- Auflisten von Waren, [Arbeiten mit](../api/user-list-people.md) Benutzern eines Benutzers
