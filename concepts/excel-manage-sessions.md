---
title: Verwalten von Sitzungen und Persistenz in Excel mit Microsoft Graph
description: Wenn Ihre Anwendung mehr als nur ein oder zwei Aufrufe an die Excel-API durchführen muss, müssen Sie eine Sitzung erstellen und die Sitzungs-ID mit jeder Anforderung übergeben. Indem Sie eine Sitzungs-ID in die Anforderungen einschließen, wird sichergestellt, dass Sie die Excel-API auf möglichst effiziente Weise verwenden.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 151119a2a2861b64db126c8f49d0b916a6f563e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921689"
---
# <a name="manage-sessions-and-persistence-in-excel-with-microsoft-graph"></a>Verwalten von Sitzungen und Persistenz in Excel mit Microsoft Graph

Wenn Ihre Anwendung mehr als nur ein oder zwei Aufrufe an die Excel-API durchführen muss, müssen Sie eine Sitzung erstellen und die Sitzungs-ID mit jeder Anforderung übergeben. Indem Sie eine Sitzungs-ID in die Anforderungen einschließen, wird sichergestellt, dass Sie die Excel-API auf möglichst effiziente Weise verwenden.

Excel-APIs können in einem der drei folgenden Modi aufgerufen werden:

1. **Beständige Sitzung**: Alle an der Arbeitsmappe vorgenommenen Änderungen werden gespeichert (beständig gemacht). Dies ist die effizienteste und leistungsfähigste Möglichkeit zur Verwendung der Excel-API.
2. **Nicht beständige Sitzung**: Die von der API vorgenommenen Änderungen werden nicht am Quellspeicherort gespeichert. Stattdessen behält der Excel-Back-End-Server eine temporäre Kopie der Datei bei, welche die während dieser API-Sitzung vorgenommenen Änderungen enthält. Wenn die Excel-Sitzung abläuft, gehen die Änderungen verloren. Dieser Modus eignet sich für Apps, die Analysen durchführen oder die Ergebnisse einer Berechnung oder eines Diagrammbilds abrufen, aber nicht den Dokumentstatus betreffen.
3. **Sitzungslos**: Die API-Aufrufe übergeben keine Sitzungs-ID. Die Excel-Server müssen die Serverkopie der Arbeitsmappe für jeden Vorgang suchen. Dies ist keine effiziente Methode zum Aufrufen der Excel-API. Sie eignet sich jedoch für bestimmte Arten von isolierten Anforderungen.

Um die Sitzung in der API darzustellen, verwenden Sie den `workbook-session-id: {session-id}`-Header.

>**Hinweis:** Der Sitzungsheader ist für das Funktionieren einer Excel-API nicht erforderlich. Die Verwendung des Sitzungsheaders wird jedoch empfohlen, um die Leistung zu verbessern. Wenn Sie keinen Sitzungsheader verwenden, _werden_ die während des API-Aufrufs vorgenommenen Änderungen in der Datei gespeichert.  

## <a name="next-step"></a>Nächster Schritt
Informationen zum Erstellen und Verwenden von Sitzungen finden Sie unter [Erstellen von Sitzungsreferenzen](/graph/api/workbook-createsession?view=graph-rest-1.0).

## <a name="see-also"></a>Siehe auch
* [Schreiben in eine Excel-Arbeitsmappe mit Microsoft Graph](excel-write-to-workbook.md)
* [Verwenden von Arbeitsmappenfunktionen in Excel mit Microsoft Graph](excel-use-functions.md)
* [Aktualisieren eines Bereichsformats in Excel mit Microsoft Graph](excel-update-range-format.md)
* [Anzeigen eines Diagrammbilds in Excel mithilfe von Microsoft Graph](excel-display-chart-image.md)
* [Verwenden der Excel-REST-API](/graph/api/resources/excel?view=graph-rest-1.0)
