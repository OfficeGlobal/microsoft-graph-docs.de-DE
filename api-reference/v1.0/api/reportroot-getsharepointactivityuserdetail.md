---
title: 'reportRoot: getSharePointActivityUserDetail'
description: Rufen Sie Details zu SharePoint-Aktivitäten nach Benutzer ab.
ms.openlocfilehash: 810d014b02c0051a03ecf644507baee66a74f13e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018926"
---
# <a name="reportroot-getsharepointactivityuserdetail"></a><span data-ttu-id="0daad-103">reportRoot: getSharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="0daad-103">reportRoot: getSharePointActivityUserDetail</span></span>

<span data-ttu-id="0daad-104">Rufen Sie Details zu SharePoint-Aktivitäten nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="0daad-104">Get details about SharePoint activity by user.</span></span>

> <span data-ttu-id="0daad-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – SharePoint-Aktivität](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="0daad-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="0daad-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0daad-106">Permissions</span></span>

<span data-ttu-id="0daad-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0daad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0daad-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0daad-109">Permission type</span></span>                        | <span data-ttu-id="0daad-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0daad-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0daad-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0daad-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0daad-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0daad-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0daad-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0daad-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0daad-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0daad-114">Not supported.</span></span>                           |
| <span data-ttu-id="0daad-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0daad-115">Application</span></span>                            | <span data-ttu-id="0daad-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0daad-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0daad-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0daad-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSharePointActivityUserDetail(period='{period_value}')
GET /reports/getSharePointActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="0daad-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="0daad-118">Function parameters</span></span>

<span data-ttu-id="0daad-119">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="0daad-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="0daad-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="0daad-120">Parameter</span></span> | <span data-ttu-id="0daad-121">Typ</span><span class="sxs-lookup"><span data-stu-id="0daad-121">Type</span></span>   | <span data-ttu-id="0daad-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0daad-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0daad-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="0daad-123">period</span></span>    | <span data-ttu-id="0daad-124">string</span><span class="sxs-lookup"><span data-stu-id="0daad-124">string</span></span> | <span data-ttu-id="0daad-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="0daad-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0daad-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="0daad-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0daad-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="0daad-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="0daad-128">date</span><span class="sxs-lookup"><span data-stu-id="0daad-128">date</span></span>      | <span data-ttu-id="0daad-129">Datum</span><span class="sxs-lookup"><span data-stu-id="0daad-129">Date</span></span>   | <span data-ttu-id="0daad-130">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="0daad-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="0daad-131">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="0daad-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="0daad-132">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="0daad-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="0daad-133">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="0daad-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0daad-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0daad-134">Request headers</span></span>

| <span data-ttu-id="0daad-135">Name</span><span class="sxs-lookup"><span data-stu-id="0daad-135">Name</span></span>          | <span data-ttu-id="0daad-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0daad-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="0daad-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="0daad-137">Authorization</span></span> | <span data-ttu-id="0daad-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0daad-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="0daad-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="0daad-140">If-None-Match</span></span> | <span data-ttu-id="0daad-141">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0daad-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="0daad-142">Optional.</span><span class="sxs-lookup"><span data-stu-id="0daad-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="0daad-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="0daad-143">Response</span></span>

<span data-ttu-id="0daad-144">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="0daad-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0daad-145">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0daad-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0daad-146">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="0daad-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0daad-147">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="0daad-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0daad-148">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="0daad-148">Report Refresh Date</span></span>
- <span data-ttu-id="0daad-149">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="0daad-149">User Principal Name</span></span>
- <span data-ttu-id="0daad-150">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="0daad-150">Is Deleted</span></span>
- <span data-ttu-id="0daad-151">Gelöscht am</span><span class="sxs-lookup"><span data-stu-id="0daad-151">Deleted Date</span></span>
- <span data-ttu-id="0daad-152">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="0daad-152">Last Activity Date</span></span>
- <span data-ttu-id="0daad-153">Anzahl der angezeigten oder bearbeiteten Dateien</span><span class="sxs-lookup"><span data-stu-id="0daad-153">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="0daad-154">Anzahl der synchronisierten Dateien</span><span class="sxs-lookup"><span data-stu-id="0daad-154">Synced File Count</span></span>
- <span data-ttu-id="0daad-155">Anzahl der intern freigegebenen Dateien</span><span class="sxs-lookup"><span data-stu-id="0daad-155">Shared Internally File Count</span></span>
- <span data-ttu-id="0daad-156">Anzahl der extern freigegebenen Dateien</span><span class="sxs-lookup"><span data-stu-id="0daad-156">Shared Externally File Count</span></span>
- <span data-ttu-id="0daad-157">Anzahl der besuchten Seiten</span><span class="sxs-lookup"><span data-stu-id="0daad-157">Visited Page Count</span></span>
- <span data-ttu-id="0daad-158">Zugewiesene Produkte</span><span class="sxs-lookup"><span data-stu-id="0daad-158">Assigned Products</span></span>
- <span data-ttu-id="0daad-159">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="0daad-159">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="0daad-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0daad-160">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0daad-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0daad-161">Request</span></span>

<span data-ttu-id="0daad-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0daad-162">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="0daad-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="0daad-163">Response</span></span>

<span data-ttu-id="0daad-164">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0daad-164">The following is an example of the response.</span></span>

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

<span data-ttu-id="0daad-165">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="0daad-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Visited Page Count,Assigned Products,Report Period
```
