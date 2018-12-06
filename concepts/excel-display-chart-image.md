---
title: Anzeigen eines Diagrammbilds in Excel mithilfe von Microsoft Graph
description: Wenn Sie einen GET-Vorgang zum Abrufen eines Diagrammbilds ausführen, gibt die Excel-API das Bild als Base-64-Zeichenfolge zurück.
ms.openlocfilehash: ae721547fca9a6fe835843544bf550c5fe222426
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092319"
---
# <a name="display-a-chart-image-in-excel-with-microsoft-graph"></a>Anzeigen eines Diagrammbilds in Excel mithilfe von Microsoft Graph

Wenn Sie einen [GET-Vorgang zum Abrufen eines Diagrammbilds](/api-reference/v1.0/api/chart-image.md) ausführen, gibt die Excel-API gibt das Bild als Base-64-Zeichenfolge zurück.

Sie können die Base64-Zeichenfolge innerhalb eines HTML-Bild-Tags anzeigen: `<img src="data:image/png;base64,{base-64 chart image string}/>`.

Verwenden Sie für das Standardverhalten `Image(width=0,height=0,fittingMode='fit')`. Hier ist ein Beispiel für ein Diagrammbild, das mit den standardmäßigen Parametern zurückgegeben wird.

![Excel-Diagrammbild mit Standardhöhe und -breite.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

Wenn Sie die Anzeige des Bilds anpassen möchten, geben Sie eine Höhe, Breite und einen Anpassmodus an. So sieht dasselbe Diagrammbild aus, wenn Sie es mit diesen Parametern abrufen: `Image(width=500,height=500,fittingMode='Fill')`.

## <a name="see-also"></a>Siehe auch

* [Verwalten von Sitzungen in Excel mit Microsoft Graph](excel-manage-sessions.md)
* [Schreiben in eine Excel-Arbeitsmappe mit Microsoft Graph](excel-write-to-workbook.md)
* [Verwenden von Arbeitsmappenfunktionen in Excel mit Microsoft Graph](excel-use-functions.md)
* [Aktualisieren eines Bereichsformats in Excel mit Microsoft Graph](excel-update-range-format.md)
* [Verwenden der Excel-REST-API](/graph/api/resources/excel?view=graph-rest-1.0)
