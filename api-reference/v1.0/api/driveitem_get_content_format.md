---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Konvertieren in andere Formate
ms.openlocfilehash: 7798905363217d366caabbdd9c82559f578c01aa
ms.sourcegitcommit: 809748ea18943f5fd1d99c4c65a9b964f39a5f25
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/08/2018
ms.locfileid: "23893298"
---
# <a name="download-a-file-in-another-format"></a><span data-ttu-id="4285c-102">Herunterladen einer Datei in einem anderen Format</span><span class="sxs-lookup"><span data-stu-id="4285c-102">Download a file in another format</span></span>

<span data-ttu-id="4285c-103">Mithilfe dieser API können Sie den Inhalt eines Elements in einem bestimmten Format abrufen.</span><span class="sxs-lookup"><span data-stu-id="4285c-103">Use this API to retrieve the contents of an item in a specific format.</span></span>
<span data-ttu-id="4285c-104">Nicht jede Datei kann in sämtliche Formate konvertiert werden.</span><span class="sxs-lookup"><span data-stu-id="4285c-104">Not all files can be converted into all formats.</span></span>

<span data-ttu-id="4285c-105">Wie Sie das Element in seinem ursprünglichen Format herunterladen können, erfahren Sie unter [Herunterladen des Inhalts von OneDrive-Elementen](driveitem_get_content.md).</span><span class="sxs-lookup"><span data-stu-id="4285c-105">To download the item in it's original format, see [download an item's contents](driveitem_get_content.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4285c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4285c-106">Prerequisites</span></span>

<span data-ttu-id="4285c-107">Damit diese API aufgerufen werden kann, muss der Benutzer der Anwendung Lesezugriff auf die Datei gewährt haben, die von der App konvertiert werden soll.</span><span class="sxs-lookup"><span data-stu-id="4285c-107">To call this API, the user must have granted the application read access to the file the app wishes to convert.</span></span>

## <a name="http-request"></a><span data-ttu-id="4285c-108">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4285c-108">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/items/{item-id}/content?format={format}
GET /drive/root:/{path and filename}:/content?format={format}
```

## <a name="query-parameters"></a><span data-ttu-id="4285c-109">Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4285c-109">Query parameters</span></span>

| <span data-ttu-id="4285c-110">Parameter</span><span class="sxs-lookup"><span data-stu-id="4285c-110">Parameter</span></span>      | <span data-ttu-id="4285c-111">Typ</span><span class="sxs-lookup"><span data-stu-id="4285c-111">Type</span></span>  | <span data-ttu-id="4285c-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4285c-112">Description</span></span>                                                    |
|:----------|:-------|:---------------------------------------------------------------|
| <span data-ttu-id="4285c-113">_Format_</span><span class="sxs-lookup"><span data-stu-id="4285c-113">_format_</span></span>  | <span data-ttu-id="4285c-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4285c-114">string</span></span> | <span data-ttu-id="4285c-115">Geben Sie das Format an, in dem der Inhalt des Elements heruntergeladen werden soll.</span><span class="sxs-lookup"><span data-stu-id="4285c-115">Specify the format the item's content should be downloaded as.</span></span> |


### <a name="format-options"></a><span data-ttu-id="4285c-116">Formatoptionen</span><span class="sxs-lookup"><span data-stu-id="4285c-116">Format options</span></span>

<span data-ttu-id="4285c-117">Die folgenden Werte sind für den **Format**-Parameter gültig:</span><span class="sxs-lookup"><span data-stu-id="4285c-117">The following values are valid for the **convert** parameter:</span></span>

| <span data-ttu-id="4285c-118">Formatwert</span><span class="sxs-lookup"><span data-stu-id="4285c-118">Format value</span></span> | <span data-ttu-id="4285c-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4285c-119">Description</span></span>                        | <span data-ttu-id="4285c-120">Unterstützte Quellerweiterungen</span><span class="sxs-lookup"><span data-stu-id="4285c-120">Supported source extensions</span></span>
|:-------------|:-----------------------------------|----------------------------
| <span data-ttu-id="4285c-121">pdf</span><span class="sxs-lookup"><span data-stu-id="4285c-121">pdf</span></span>          | <span data-ttu-id="4285c-122">Konvertiert das Element ins PDF-Format.</span><span class="sxs-lookup"><span data-stu-id="4285c-122">Converts the item into PDF format.</span></span> | <span data-ttu-id="4285c-123">CSV, DOC, DOCX, ODP, ODS, ODT, POT, POTM, POTX, PPS, PPSX, PPSXM, PPT, PPTM, PPTX, RTF, XLS, XLSX</span><span class="sxs-lookup"><span data-stu-id="4285c-123">csv, doc, docx, odp, ods, odt, pot, potm, potx, pps, ppsx, ppsxm, ppt, pptm, pptx, rtf, xls, xlsx</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="4285c-124">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4285c-124">Optional request headers</span></span>

| <span data-ttu-id="4285c-125">Name</span><span class="sxs-lookup"><span data-stu-id="4285c-125">Name</span></span>            | <span data-ttu-id="4285c-126">Wert</span><span class="sxs-lookup"><span data-stu-id="4285c-126">Value</span></span>   | <span data-ttu-id="4285c-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4285c-127">Description</span></span>                                                                                                                                              |
|:----------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4285c-128">_if-none-match_</span><span class="sxs-lookup"><span data-stu-id="4285c-128">_if-none-match_</span></span> | <span data-ttu-id="4285c-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4285c-129">String</span></span>  | <span data-ttu-id="4285c-130">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) mit dem aktuellen Tag in der Datei übereinstimmt, wird die Antwort `HTTP 304 Not Modified` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4285c-130">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="example"></a><span data-ttu-id="4285c-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4285c-131">Example</span></span>

<!-- { "blockType": "request", "name": "convert-item-content", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/content?format={format}
```

## <a name="response"></a><span data-ttu-id="4285c-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="4285c-132">Response</span></span>

<span data-ttu-id="4285c-133">Die Methode gibt eine Antwort `302 Found` zurück, die auf eine vorab authentifizierte URL zum Download der konvertierten Datei umleitet.</span><span class="sxs-lookup"><span data-stu-id="4285c-133">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the converted file.</span></span>

<span data-ttu-id="4285c-134">Um die konvertierte Datei herunterladen zu können, muss die App den `Location`-Header in der Antwort aufrufen.</span><span class="sxs-lookup"><span data-stu-id="4285c-134">To download the converted file, your app must follow the `Location` header in the response.</span></span>

<span data-ttu-id="4285c-135">Vorab authentifizierte URLs sind nur für eine kurze Zeit gültig (einige Minuten) und erfordern für den Zugriff keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="4285c-135">Pre-authenticated URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to access.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 302 Found
Location: https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi
```

### <a name="error-responses"></a><span data-ttu-id="4285c-136">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="4285c-136">Error responses</span></span>

<span data-ttu-id="4285c-137">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie unter [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="4285c-137">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: ../../../concepts/errors.md
[file-facet]: ../resources/file.md

<!-- {
  "type": "#page.annotation",
  "description": "Convert the contents of an item in OneDrive to a different format.",
  "keywords": "convert,pdf,convert to pdf",
  "section": "documentation",
  "tocPath": "Items/Download formats"
} -->
