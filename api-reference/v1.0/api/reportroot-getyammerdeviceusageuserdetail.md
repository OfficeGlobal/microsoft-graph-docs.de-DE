---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: Rufen Sie Details zur Yammer-Gerätenutzung nach Benutzer ab.
ms.openlocfilehash: c112ba0948adb07dbb5264ab73f6458f2ef97b09
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018177"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="a0680-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="a0680-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

<span data-ttu-id="a0680-104">Rufen Sie Details zur Yammer-Gerätenutzung nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="a0680-104">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="a0680-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Gerätenutzung](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="a0680-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="a0680-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a0680-106">Permissions</span></span>

<span data-ttu-id="a0680-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0680-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a0680-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a0680-109">Permission type</span></span>                        | <span data-ttu-id="a0680-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a0680-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a0680-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a0680-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a0680-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0680-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a0680-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a0680-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0680-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a0680-114">Not supported.</span></span>                           |
| <span data-ttu-id="a0680-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a0680-115">Application</span></span>                            | <span data-ttu-id="a0680-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0680-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a0680-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a0680-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="a0680-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="a0680-118">Function parameters</span></span>

<span data-ttu-id="a0680-119">Stellen Sie in der URL der Anforderung den Parameter mit einem gültigen Wert bereit.</span><span class="sxs-lookup"><span data-stu-id="a0680-119">In the request URL, provide the query parameter with a valid value.</span></span>

| <span data-ttu-id="a0680-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="a0680-120">Parameter</span></span> | <span data-ttu-id="a0680-121">Typ</span><span class="sxs-lookup"><span data-stu-id="a0680-121">Type</span></span>   | <span data-ttu-id="a0680-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a0680-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a0680-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="a0680-123">period</span></span>    | <span data-ttu-id="a0680-124">string</span><span class="sxs-lookup"><span data-stu-id="a0680-124">string</span></span> | <span data-ttu-id="a0680-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="a0680-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a0680-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="a0680-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a0680-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="a0680-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="a0680-128">date</span><span class="sxs-lookup"><span data-stu-id="a0680-128">date</span></span>      | <span data-ttu-id="a0680-129">Datum</span><span class="sxs-lookup"><span data-stu-id="a0680-129">Date</span></span>   | <span data-ttu-id="a0680-130">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="a0680-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="a0680-131">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="a0680-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="a0680-132">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="a0680-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="a0680-133">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="a0680-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0680-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a0680-134">Request headers</span></span>

| <span data-ttu-id="a0680-135">Name</span><span class="sxs-lookup"><span data-stu-id="a0680-135">Name</span></span>          | <span data-ttu-id="a0680-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a0680-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="a0680-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0680-137">Authorization</span></span> | <span data-ttu-id="a0680-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a0680-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="a0680-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="a0680-140">If-None-Match</span></span> | <span data-ttu-id="a0680-141">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a0680-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="a0680-142">Optional.</span><span class="sxs-lookup"><span data-stu-id="a0680-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="a0680-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="a0680-143">Response</span></span>

<span data-ttu-id="a0680-144">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="a0680-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a0680-145">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a0680-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a0680-146">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="a0680-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a0680-147">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="a0680-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a0680-148">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="a0680-148">Report Refresh Date</span></span>
- <span data-ttu-id="a0680-149">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="a0680-149">User Principal Name</span></span>
- <span data-ttu-id="a0680-150">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="a0680-150">Display Name</span></span>
- <span data-ttu-id="a0680-151">Benutzerstatus</span><span class="sxs-lookup"><span data-stu-id="a0680-151">User State</span></span>
- <span data-ttu-id="a0680-152">Datum der Statusänderung</span><span class="sxs-lookup"><span data-stu-id="a0680-152">State Change Date</span></span>
- <span data-ttu-id="a0680-153">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="a0680-153">Last Activity Date</span></span>
- <span data-ttu-id="a0680-154">Verwendetes Web</span><span class="sxs-lookup"><span data-stu-id="a0680-154">Used Web</span></span>
- <span data-ttu-id="a0680-155">Verwendetes Windows Phone</span><span class="sxs-lookup"><span data-stu-id="a0680-155">Used Windows Phone</span></span>
- <span data-ttu-id="a0680-156">Verwendetes Android Phone</span><span class="sxs-lookup"><span data-stu-id="a0680-156">Used Android Phone</span></span>
- <span data-ttu-id="a0680-157">Verwendetes iPhone</span><span class="sxs-lookup"><span data-stu-id="a0680-157">Used iPhone</span></span>
- <span data-ttu-id="a0680-158">Verwendetes iPad</span><span class="sxs-lookup"><span data-stu-id="a0680-158">Used iPad</span></span>
- <span data-ttu-id="a0680-159">Andere verwendet</span><span class="sxs-lookup"><span data-stu-id="a0680-159">Used Others</span></span>
- <span data-ttu-id="a0680-160">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="a0680-160">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="a0680-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a0680-161">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a0680-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a0680-162">Request</span></span>

<span data-ttu-id="a0680-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a0680-163">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="a0680-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="a0680-164">Response</span></span>

<span data-ttu-id="a0680-165">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a0680-165">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="a0680-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a0680-166">Request</span></span>

<span data-ttu-id="a0680-167">Wenn aufgerufen, wobei die `date` Parameter, den Bericht zur Verwendung auf das angegebene Datum ausgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="a0680-167">If called with the `date` parameter, the report is scoped to usage on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="a0680-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="a0680-168">Response</span></span>

<span data-ttu-id="a0680-169">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a0680-169">The following is an example of the response.</span></span>

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

<span data-ttu-id="a0680-170">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="a0680-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Used Web,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Used Others,Report Period
```
