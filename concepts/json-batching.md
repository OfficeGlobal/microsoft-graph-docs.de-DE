---
title: Kombinieren von mehreren Anforderungen in einem HTTP-Aufruf unter Verwendung der JSON-Batchverarbeitung
description: 'Die JSON-Batchverarbeitung ermöglicht es Ihnen, Ihre Anwendung durch Kombinieren von mehreren Anforderungen in einem einzigen JSON-Objekt zu optimieren. Ein Client möchte z. B. eine Ansicht aus nicht verbundenen Daten wie den folgenden zusammenstellen:'
author: piotrci
localization_priority: Priority
ms.openlocfilehash: f36cc1c8e8ccc016078eab52c4c7f3874892d000
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885183"
---
# <a name="combine-multiple-requests-in-one-http-call-using-json-batching"></a>Kombinieren von mehreren Anforderungen in einem HTTP-Aufruf unter Verwendung der JSON-Batchverarbeitung

Die JSON-Batchverarbeitung ermöglicht es Ihnen, Ihre Anwendung durch Kombinieren von mehreren Anforderungen in einem einzigen JSON-Objekt zu optimieren. Ein Client möchte z. B. eine Ansicht aus nicht verbundenen Daten wie den folgenden zusammenstellen:

1. Ein in OneDrive gespeichertes Bild
2. Eine Liste von Planner-Aufgaben
3. Der Kalender für eine Gruppe

Indem Sie diese drei einzelnen Anforderungen in einer einzigen Batchanforderung kombinieren, können Sie die Netzwerklatenz der Anwendung erheblich reduzieren.

## <a name="first-json-batch-request"></a>Erste JSON-Batchanforderung

Zunächst erstellen Sie die JSON-Batchanforderung für das vorherige Beispiel. In diesem Szenario sind die einzelnen Anforderungen in keiner Weise voneinander abhängig und können daher in beliebiger Reihenfolge in der Batchanforderung platziert werden.

```http
POST https://graph.microsoft.com/v1.0/$batch
Accept: application/json
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "id": "1",
      "method": "GET",
      "url": "/me/drive/root:/{file}:/content"
    },
    {
      "id": "2",
      "method": "GET",
      "url": "/me/planner/tasks"
    },
    {
      "id": "3",
      "method": "GET",
      "url": "/groups/{id}/events"
    },
    {
      "id": "4",
      "url": "/me",
      "method": "PATCH",
      "body": {
        "city" : "Redmond"
      },
      "headers": {
        "Content-Type": "application/json"
      }
    }
  ]
}
```

Antworten auf die zum Batch zusammengefassten Anforderungen werden möglicherweise in einer anderen Reihenfolge angezeigt. Die `id`-Eigenschaft kann verwendet werden, um einzelne Anforderungen und Antworten zu korrelieren.

```http
200 OK
Content-Type: application/json
```

```json
{
  "responses": [
    {
      "id": "1",
      "status": 302,
      "headers": {
        "location": "https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi"
      }
    },
    {
      "id": "3",
      "status": 401,
      "body": {
        "error": {
          "code": "Forbidden",
          "message": "..."
        }
      }
    },
    {
      "id": "2",
      "status": 200,
      "body": {
        "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.plannerTask)",
        "value": []
      }
    },
    {
      "id": "4",
      "status": 204,
      "body": null
    }
  ]
}
```

## <a name="request-format"></a>Anforderungsformat

Batchanforderungen werden immer mithilfe von `POST` an den Endpunkt `/$batch` gesendet.

Der Textkörper einer JSON-Batchanforderung besteht aus einem einzelnen JSON-Objekt mit einer erforderlichen Eigenschaft: `requests`. Die `requests`-Eigenschaft ist ein Array von einzelnen Anforderungen. Für jede einzelne Anforderung sind die Eigenschaften `id`, `method` und `url` erforderlich.

Die `id`-Eigenschaft dient in erster Linie als Korrelationswert zum Zuordnen einzelner Antworten zu Anforderungen. Dadurch kann der Server Anforderungen im Batch in der effizientesten Reihenfolge verarbeiten.

Die Eigenschaften `method` und `url` sind genau das, was Sie am Anfang jeder HTTP-Anforderung sehen. Die Methode ist die HTTP-Methode, und die URL ist die Ressourcen-URL, an die die einzelne Anforderung normalerweise gesendet wird.

Einzelne Anforderungen können optional auch eine `headers`- und eine `body`-Eigenschaft enthalten. Beide Eigenschaften sind in der Regel JSON-Objekte, wie im vorherigen Beispiel gezeigt. In einigen Fällen ist die `body`-Eigenschaft möglicherweise ein base64-codierter URL-Wert anstelle eines JSON Objekts, beispielsweise wenn der Textkörper ein Bild ist. Wenn ein `body` in der Anforderung enthalten ist, muss das `headers`-Objekt einen Wert für `Content-Type` enthalten.

## <a name="response-format"></a>Antwortformat

Das Antwortformat für JSON-Batchanforderungen ähnelt dem Anforderungsformat. Die wichtigsten Unterschiede sind folgende:

* Die Eigenschaft im JSON-Hauptobjekt heißt `responses`, im Gegensatz zu `requests`.
* Einzelne Antworten werden möglicherweise in einer anderen Reihenfolge angezeigt als die Anforderungen.
* Anstelle von `method` und `url` verfügen einzelne Antworten über eine `status`-Eigenschaft. Der Wert von `status` ist eine Zahl, die den HTTP-Statuscode darstellt.

Der Statuscode einer Batchantwort lautet in der Regel `200` oder `400`. Wenn die Batchanforderung selbst falsch formatiert ist, lautet der Statuscode `400`. Wenn die Batchanforderung analysierbar ist, lautet der Statuscode `200`. Ein Statuscode `200` in der Batchantwort besagt nicht, dass die einzelnen Anforderungen innerhalb des Batches erfolgreich waren. Aus diesem Grund hat jede einzelne Antwort in der `responses`-Eigenschaft einen Statuscode.

Zusätzlich zur `responses`-Eigenschaft kann auch eine `nextLink`-Eigenschaft in der Batchantwort enthalten sein. Diese ermöglicht es Microsoft Graph, eine Batchantwort zurückzugeben, sobald eine der einzelnen Anforderungen abgeschlossen ist. Um sicherzustellen, dass alle einzelnen Antworten empfangen wurden, folgen Sie weiterhin dem `nextLink`, solange er vorhanden ist.

## <a name="sequencing-requests-with-the-dependson-property"></a>Sequenzieren von Anforderungen mit der dependsOn-Eigenschaft

Einzelne Anforderungen können mithilfe der `dependsOn`-Eigenschaft in einer bestimmten Reihenfolge ausgeführt werden. Diese Eigenschaft ist ein Array von Zeichenfolgen, die auf die `id` einer anderen einzelnen Anforderung verweisen. Aus diesem Grund müssen die Werte für `id` eindeutig sein. In der folgenden Anforderung gibt der Client beispielsweise an, dass die Anforderungen 1 und 3 zuerst ausgeführt werden sollen, dann Anforderung 2 und dann Anforderung 4.

```json
{
  "requests": [
    {
      "id": "1",
      "method": "GET",
      "url": "..."
    },
    {
      "id": "2",
      "dependsOn": [ "1" ],
      "method": "GET",
      "url": "..."
    },
    {
      "id": "3",
      "method": "GET",
      "url": "..."
    },
    {
      "id": "4",
      "dependsOn": [ "2" ],
      "method": "GET",
      "url": "..."
    }
  ]
}
```

Wenn beim Ausführen einer einzelnen Anforderung ein Fehler auftritt, tritt bei allen Anforderungen, die von der betreffenden Anforderung abhängen, ein Fehler mit dem Statuscode `424` (Abhängigkeitsfehler) auf.

## <a name="bypassing-url-length-limitations-with-batching"></a>Umgehen von URL-Längenbeschränkungen durch Batchverarbeitung

Ein weiterer Anwendungsfall für die JSON-Batchverarbeitung ist die Umgehung von URL-Längenbeschränkungen. Im Fall einer komplexen Filterklausel kann es passieren, dass die URL die in Browsern oder anderen HTTP-Clients integrierten Längenbeschränkungen nicht einhält. Sie können die JSON-Batchverarbeitung als Problemumgehung zum Ausführen dieser Anforderungen verwenden, da die lange URL einfach Teil der Anforderungsnutzlast wird.

## <a name="known-issues"></a>Bekannte Probleme

Eine Liste von aktuellen Beschränkungen im Zusammenhang mit der Batchverarbeitung finden Sie unter [bekannte Probleme][batching-known-issues].

[batching-known-issues]: known-issues.md#json-batching
[odata-4.01-json]: https://www.oasis-open.org/committees/download.php/60365/odata-json-format-v4.01-wd02-2017-03-24.docx


## <a name="see-also"></a>Siehe auch

Weitere Informationen zum Format von JSON-Batchanforderungen/-antworten finden Sie in der [OData JSON-Formatspezifikation Version 4.01][odata-4.01-json], Abschnitt 18. Beachten Sie, dass diese Spezifikation derzeit eine Entwurfsversion ist, eine Änderung wird jedoch nicht erwartet.

