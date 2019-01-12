---
title: 'reportRoot: getOneDriveUsageStorage'
description: Verschaffen Sie sich einen Überblick über die Menge an Speicherplatz, die Sie in OneDrive for Business verwenden.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 61982c9013d5827fa9b47e4c98d453e4cf8f2b94
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936053"
---
# <a name="reportroot-getonedriveusagestorage"></a><span data-ttu-id="0a12f-103">reportRoot: getOneDriveUsageStorage</span><span class="sxs-lookup"><span data-stu-id="0a12f-103">reportRoot: getOneDriveUsageStorage</span></span>

<span data-ttu-id="0a12f-104">Verschaffen Sie sich einen Überblick über die Menge an Speicherplatz, die Sie in OneDrive for Business verwenden.</span><span class="sxs-lookup"><span data-stu-id="0a12f-104">Get the trend on the amount of storage you are using in OneDrive for Business.</span></span>

> <span data-ttu-id="0a12f-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – OneDrive for Business-Nutzung](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="0a12f-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="0a12f-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0a12f-106">Permissions</span></span>

<span data-ttu-id="0a12f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a12f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0a12f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0a12f-109">Permission type</span></span>                        | <span data-ttu-id="0a12f-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0a12f-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0a12f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0a12f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a12f-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a12f-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0a12f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0a12f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a12f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0a12f-114">Not supported.</span></span>                           |
| <span data-ttu-id="0a12f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0a12f-115">Application</span></span>                            | <span data-ttu-id="0a12f-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a12f-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0a12f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a12f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="0a12f-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="0a12f-118">Function parameters</span></span>

<span data-ttu-id="0a12f-119">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="0a12f-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0a12f-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="0a12f-120">Parameter</span></span> | <span data-ttu-id="0a12f-121">Typ</span><span class="sxs-lookup"><span data-stu-id="0a12f-121">Type</span></span>   | <span data-ttu-id="0a12f-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a12f-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0a12f-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="0a12f-123">period</span></span>    | <span data-ttu-id="0a12f-124">string</span><span class="sxs-lookup"><span data-stu-id="0a12f-124">string</span></span> | <span data-ttu-id="0a12f-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="0a12f-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0a12f-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="0a12f-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0a12f-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="0a12f-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0a12f-128">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="0a12f-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="0a12f-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0a12f-129">Request headers</span></span>

| <span data-ttu-id="0a12f-130">Name</span><span class="sxs-lookup"><span data-stu-id="0a12f-130">Name</span></span>          | <span data-ttu-id="0a12f-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a12f-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="0a12f-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a12f-132">Authorization</span></span> | <span data-ttu-id="0a12f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0a12f-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="0a12f-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="0a12f-135">If-None-Match</span></span> | <span data-ttu-id="0a12f-136">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0a12f-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="0a12f-137">Optional.</span><span class="sxs-lookup"><span data-stu-id="0a12f-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="0a12f-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a12f-138">Response</span></span>

<span data-ttu-id="0a12f-139">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="0a12f-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0a12f-140">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0a12f-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0a12f-141">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="0a12f-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0a12f-142">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="0a12f-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0a12f-143">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="0a12f-143">Report Refresh Date</span></span>
- <span data-ttu-id="0a12f-144">Websitetyp</span><span class="sxs-lookup"><span data-stu-id="0a12f-144">Site Type</span></span>
- <span data-ttu-id="0a12f-145">Verwendeter Speicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="0a12f-145">Storage Used (Byte)</span></span>
- <span data-ttu-id="0a12f-146">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="0a12f-146">Report Date</span></span>
- <span data-ttu-id="0a12f-147">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="0a12f-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="0a12f-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0a12f-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0a12f-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a12f-149">Request</span></span>

<span data-ttu-id="0a12f-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0a12f-150">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusagestorage"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageStorage(period='D7')
```

#### <a name="response"></a><span data-ttu-id="0a12f-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a12f-151">Response</span></span>

<span data-ttu-id="0a12f-152">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0a12f-152">The following is an example of the response.</span></span>

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

<span data-ttu-id="0a12f-153">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="0a12f-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Storage Used (Byte),Report Date,Report Period
```
