---
title: 'reportRoot: getSharePointActivityUserDetail'
description: Rufen Sie Details zu SharePoint-Aktivitäten nach Benutzer ab.
localization_priority: Normal
ms.openlocfilehash: b854e74db351ee2f3fb890ade26da9ec0cd21341
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823310"
---
# <a name="reportroot-getsharepointactivityuserdetail"></a><span data-ttu-id="30ffe-103">reportRoot: getSharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="30ffe-103">reportRoot: getSharePointActivityUserDetail</span></span>

<span data-ttu-id="30ffe-104">Rufen Sie Details zu SharePoint-Aktivitäten nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="30ffe-104">Get details about SharePoint activity by user.</span></span>

> <span data-ttu-id="30ffe-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – SharePoint-Aktivität](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="30ffe-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="30ffe-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="30ffe-106">Permissions</span></span>

<span data-ttu-id="30ffe-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30ffe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="30ffe-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="30ffe-109">Permission type</span></span>                        | <span data-ttu-id="30ffe-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="30ffe-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="30ffe-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="30ffe-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="30ffe-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="30ffe-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="30ffe-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="30ffe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30ffe-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="30ffe-114">Not supported.</span></span>                           |
| <span data-ttu-id="30ffe-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="30ffe-115">Application</span></span>                            | <span data-ttu-id="30ffe-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="30ffe-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="30ffe-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="30ffe-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSharePointActivityUserDetail(period='{period_value}')
GET /reports/getSharePointActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="30ffe-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="30ffe-118">Function parameters</span></span>

<span data-ttu-id="30ffe-119">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="30ffe-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="30ffe-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="30ffe-120">Parameter</span></span> | <span data-ttu-id="30ffe-121">Typ</span><span class="sxs-lookup"><span data-stu-id="30ffe-121">Type</span></span>   | <span data-ttu-id="30ffe-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="30ffe-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="30ffe-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="30ffe-123">period</span></span>    | <span data-ttu-id="30ffe-124">string</span><span class="sxs-lookup"><span data-stu-id="30ffe-124">string</span></span> | <span data-ttu-id="30ffe-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="30ffe-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="30ffe-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="30ffe-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="30ffe-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="30ffe-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="30ffe-128">date</span><span class="sxs-lookup"><span data-stu-id="30ffe-128">date</span></span>      | <span data-ttu-id="30ffe-129">Datum</span><span class="sxs-lookup"><span data-stu-id="30ffe-129">Date</span></span>   | <span data-ttu-id="30ffe-130">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="30ffe-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="30ffe-131">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="30ffe-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="30ffe-132">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="30ffe-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="30ffe-133">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="30ffe-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30ffe-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="30ffe-134">Request headers</span></span>

| <span data-ttu-id="30ffe-135">Name</span><span class="sxs-lookup"><span data-stu-id="30ffe-135">Name</span></span>          | <span data-ttu-id="30ffe-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="30ffe-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="30ffe-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="30ffe-137">Authorization</span></span> | <span data-ttu-id="30ffe-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="30ffe-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="30ffe-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="30ffe-140">If-None-Match</span></span> | <span data-ttu-id="30ffe-141">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="30ffe-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="30ffe-142">Optional.</span><span class="sxs-lookup"><span data-stu-id="30ffe-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="30ffe-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="30ffe-143">Response</span></span>

<span data-ttu-id="30ffe-144">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="30ffe-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="30ffe-145">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="30ffe-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="30ffe-146">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="30ffe-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="30ffe-147">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="30ffe-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="30ffe-148">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="30ffe-148">Report Refresh Date</span></span>
- <span data-ttu-id="30ffe-149">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="30ffe-149">User Principal Name</span></span>
- <span data-ttu-id="30ffe-150">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="30ffe-150">Is Deleted</span></span>
- <span data-ttu-id="30ffe-151">Gelöscht am</span><span class="sxs-lookup"><span data-stu-id="30ffe-151">Deleted Date</span></span>
- <span data-ttu-id="30ffe-152">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="30ffe-152">Last Activity Date</span></span>
- <span data-ttu-id="30ffe-153">Anzahl der angezeigten oder bearbeiteten Dateien</span><span class="sxs-lookup"><span data-stu-id="30ffe-153">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="30ffe-154">Anzahl der synchronisierten Dateien</span><span class="sxs-lookup"><span data-stu-id="30ffe-154">Synced File Count</span></span>
- <span data-ttu-id="30ffe-155">Anzahl der intern freigegebenen Dateien</span><span class="sxs-lookup"><span data-stu-id="30ffe-155">Shared Internally File Count</span></span>
- <span data-ttu-id="30ffe-156">Anzahl der extern freigegebenen Dateien</span><span class="sxs-lookup"><span data-stu-id="30ffe-156">Shared Externally File Count</span></span>
- <span data-ttu-id="30ffe-157">Anzahl der besuchten Seiten</span><span class="sxs-lookup"><span data-stu-id="30ffe-157">Visited Page Count</span></span>
- <span data-ttu-id="30ffe-158">Zugewiesene Produkte</span><span class="sxs-lookup"><span data-stu-id="30ffe-158">Assigned Products</span></span>
- <span data-ttu-id="30ffe-159">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="30ffe-159">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="30ffe-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="30ffe-160">Example</span></span>

#### <a name="request"></a><span data-ttu-id="30ffe-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="30ffe-161">Request</span></span>

<span data-ttu-id="30ffe-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="30ffe-162">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="30ffe-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="30ffe-163">Response</span></span>

<span data-ttu-id="30ffe-164">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="30ffe-164">The following is an example of the response.</span></span>

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

<span data-ttu-id="30ffe-165">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="30ffe-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Visited Page Count,Assigned Products,Report Period
```
