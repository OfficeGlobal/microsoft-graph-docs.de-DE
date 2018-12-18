---
title: Abrufen von unveränderlichen Bezeichnern für Outlook-Ressourcen
description: 'Outlook-Elemente (Nachrichten, Ereignisse, Kontakte, Aufgaben) haben ein interessantes Verhalten, das Sie vermutlich entweder noch nie bemerkt haben oder das bei Ihnen erhebliche Frustration ausgelöst hat: ihre IDs ändern sich. Das geschieht nicht oft, nur wenn das Element verschoben wird, es kann aber für Apps, die IDs zwecks späterer Verwendung offline speichern, zu echten Problemen führen. Unveränderliche Bezeichner ermöglichen Ihrer Anwendung das Abrufen einer ID, die sich über die gesamte Lebensdauer des Elements nicht ändert.'
author: angelgolfer-ms
ms.openlocfilehash: 34d88ed2cbc39902f1240757367beb112cc007b4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315197"
---
# <a name="get-immutable-identifiers-for-outlook-resources"></a>Abrufen von unveränderlichen Bezeichnern für Outlook-Ressourcen

Outlook-Elemente (Nachrichten, Ereignisse, Kontakte, Aufgaben) haben ein interessantes Verhalten, das Sie vermutlich entweder noch nie bemerkt haben oder das bei Ihnen erhebliche Frustration ausgelöst hat: ihre IDs ändern sich. Das geschieht nicht oft, nur wenn das Element verschoben wird, es kann aber für Apps, die IDs zwecks späterer Verwendung offline speichern, zu echten Problemen führen. Unveränderliche Bezeichner ermöglichen Ihrer Anwendung das Abrufen einer ID, die sich über die gesamte Lebensdauer des Elements nicht ändert.

> **Wichtig:** Unveränderliche Bezeichner sind nur in der /beta-Version von Microsoft Graph verfügbar.

## <a name="how-it-works"></a>Funktionsweise

Unveränderliche IDs stellen ein optionales Feature von Microsoft Graph dar. Um sich dafür zu entscheiden, muss Ihre Anwendung einen zusätzlichen HTTP-Header in Ihren API-Anforderungen senden:

```http
Prefer: IdType="ImmutableId"
```

Dieser Header gilt nur für die Anforderung, in der er enthalten ist. Wenn Sie immer unveränderliche IDs verwenden möchten, müssen Sie diesen Header in jede API-Anforderung aufnehmen.

## <a name="lifetime-of-immutable-ids"></a>Lebensdauer unveränderlicher IDs

Die unveränderliche ID eines Elements ändert sich nicht, solange das Element im gleichen Postfach verbleibt. Das bedeutet, dass sich die unveränderliche ID NICHT ändert, wenn das Element in einen anderen Ordner im Postfach verschoben wird. Die unveränderliche ID ändert sich aber unter diesen Umständen:

- Der Benutzer verschiebt das Element in ein Archivpostfach
- Der Benutzer exportiert das Element (in eine PST-Datei, als MSG-Datei usw.) und importiert es anschließend wieder in sein Postfach

## <a name="items-that-support-immutable-id"></a>Elemente, die unveränderliche IDs unterstützen.

Die folgenden Elemente unterstützen unveränderliche IDs:

- [Ressourcentyp Nachricht](/graph/api/resources/message?view=graph-rest-beta)
- [Ressourcentyp Anlage](/graph/api/resources/attachment?view=graph-rest-beta)
- [Ressourcentyp Ereignis](/graph/api/resources/event?view=graph-rest-beta)
- [Ressourcentyp eventMessage](/graph/api/resources/eventmessage?view=graph-rest-beta)
- [Ressourcentyp Kontakt](/graph/api/resources/contact?view=graph-rest-beta)
- [Ressourcentyp outlookTask](/graph/api/resources/outlooktask?view=graph-rest-beta)

Containertypen (mailFolder, calendar usw.) unterstützen keine unveränderlichen IDs, aber ihre regulären IDs stellen bereits Konstanten dar.

## <a name="immutable-id-with-change-notifications"></a>Unveränderliche IDs mit Änderungsbenachrichtigungen

Sie können festlegen, dass Microsoft Graph unveränderliche IDs in Änderungsbenachrichtigungen sendet, indem Sie den Header `Prefer: IdType="ImmutableId"` beim [Erstellen eines Abonnements](/graph/api/subscription-post-subscriptions?view=graph-rest-beta) einschließen. Vorhandene Abonnements, die ohne den Header erstellt wurden, verwenden weiterhin das ID-Standardformat. Um vorhandene IDs auf die Verwendung von unveränderlichen IDs umzustellen, müssen Sie sie löschen und unter Verwendung des Headers neu erstellen.

## <a name="immutable-id-with-delta-query"></a>Unveränderliche IDs mit Delta-Abfragen

Sie können festlegen, dass Microsoft Graph für unterstützte Ressourcentypen unveränderliche IDs in [Antworten auf Delta-Abfragen](delta-query-overview.md) zurückgibt, indem Sie den Header `Prefer: IdType="ImmutableId"` einschließen. Die von Delta-Abfragen zurückgegebenen Werte `nextLink` und `deltaLink` sind mit beiden ID-Formaten kompatibel, daher muss Ihre Anwendung nicht neu synchronisiert werden, um unveränderliche IDs zu nutzen. Sie können den Header verwenden, um von jetzt an unveränderliche IDs abzurufen, und Sie können [den Speicher Ihrer App](#updating-existing-data) separat aktualisieren.

## <a name="updating-existing-data"></a>Aktualisieren vorhandener Daten

Wenn Sie bereits über eine Datenbank verfügen, die mit Tausenden regulärer IDs gefüllt ist, können Sie diese IDs mithilfe der Funktion [translateExchangeIds](/graph/api/user-translateexchangeids?view=graph-rest-beta) in das unveränderliche Format konvertieren. Sie können ein Array von bis zu 1.000 IDs angeben, die in ein Zielformat übersetzt werden sollen.

> **Hinweis:** `translateExchangeIds` kann auch für die Migration von Exchange-Webdiensten nach Microsoft Graph verwendet werden.

### <a name="example"></a>Beispiel

Im folgenden Beispiel wird eine normale Graph-ID in eine unveränderliche Graph-ID übersetzt.

#### <a name="request"></a>Anforderung

```http
POST https://graph.microsoft.com/beta/me/translateExchangeIds

{
  "inputIds" :
  [
    "AQMkAGM2…"
  ],
  "targetIdType" : "restImmutableEntryId",
  "sourceIdType" : "restId"
}
```

#### <a name="response"></a>Antwort

```http
HTTP 200 OK

{
  "value": [
    {
      "targetId": "AAkALgAA...",
      "sourceId": "AQMkAGM2..."
    }
  ]
}
```