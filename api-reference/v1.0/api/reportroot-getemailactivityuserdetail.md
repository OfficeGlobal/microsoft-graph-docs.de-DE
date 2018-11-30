---
title: 'reportRoot: getEmailActivityUserDetail'
description: Erhalten Sie detaillierte Informationen über die von Benutzern ausgeführten E-Mail-Aktivitäten.
ms.openlocfilehash: 11d8e081c15be137c181d0f2608f5821d3e2e63e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016117"
---
# <a name="reportroot-getemailactivityuserdetail"></a><span data-ttu-id="7b1f2-103">reportRoot: getEmailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="7b1f2-103">reportRoot: getEmailActivityUserDetail</span></span>

<span data-ttu-id="7b1f2-104">Erhalten Sie detaillierte Informationen über die von Benutzern ausgeführten E-Mail-Aktivitäten.</span><span class="sxs-lookup"><span data-stu-id="7b1f2-104">Get details about email activity users have performed.</span></span>

> <span data-ttu-id="7b1f2-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – E-Mail-Aktivität](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="7b1f2-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="7b1f2-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7b1f2-106">Permissions</span></span>

<span data-ttu-id="7b1f2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b1f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7b1f2-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7b1f2-109">Permission type</span></span>                        | <span data-ttu-id="7b1f2-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7b1f2-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7b1f2-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7b1f2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7b1f2-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b1f2-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7b1f2-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7b1f2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b1f2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b1f2-114">Not supported.</span></span>                           |
| <span data-ttu-id="7b1f2-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7b1f2-115">Application</span></span>                            | <span data-ttu-id="7b1f2-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b1f2-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7b1f2-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b1f2-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getEmailActivityUserDetail(period='{period_value}')
GET /reports/getEmailActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="7b1f2-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="7b1f2-118">Function parameters</span></span>

<span data-ttu-id="7b1f2-119">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="7b1f2-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="7b1f2-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="7b1f2-120">Parameter</span></span> | <span data-ttu-id="7b1f2-121">Typ</span><span class="sxs-lookup"><span data-stu-id="7b1f2-121">Type</span></span>   | <span data-ttu-id="7b1f2-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b1f2-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7b1f2-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="7b1f2-123">period</span></span>    | <span data-ttu-id="7b1f2-124">string</span><span class="sxs-lookup"><span data-stu-id="7b1f2-124">string</span></span> | <span data-ttu-id="7b1f2-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="7b1f2-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7b1f2-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="7b1f2-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7b1f2-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="7b1f2-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="7b1f2-128">date</span><span class="sxs-lookup"><span data-stu-id="7b1f2-128">date</span></span>      | <span data-ttu-id="7b1f2-129">Datum</span><span class="sxs-lookup"><span data-stu-id="7b1f2-129">Date</span></span>   | <span data-ttu-id="7b1f2-130">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="7b1f2-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="7b1f2-131">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="7b1f2-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="7b1f2-132">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="7b1f2-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="7b1f2-133">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="7b1f2-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b1f2-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7b1f2-134">Request headers</span></span>

| <span data-ttu-id="7b1f2-135">Name</span><span class="sxs-lookup"><span data-stu-id="7b1f2-135">Name</span></span>          | <span data-ttu-id="7b1f2-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b1f2-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="7b1f2-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b1f2-137">Authorization</span></span> | <span data-ttu-id="7b1f2-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7b1f2-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="7b1f2-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="7b1f2-140">If-None-Match</span></span> | <span data-ttu-id="7b1f2-141">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7b1f2-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="7b1f2-142">Optional.</span><span class="sxs-lookup"><span data-stu-id="7b1f2-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="7b1f2-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b1f2-143">Response</span></span>

<span data-ttu-id="7b1f2-144">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="7b1f2-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7b1f2-145">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7b1f2-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7b1f2-146">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="7b1f2-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7b1f2-147">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="7b1f2-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7b1f2-148">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="7b1f2-148">Report Refresh Date</span></span>
- <span data-ttu-id="7b1f2-149">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="7b1f2-149">User Principal Name</span></span>
- <span data-ttu-id="7b1f2-150">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="7b1f2-150">Display Name</span></span>
- <span data-ttu-id="7b1f2-151">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="7b1f2-151">Is Deleted</span></span>
- <span data-ttu-id="7b1f2-152">Gelöscht am</span><span class="sxs-lookup"><span data-stu-id="7b1f2-152">Deleted Date</span></span>
- <span data-ttu-id="7b1f2-153">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="7b1f2-153">Last Activity Date</span></span>
- <span data-ttu-id="7b1f2-154">Anzahl gesendet</span><span class="sxs-lookup"><span data-stu-id="7b1f2-154">Send Count</span></span>
- <span data-ttu-id="7b1f2-155">Anzahl empfangen</span><span class="sxs-lookup"><span data-stu-id="7b1f2-155">Receive Count</span></span>
- <span data-ttu-id="7b1f2-156">Anzahl gelesen</span><span class="sxs-lookup"><span data-stu-id="7b1f2-156">Read Count</span></span>
- <span data-ttu-id="7b1f2-157">Zugewiesene Produkte</span><span class="sxs-lookup"><span data-stu-id="7b1f2-157">Assigned Products</span></span>
- <span data-ttu-id="7b1f2-158">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="7b1f2-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="7b1f2-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7b1f2-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7b1f2-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b1f2-160">Request</span></span>

<span data-ttu-id="7b1f2-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7b1f2-161">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="7b1f2-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b1f2-162">Response</span></span>

<span data-ttu-id="7b1f2-163">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7b1f2-163">The following is an example of the response.</span></span>

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

<span data-ttu-id="7b1f2-164">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="7b1f2-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Send Count,Receive Count,Read Count,Assigned Products,Report Period
```
