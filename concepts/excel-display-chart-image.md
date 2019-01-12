---
title: Anzeigen eines Diagrammbilds in Excel mithilfe von Microsoft Graph
description: Wenn Sie einen GET-Vorgang zum Abrufen eines Diagrammbilds ausführen, gibt die Excel-API das Bild als Base-64-Zeichenfolge zurück.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 5cdf5522ccd0a72798ee62211e9221cf2ea9cd53
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946371"
---
# <a name="display-a-chart-image-in-excel-with-microsoft-graph"></a><span data-ttu-id="06131-103">Anzeigen eines Diagrammbilds in Excel mithilfe von Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="06131-103">Display a chart image in Excel with Microsoft Graph</span></span>

<span data-ttu-id="06131-104">Wenn Sie einen [GET-Vorgang zum Abrufen eines Diagrammbilds](/api-reference/v1.0/api/chart-image.md) ausführen, gibt die Excel-API gibt das Bild als Base-64-Zeichenfolge zurück.</span><span class="sxs-lookup"><span data-stu-id="06131-104">When you perform a [GET operation to retrieve a chart image](/api-reference/v1.0/api/chart-image.md), the Excel API returns the image as a base-64 string.</span></span>

<span data-ttu-id="06131-105">Sie können die Base64-Zeichenfolge innerhalb eines HTML-Bild-Tags anzeigen: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span><span class="sxs-lookup"><span data-stu-id="06131-105">You can display the base-64 string inside an HTML image tag: `<img src="data:image/png;base64,{base-64 chart image string}/>`.</span></span>

<span data-ttu-id="06131-106">Verwenden Sie für das Standardverhalten `Image(width=0,height=0,fittingMode='fit')`.</span><span class="sxs-lookup"><span data-stu-id="06131-106">For default behavior, use `Image(width=0,height=0,fittingMode='fit')`.</span></span> <span data-ttu-id="06131-107">Hier ist ein Beispiel für ein Diagrammbild, das mit den standardmäßigen Parametern zurückgegeben wird.</span><span class="sxs-lookup"><span data-stu-id="06131-107">Here is an example of a chart image returned with the default parameters.</span></span>

![Excel-Diagrammbild mit Standardhöhe und -breite.](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/GetChart-default.png)

<span data-ttu-id="06131-109">Wenn Sie die Anzeige des Bilds anpassen möchten, geben Sie eine Höhe, Breite und einen Anpassmodus an.</span><span class="sxs-lookup"><span data-stu-id="06131-109">If you want to customize the display of the image, specify a height, width, and a fitting mode.</span></span> <span data-ttu-id="06131-110">So sieht dasselbe Diagrammbild aus, wenn Sie es mit diesen Parametern abrufen: `Image(width=500,height=500,fittingMode='Fill')`.</span><span class="sxs-lookup"><span data-stu-id="06131-110">Here is what the same chart image looks like if you retrieve it with these parameters: `Image(width=500,height=500,fittingMode='Fill')`.</span></span>

## <a name="see-also"></a><span data-ttu-id="06131-111">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="06131-111">See also</span></span>

* [<span data-ttu-id="06131-112">Verwalten von Sitzungen in Excel mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="06131-112">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="06131-113">Schreiben in eine Excel-Arbeitsmappe mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="06131-113">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="06131-114">Verwenden von Arbeitsmappenfunktionen in Excel mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="06131-114">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="06131-115">Aktualisieren eines Bereichsformats in Excel mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="06131-115">Update a range’s format in Excel with Microsoft Graph</span></span>](excel-update-range-format.md)
* [<span data-ttu-id="06131-116">Verwenden der Excel-REST-API</span><span class="sxs-lookup"><span data-stu-id="06131-116">Use the Excel REST API</span></span>](/graph/api/resources/excel?view=graph-rest-1.0)
