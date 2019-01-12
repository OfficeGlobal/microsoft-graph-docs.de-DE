---
title: Ressourcentyp Aktivität
description: Stellt eine einzelne Aktivität in einer app - beispielsweise ein TV-Programm, ein Dokument oder eine aktuelle Kampagne in einem Video Spiel. Wenn ein Benutzer Aktivität einbezieht, wird das Engagement als Element Verlauf erfasst, das die Start- und Endzeit für diese Aktivität angibt. Wie der Benutzer Aktivität über einen Zeitraum erneut einbezieht, werden mehrere Verlaufselemente für eine einzelne Benutzeraktivität aufgezeichnet.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 7a9000de339bc5d44fcbf2d282237caef85e076f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939294"
---
# <a name="activity-resource-type"></a>Ressourcentyp Aktivität

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt eine einzelne Aktivität in einer app - beispielsweise ein TV-Programm, ein Dokument oder eine aktuelle Kampagne in einem Video Spiel. Wenn ein Benutzer Aktivität einbezieht, wird das Engagement als [Historienelement](projectrome-historyitem.md) erfasst, das die Start- und Endzeit für diese Aktivität angibt. Wie der Benutzer Aktivität über einen Zeitraum erneut einbezieht, werden mehrere Verlaufselemente für eine einzelne Benutzeraktivität aufgezeichnet.

Sie können Aktivitäten in Microsoft Graph, damit Benutzer zurückerhalten, was sie für mehrere Geräte in ihrer app getan haben. Aktivitäten, die Ihre app erstellt auf Geräten alle Benutzer angezeigt werden, und für Benutzer als deep-Links auf bestimmte Inhalte Ihrer App verfügbar gemacht. Sie können bestimmte Inhalte Ihrer App als Ziel Ausdrücken, die in Windows und den Zugriff auf iOS und Android-Geräte über Cortana Benachrichtigungen präsentiert wird.

Da jeder app anders ist, ist es Ihnen zu verstehen, die beste Möglichkeit zum Zuordnen von Aktionen innerhalb der Anwendung auf die Benutzeraktivitäten, die in Cortana und Zeitachse angezeigt wird. Beispielsweise Spiele möglicherweise eine Aktivität für jede Kampagne erstellen, Erstellen von apps Dokument möglicherweise eine Aktivität für jedes Dokument erstellen und Line-of-Business-apps möglicherweise eine Aktivität für jeden Workflow erstellen.

Ihre Benutzeraktivitäten werden in Cortana und Windows-Zeitachsen Benutzererlebnis präsentiert werden die konzentriert sich eine Erhöhung Benutzer Produktivität und Effizienz durch Unterstützung bei der ähnliche Inhalte zu erhalten, die sie in der Vergangenheit gearbeitet.

## <a name="methods"></a>Methoden

|Methode | Rückgabetyp | Beschreibung|
|:------|:------------|:-----------|
|[Erstellen oder Ersetzen Sie die Aktivität](../api/projectrome-put-activity.md) | [Aktivität](projectrome-activity.md) |Erstellt oder eine vorhandene Aktivität (Upsert) ersetzt. Die AppActivityId URL-sichere (alle Zeichen mit Ausnahme der RFC 2396 nicht reservierte Zeichen in ihre hexadezimale Darstellung konvertiert werden müssen) sein muss, aber die ursprünglichen AppActivityId benötigt keinen URL-sicheren. |
|[Aktivität löschen](../api/projectrome-delete-activity.md) | Kein Inhalt | Löscht die angegebene Aktivität für diesen Benutzer von Ihrer app aus.|
|[Abrufen von Aktivitäten](../api/projectrome-get-activities.md) | Auflistung von [Aktivitäten](projectrome-activity.md) | Ruft die Aktivitäten für Ihre app für einen bestimmten Benutzer ab.|
|[Aktuelle Aktivitäten abrufen](../api/projectrome-get-recent-activities.md) | Auflistung von [Aktivitäten](projectrome-activity.md) | Ruft die neuesten Aktivitäten für Ihre app für einen bestimmten Benutzer, sortiert und basierend auf der am häufigsten zuletzt erstellte oder aktualisierte [HistoryItems](projectrome-historyitem.md)ab.|

## <a name="properties"></a>Eigenschaften

|Name | Typ | Beschreibung|
|:----|:-----|:-----------|
|userTimezone | Zeichenfolge | Optional. Die Zeitzone, in der das Gerät des Benutzers verwendet, um die Aktivität generieren zum Zeitpunkt der Erstellung Aktivität gefunden wurde; Werte, die zur Unterstützung der plattformübergreifende Darstellung als Olson-IDs angegeben.|
|createdDateTime | DateTimeOffset | Vom Server festgelegt. DateTime in UTC, wenn das Objekt auf dem Server erstellt wurde. |
|lastModifiedDateTime | DateTimeOffset | Vom Server festgelegt. DateTime in UTC, wenn das Objekt auf dem Server geändert wurde. |
|id | Zeichenfolge | Server generierte ID für die URL-Adressen verwendet.|
|appActivityId | Zeichenfolge | Erforderlich. Die eindeutige Aktivitäts-ID im Kontext der app - vom Anrufer und unveränderlich danach bereitgestellt.|
|activitySourceHost | Zeichenfolge | Erforderlich. URL für die Domäne, die die Zuordnung plattformübergreifende Identität für die app darstellt. Zuordnung ist gespeicherte entweder als JSON-Datei für die Domäne gehostet oder über Windows-Entwicklungscenter konfigurierbar. Die Datei JSON heißt Cross-Plattform-app-IDs und befindet sich am Stamm der Domäne HTTPS, entweder auf die Domäne der obersten Ebene oder enthalten eine Sub-Domäne. Zum Beispiel: https://contoso.com oder https://myapp.contoso.com, jedoch NICHT https://myapp.contoso.com/somepath. Sie müssen einen eindeutigen Dateinamen und Domäne (oder Sub Domäne) pro plattformübergreifende app-Identität verfügen. Beispielsweise ist eine separate Datei und eine Domäne für Word und PowerPoint erforderlich.|
|appDisplayName | Zeichenfolge | Optional. Kurze Beschreibung der app verwendet, um die Aktivität für die Verwendung in Fällen generiert werden, wenn die app nicht auf das lokale Gerät des Benutzers installiert ist.|
|activationUrl | Zeichenfolge | Erforderlich. So starten Sie die Aktivität im systemeigenen optimal dargestellt durch die AppId verwendete URL. Starten eine webbasierten app möglicherweise, wenn keine systemeigene Anwendung vorhanden ist.|
|fallbackUrl | Zeichenfolge | Optional. URL zum Starten der Aktivitätsfeeds in einer webbasierten-app verwendet werden, falls verfügbar.|
|contentUrl | Zeichenfolge | Optional. Verwendet den Fall, dass der Inhalt außerhalb einer systemeigenen oder webbasierte app-Benutzeroberfläche (beispielsweise einen Zeiger auf ein Element in einem RSS-Feed) gerendert werden kann.|
|visualElements| [visualInfo](../resources/projectrome-visualinfo.md) | Erforderlich. Das Objekt mit Informationen zum Rendern der Aktivitätsfeeds in die UX.|
|ContentInfo dar | Nicht typisierte JSON-Objekt | Optional. Eine benutzerdefinierte Datenelement - JSON-LD extensible Beschreibung des Inhalts entsprechend [schema.org](https://schema.org) Syntax.|
|expirationDateTime | DateTimeOffset | Vom Server festgelegt. DateTime in UTC, wenn das Objekt auf dem Server abgelaufen.|
|status | EnumType | Vom Server festgelegt. Einen Statuscode verwendet, um gültige Objekte identifizieren. Werte: aktiv, aktualisiert, gelöscht, ignoriert.|

## <a name="relationships"></a>Beziehungen

|Beziehung | Typ | Beschreibung|
|:------------|:-----|:-----------|
|historyItems| [HistoryItem](../resources/projectrome-historyitem.md) -Auflistung | Optional. NavigationProperty/Kapselung; Navigationseigenschaft der Aktivität HistoryItems.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "appDisplayName",
    "fallbackUrl",
    "contentUrl",
    "contentInfo",
    "visualElements",
    "historyItems"
  ],
  "@odata.type": "microsoft.graph.activity"
}-->

```json
{
    "appActivityId": "String",
    "activitySourceHost": "String (host name/domain/URL)",
    "userTimezone": "String",
    "appDisplayName": "String",
    "activationUrl": "String (URL)",
    "contentUrl": "String (URL)",
    "fallbackUrl": "String (URL)",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "expirationDateTime": "DateTimeOffset",
    "id": "String",
    "status": "EnumType",
    "contentInfo": { "@data.type": "microsoft.graph.Json" },
    "visualElements": { "@data.type": "microsoft.graph.visualInfo" },
    "historyItems": [{ "@odata.type": "microsoft.graph.historyItem" }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "activity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
