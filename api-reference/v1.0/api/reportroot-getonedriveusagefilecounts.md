---
title: 'reportRoot: getOneDriveUsageFileCounts'
description: Rufen Sie die Gesamtzahl der Dateien aller Websites und die Anzahl der aktiven Dateien ab. Eine Datei wird als aktiv betrachtet, wenn sie innerhalb des angegebenen Zeitraums gespeichert, synchronisiert, geändert oder freigegeben wurde.
localization_priority: Normal
ms.openlocfilehash: d5c7127bfb5389dbf77e2bf168fd966768711932
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815666"
---
# <a name="reportroot-getonedriveusagefilecounts"></a><span data-ttu-id="b8500-104">reportRoot: getOneDriveUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="b8500-104">reportRoot: getOneDriveUsageFileCounts</span></span>

<span data-ttu-id="b8500-105">Rufen Sie die Gesamtzahl der Dateien aller Websites und die Anzahl der aktiven Dateien ab.</span><span class="sxs-lookup"><span data-stu-id="b8500-105">Get the total number of files across all sites and how many are active files.</span></span> <span data-ttu-id="b8500-106">Eine Datei wird als aktiv betrachtet, wenn sie innerhalb des angegebenen Zeitraums gespeichert, synchronisiert, geändert oder freigegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="b8500-106">A file is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="b8500-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – OneDrive for Business-Nutzung](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="b8500-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="b8500-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b8500-108">Permissions</span></span>

<span data-ttu-id="b8500-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8500-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b8500-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b8500-111">Permission type</span></span>                        | <span data-ttu-id="b8500-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b8500-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b8500-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b8500-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b8500-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8500-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b8500-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b8500-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8500-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8500-116">Not supported.</span></span>                           |
| <span data-ttu-id="b8500-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b8500-117">Application</span></span>                            | <span data-ttu-id="b8500-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8500-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b8500-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8500-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b8500-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="b8500-120">Function parameters</span></span>

<span data-ttu-id="b8500-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="b8500-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b8500-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="b8500-122">Parameter</span></span> | <span data-ttu-id="b8500-123">Typ</span><span class="sxs-lookup"><span data-stu-id="b8500-123">Type</span></span>   | <span data-ttu-id="b8500-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8500-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b8500-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="b8500-125">period</span></span>    | <span data-ttu-id="b8500-126">string</span><span class="sxs-lookup"><span data-stu-id="b8500-126">string</span></span> | <span data-ttu-id="b8500-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="b8500-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b8500-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="b8500-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b8500-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="b8500-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b8500-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="b8500-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="b8500-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b8500-131">Request headers</span></span>

| <span data-ttu-id="b8500-132">Name</span><span class="sxs-lookup"><span data-stu-id="b8500-132">Name</span></span>          | <span data-ttu-id="b8500-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8500-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b8500-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8500-134">Authorization</span></span> | <span data-ttu-id="b8500-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b8500-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b8500-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b8500-137">If-None-Match</span></span> | <span data-ttu-id="b8500-138">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8500-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b8500-139">Optional.</span><span class="sxs-lookup"><span data-stu-id="b8500-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b8500-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8500-140">Response</span></span>

<span data-ttu-id="b8500-141">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="b8500-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b8500-142">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b8500-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b8500-143">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="b8500-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b8500-144">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="b8500-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b8500-145">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="b8500-145">Report Refresh Date</span></span>
- <span data-ttu-id="b8500-146">Websitetyp</span><span class="sxs-lookup"><span data-stu-id="b8500-146">Site Type</span></span>
- <span data-ttu-id="b8500-147">Gesamt</span><span class="sxs-lookup"><span data-stu-id="b8500-147">Total</span></span>
- <span data-ttu-id="b8500-148">Aktiv</span><span class="sxs-lookup"><span data-stu-id="b8500-148">Active</span></span>
- <span data-ttu-id="b8500-149">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="b8500-149">Report Date</span></span>
- <span data-ttu-id="b8500-150">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="b8500-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b8500-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b8500-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b8500-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8500-152">Request</span></span>

<span data-ttu-id="b8500-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b8500-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusagefilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageFileCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="b8500-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8500-154">Response</span></span>

<span data-ttu-id="b8500-155">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b8500-155">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b8500-156">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="b8500-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```
