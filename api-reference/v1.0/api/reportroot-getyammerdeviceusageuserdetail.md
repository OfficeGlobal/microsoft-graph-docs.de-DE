---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: Rufen Sie Details zur Yammer-Gerätenutzung nach Benutzer ab.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d273c2102226f75ff0638402b534511003b0102f
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572836"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="5555a-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="5555a-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

<span data-ttu-id="5555a-104">Rufen Sie Details zur Yammer-Gerätenutzung nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="5555a-104">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="5555a-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Gerätenutzung](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="5555a-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="5555a-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5555a-106">Permissions</span></span>

<span data-ttu-id="5555a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5555a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5555a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5555a-109">Permission type</span></span>                        | <span data-ttu-id="5555a-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5555a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5555a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5555a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5555a-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5555a-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5555a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5555a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5555a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5555a-114">Not supported.</span></span>                           |
| <span data-ttu-id="5555a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5555a-115">Application</span></span>                            | <span data-ttu-id="5555a-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5555a-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5555a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5555a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="5555a-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="5555a-118">Function parameters</span></span>

<span data-ttu-id="5555a-119">Stellen Sie in der URL der Anforderung den Parameter mit einem gültigen Wert bereit.</span><span class="sxs-lookup"><span data-stu-id="5555a-119">In the request URL, provide the query parameter with a valid value.</span></span>

| <span data-ttu-id="5555a-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="5555a-120">Parameter</span></span> | <span data-ttu-id="5555a-121">Typ</span><span class="sxs-lookup"><span data-stu-id="5555a-121">Type</span></span>   | <span data-ttu-id="5555a-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5555a-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5555a-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="5555a-123">period</span></span>    | <span data-ttu-id="5555a-124">string</span><span class="sxs-lookup"><span data-stu-id="5555a-124">string</span></span> | <span data-ttu-id="5555a-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="5555a-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5555a-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="5555a-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5555a-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="5555a-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="5555a-128">date</span><span class="sxs-lookup"><span data-stu-id="5555a-128">date</span></span>      | <span data-ttu-id="5555a-129">Datum</span><span class="sxs-lookup"><span data-stu-id="5555a-129">Date</span></span>   | <span data-ttu-id="5555a-130">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="5555a-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="5555a-131">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="5555a-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="5555a-132">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="5555a-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="5555a-133">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="5555a-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5555a-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5555a-134">Request headers</span></span>

| <span data-ttu-id="5555a-135">Name</span><span class="sxs-lookup"><span data-stu-id="5555a-135">Name</span></span>          | <span data-ttu-id="5555a-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5555a-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="5555a-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="5555a-137">Authorization</span></span> | <span data-ttu-id="5555a-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5555a-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="5555a-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="5555a-140">If-None-Match</span></span> | <span data-ttu-id="5555a-141">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5555a-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="5555a-142">Optional.</span><span class="sxs-lookup"><span data-stu-id="5555a-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5555a-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="5555a-143">Response</span></span>

<span data-ttu-id="5555a-144">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="5555a-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5555a-145">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5555a-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5555a-146">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="5555a-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5555a-147">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="5555a-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5555a-148">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="5555a-148">Report Refresh Date</span></span>
- <span data-ttu-id="5555a-149">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="5555a-149">User Principal Name</span></span>
- <span data-ttu-id="5555a-150">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="5555a-150">Display Name</span></span>
- <span data-ttu-id="5555a-151">Benutzerstatus</span><span class="sxs-lookup"><span data-stu-id="5555a-151">User State</span></span>
- <span data-ttu-id="5555a-152">Datum der Statusänderung</span><span class="sxs-lookup"><span data-stu-id="5555a-152">State Change Date</span></span>
- <span data-ttu-id="5555a-153">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="5555a-153">Last Activity Date</span></span>
- <span data-ttu-id="5555a-154">Verwendetes Web</span><span class="sxs-lookup"><span data-stu-id="5555a-154">Used Web</span></span>
- <span data-ttu-id="5555a-155">Verwendetes Windows Phone</span><span class="sxs-lookup"><span data-stu-id="5555a-155">Used Windows Phone</span></span>
- <span data-ttu-id="5555a-156">Verwendetes Android Phone</span><span class="sxs-lookup"><span data-stu-id="5555a-156">Used Android Phone</span></span>
- <span data-ttu-id="5555a-157">Verwendetes iPhone</span><span class="sxs-lookup"><span data-stu-id="5555a-157">Used iPhone</span></span>
- <span data-ttu-id="5555a-158">Verwendetes iPad</span><span class="sxs-lookup"><span data-stu-id="5555a-158">Used iPad</span></span>
- <span data-ttu-id="5555a-159">Andere verwendet</span><span class="sxs-lookup"><span data-stu-id="5555a-159">Used Others</span></span>
- <span data-ttu-id="5555a-160">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="5555a-160">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="5555a-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5555a-161">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5555a-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5555a-162">Request</span></span>

<span data-ttu-id="5555a-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5555a-163">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="5555a-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="5555a-164">Response</span></span>

<span data-ttu-id="5555a-165">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5555a-165">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="5555a-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5555a-166">Request</span></span>

<span data-ttu-id="5555a-167">Wenn aufgerufen, wobei die `date` Parameter, den Bericht zur Verwendung auf das angegebene Datum ausgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="5555a-167">If called with the `date` parameter, the report is scoped to usage on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="5555a-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="5555a-168">Response</span></span>

<span data-ttu-id="5555a-169">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5555a-169">The following is an example of the response.</span></span>

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

<span data-ttu-id="5555a-170">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="5555a-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Used Web,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Used Others,Report Period
```
