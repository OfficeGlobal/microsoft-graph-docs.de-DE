---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Konvertieren in andere Formate
localization_priority: Normal
ms.openlocfilehash: d27420153a295eac9d3f880910d63bd701525427
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887437"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="81d41-102">Herunterladen einer Datei in einem anderen Format</span><span class="sxs-lookup"><span data-stu-id="81d41-102">Download a file in another format</span></span>

> <span data-ttu-id="81d41-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="81d41-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81d41-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="81d41-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="81d41-105">Mithilfe dieser API können Sie den Inhalt eines Elements in einem bestimmten Format abrufen.</span><span class="sxs-lookup"><span data-stu-id="81d41-105">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="81d41-106">Nicht jede Datei kann in sämtliche Formate konvertiert werden.</span><span class="sxs-lookup"><span data-stu-id="81d41-106">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="81d41-107">Wenn das Element im Originalformat herunterladen möchten, finden Sie unter [Herunterladen der Inhalt des Elements](driveitem-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="81d41-107">To download the item in its original format, see [download an item's contents](driveitem-get-content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81d41-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="81d41-108">Prerequisites</span></span>

<span data-ttu-id="81d41-109">Damit diese API aufgerufen werden kann, muss der Benutzer der Anwendung Lesezugriff auf die Datei gewährt haben, die von der App konvertiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="81d41-109">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="81d41-110">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="81d41-110">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="81d41-111">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="81d41-111">Query parameters</span></span>

| <span data-ttu-id="81d41-112">Parameter</span><span class="sxs-lookup"><span data-stu-id="81d41-112">Parameter</span></span>      | <span data-ttu-id="81d41-113">Typ</span><span class="sxs-lookup"><span data-stu-id="81d41-113">Type</span></span>  | <span data-ttu-id="81d41-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="81d41-114">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="81d41-115">_format_</span><span class="sxs-lookup"><span data-stu-id="81d41-115">_format_</span></span>  | <span data-ttu-id="81d41-116">string</span><span class="sxs-lookup"><span data-stu-id="81d41-116">string</span></span> | <span data-ttu-id="81d41-117">Hier geben Sie das Format an, in dem der Elementinhalt heruntergeladen werden soll.</span><span class="sxs-lookup"><span data-stu-id="81d41-117">Specify the format the item's content should be downloaded as.</span></span> |


<span data-ttu-id="81d41-118">Die folgenden Werte sind für den **Format** -Parameter gültig:</span><span class="sxs-lookup"><span data-stu-id="81d41-118">The following values are valid for the **format** parameter:</span></span>

| <span data-ttu-id="81d41-119">Wert</span><span class="sxs-lookup"><span data-stu-id="81d41-119">Value</span></span> | <span data-ttu-id="81d41-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="81d41-120">Description</span></span>                        | <span data-ttu-id="81d41-121">Unterstützte Quellerweiterungen</span><span class="sxs-lookup"><span data-stu-id="81d41-121">Supported source extensions</span></span>
|:------|:-----------------------------------|---------------------------------
| <span data-ttu-id="81d41-122">GLB</span><span class="sxs-lookup"><span data-stu-id="81d41-122">glb</span></span>   | <span data-ttu-id="81d41-123">Das Element konvertiert in GLB-format</span><span class="sxs-lookup"><span data-stu-id="81d41-123">Converts the item into GLB format</span></span>  | <span data-ttu-id="81d41-124">Cool, Fbx, Obj, Blatt, Stl, 3mf</span><span class="sxs-lookup"><span data-stu-id="81d41-124">cool, fbx, obj, ply, stl, 3mf</span></span>
| <span data-ttu-id="81d41-125">html</span><span class="sxs-lookup"><span data-stu-id="81d41-125">html</span></span>  | <span data-ttu-id="81d41-126">Das Element konvertiert in HTML-format</span><span class="sxs-lookup"><span data-stu-id="81d41-126">Converts the item into HTML format</span></span> | <span data-ttu-id="81d41-127">EML, Md, msg</span><span class="sxs-lookup"><span data-stu-id="81d41-127">eml, md, msg</span></span>
| <span data-ttu-id="81d41-128">JPG</span><span class="sxs-lookup"><span data-stu-id="81d41-128">jpg</span></span>   | <span data-ttu-id="81d41-129">Das Element konvertiert in das JPG-format</span><span class="sxs-lookup"><span data-stu-id="81d41-129">Converts the item into JPG format</span></span>  | <span data-ttu-id="81d41-130">3g 2, 3gp, 3gp2, 3gpp, 3mf, Ai, Arw, Asf, Avi, Bas, Bash, Bat, Bmp, c, Cbl, Cmd, Cool, Cpp, cr2, Crw, Cs, Css, Csv, übernehmen, dcm, dcm30, Dic, Dicm, Dicom, Dng, Doc, Docx, Dwg, Eml, Epi, Eps, Epsf, Epsi, Epub, Erf, Fbx, Fppx, Gif, Glb, h, hcp , Heic, Heif, Htm, html, Ico, Symbol, Java, Jfif, Jpeg, Jpg, Js, Json, Schlüssel, melden Sie sich, m2ts, m4a, m4v, Abzugsverteilung(en), Md, Mef, Mov, Film, MP3-, MP4 (engl.), mp4v, Mrw, msg, Mts, Nef, Nrw, Zahlen, Obj, Odp, Odt, Ogg, Orf, Seiten, Zusammenheften, Pdf, Pef, Php, Pict, pl, Blatt, Png, POT- , Potm, Potx, Pps, Ppsx, Ppsxm, ppt, Pptm, Pptx, Ps, ps1, Psb, Psd, hierhin, unformatiert, Rb, Rtf, rw1, rw2, sh skizzieren, Sql, sr2, Stl, Tif, Tiff, ts, Txt, Vb, Webm, Wma, Wmv, Xaml, Xbm, Xcf, xd, Xml, Xpm, Yaml, Yml</span><span class="sxs-lookup"><span data-stu-id="81d41-130">3g2, 3gp, 3gp2, 3gpp, 3mf, ai, arw, asf, avi, bas, bash, bat, bmp, c, cbl, cmd, cool, cpp, cr2, crw, cs, css, csv, cur, dcm, dcm30, dic, dicm, dicom, dng, doc, docx, dwg, eml, epi, eps, epsf, epsi, epub, erf, fbx, fppx, gif, glb, h, hcp, heic, heif, htm, html, ico, icon, java, jfif, jpeg, jpg, js, json, key, log, m2ts, m4a, m4v, markdown, md, mef, mov, movie, mp3, mp4, mp4v, mrw, msg, mts, nef, nrw, numbers, obj, odp, odt, ogg, orf, pages, pano, pdf, pef, php, pict, pl, ply, png, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, ps, ps1, psb, psd, py, raw, rb, rtf, rw1, rw2, sh, sketch, sql, sr2, stl, tif, tiff, ts, txt, vb, webm, wma, wmv, xaml, xbm, xcf, xd, xml, xpm, yaml, yml</span></span>
| <span data-ttu-id="81d41-131">PDF-Datei</span><span class="sxs-lookup"><span data-stu-id="81d41-131">pdf</span></span>   | <span data-ttu-id="81d41-132">Das Element konvertiert in das PDF-format</span><span class="sxs-lookup"><span data-stu-id="81d41-132">Converts the item into PDF format</span></span>  | <span data-ttu-id="81d41-133">Doc, Docx, Epub, Eml, Htm, html, Md, msg, Odp, ods, Odt, PPS-, PPSX-, ppt, Pptx, Rtf, Tif, Tiff, Xls, Xlsm, Xlsx</span><span class="sxs-lookup"><span data-stu-id="81d41-133">doc, docx, epub, eml, htm, html, md, msg, odp, ods, odt, pps, ppsx, ppt, pptx, rtf, tif, tiff, xls, xlsm, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="81d41-134">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="81d41-134">Optional request headers</span></span>

| <span data-ttu-id="81d41-135">Name</span><span class="sxs-lookup"><span data-stu-id="81d41-135">Name</span></span>            | <span data-ttu-id="81d41-136">Wert</span><span class="sxs-lookup"><span data-stu-id="81d41-136">Value</span></span>   | <span data-ttu-id="81d41-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="81d41-137">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="81d41-138">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="81d41-138">_if-none-match_</span></span> | <span data-ttu-id="81d41-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="81d41-139">String</span></span>  | <span data-ttu-id="81d41-140">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) mit dem aktuellen Tag in der Datei übereinstimmt, wird die Antwort `HTTP 304 Not Modified` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="81d41-140">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="81d41-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="81d41-141">Example</span></span>

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /drive/items/{item-id}/content?format={format}
```

## <a name="response"></a><span data-ttu-id="81d41-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="81d41-142">Response</span></span>

<span data-ttu-id="81d41-143">Die Methode gibt eine Antwort `302 Found` zurück, die auf eine vorab authentifizierte URL zum Download der konvertierten Datei umleitet.</span><span class="sxs-lookup"><span data-stu-id="81d41-143">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="81d41-144">Um die konvertierte Datei herunterladen zu können, muss die App den `Location`-Header in der Antwort aufrufen.</span><span class="sxs-lookup"><span data-stu-id="81d41-144">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="81d41-145">Vorab authentifizierte URLs sind nur für eine kurze Zeit gültig (einige Minuten) und erfordern für den Zugriff keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="81d41-145">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="81d41-146">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="81d41-146">Error responses</span></span>

<span data-ttu-id="81d41-147">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie im unter [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="81d41-147">See [Error Responses][error-response] for more information about how errors are returned.</span></span>

[error-response]: /graph/errors
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats"
} -->
