---
title: 'reportRoot: getOneDriveActivityUserDetail'
description: Rufen Sie Details zu OneDrive-Aktivitäten nach Benutzer ab.
ms.openlocfilehash: 43d16f9e71a2d2ab2535c206c39f3a09b4c391e9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017323"
---
# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="bd58a-103">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="bd58a-103">reportRoot: getOneDriveActivityUserDetail</span></span>

<span data-ttu-id="bd58a-104">Rufen Sie Details zu OneDrive-Aktivitäten nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="bd58a-104">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="bd58a-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – OneDrive for Business-Aktivität](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="bd58a-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="bd58a-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bd58a-106">Permissions</span></span>

<span data-ttu-id="bd58a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd58a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd58a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bd58a-109">Permission type</span></span>                        | <span data-ttu-id="bd58a-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bd58a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bd58a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bd58a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd58a-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd58a-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bd58a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bd58a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd58a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bd58a-114">Not supported.</span></span>                           |
| <span data-ttu-id="bd58a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bd58a-115">Application</span></span>                            | <span data-ttu-id="bd58a-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd58a-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bd58a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd58a-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="bd58a-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="bd58a-118">Function parameters</span></span>

<span data-ttu-id="bd58a-119">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="bd58a-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="bd58a-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="bd58a-120">Parameter</span></span> | <span data-ttu-id="bd58a-121">Typ</span><span class="sxs-lookup"><span data-stu-id="bd58a-121">Type</span></span>   | <span data-ttu-id="bd58a-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd58a-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bd58a-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="bd58a-123">period</span></span>    | <span data-ttu-id="bd58a-124">string</span><span class="sxs-lookup"><span data-stu-id="bd58a-124">string</span></span> | <span data-ttu-id="bd58a-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="bd58a-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bd58a-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="bd58a-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bd58a-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="bd58a-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="bd58a-128">date</span><span class="sxs-lookup"><span data-stu-id="bd58a-128">date</span></span>      | <span data-ttu-id="bd58a-129">Datum</span><span class="sxs-lookup"><span data-stu-id="bd58a-129">Date</span></span>   | <span data-ttu-id="bd58a-130">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="bd58a-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="bd58a-131">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="bd58a-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="bd58a-132">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="bd58a-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="bd58a-133">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="bd58a-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd58a-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bd58a-134">Request headers</span></span>

| <span data-ttu-id="bd58a-135">Name</span><span class="sxs-lookup"><span data-stu-id="bd58a-135">Name</span></span>          | <span data-ttu-id="bd58a-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd58a-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="bd58a-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd58a-137">Authorization</span></span> | <span data-ttu-id="bd58a-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bd58a-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="bd58a-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="bd58a-140">If-None-Match</span></span> | <span data-ttu-id="bd58a-141">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bd58a-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="bd58a-142">Optional.</span><span class="sxs-lookup"><span data-stu-id="bd58a-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="bd58a-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd58a-143">Response</span></span>

<span data-ttu-id="bd58a-144">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="bd58a-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bd58a-145">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bd58a-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bd58a-146">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="bd58a-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bd58a-147">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="bd58a-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bd58a-148">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="bd58a-148">Report Refresh Date</span></span>
- <span data-ttu-id="bd58a-149">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="bd58a-149">User Principal Name</span></span>
- <span data-ttu-id="bd58a-150">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="bd58a-150">Is Deleted</span></span>
- <span data-ttu-id="bd58a-151">Gelöscht am</span><span class="sxs-lookup"><span data-stu-id="bd58a-151">Deleted Date</span></span>
- <span data-ttu-id="bd58a-152">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="bd58a-152">Last Activity Date</span></span>
- <span data-ttu-id="bd58a-153">Anzahl der angezeigten oder bearbeiteten Dateien</span><span class="sxs-lookup"><span data-stu-id="bd58a-153">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="bd58a-154">Anzahl der synchronisierten Dateien</span><span class="sxs-lookup"><span data-stu-id="bd58a-154">Synced File Count</span></span>
- <span data-ttu-id="bd58a-155">Anzahl der intern freigegebenen Dateien</span><span class="sxs-lookup"><span data-stu-id="bd58a-155">Shared Internally File Count</span></span>
- <span data-ttu-id="bd58a-156">Anzahl der extern freigegebenen Dateien</span><span class="sxs-lookup"><span data-stu-id="bd58a-156">Shared Externally File Count</span></span>
- <span data-ttu-id="bd58a-157">Zugewiesene Produkte</span><span class="sxs-lookup"><span data-stu-id="bd58a-157">Assigned Products</span></span>
- <span data-ttu-id="bd58a-158">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="bd58a-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="bd58a-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bd58a-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bd58a-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd58a-160">Request</span></span>

<span data-ttu-id="bd58a-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bd58a-161">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="bd58a-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd58a-162">Response</span></span>

<span data-ttu-id="bd58a-163">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bd58a-163">The following is an example of the response.</span></span>

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

<span data-ttu-id="bd58a-164">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="bd58a-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Assigned Products,Report Period
```
