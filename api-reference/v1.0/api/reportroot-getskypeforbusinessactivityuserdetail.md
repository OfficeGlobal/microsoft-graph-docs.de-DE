---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: Rufen Sie Details der Skype for Business-Aktivität nach Benutzer ab.
ms.openlocfilehash: c5bc32441b65bf55ff5114c161bd9a85bf795fbe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019958"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="2e239-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="2e239-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

<span data-ttu-id="2e239-104">Rufen Sie Details der Skype for Business-Aktivität nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="2e239-104">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="2e239-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Aktivität](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="2e239-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="2e239-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2e239-106">Permissions</span></span>

<span data-ttu-id="2e239-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e239-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2e239-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2e239-109">Permission type</span></span>                        | <span data-ttu-id="2e239-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2e239-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2e239-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2e239-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2e239-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e239-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2e239-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2e239-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e239-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e239-114">Not supported.</span></span>                           |
| <span data-ttu-id="2e239-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2e239-115">Application</span></span>                            | <span data-ttu-id="2e239-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e239-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2e239-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e239-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="2e239-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="2e239-118">Function parameters</span></span>

<span data-ttu-id="2e239-119">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="2e239-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="2e239-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="2e239-120">Parameter</span></span> | <span data-ttu-id="2e239-121">Typ</span><span class="sxs-lookup"><span data-stu-id="2e239-121">Type</span></span>   | <span data-ttu-id="2e239-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e239-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2e239-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="2e239-123">period</span></span>    | <span data-ttu-id="2e239-124">string</span><span class="sxs-lookup"><span data-stu-id="2e239-124">string</span></span> | <span data-ttu-id="2e239-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="2e239-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2e239-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="2e239-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2e239-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="2e239-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="2e239-128">date</span><span class="sxs-lookup"><span data-stu-id="2e239-128">date</span></span>      | <span data-ttu-id="2e239-129">Datum</span><span class="sxs-lookup"><span data-stu-id="2e239-129">Date</span></span>   | <span data-ttu-id="2e239-130">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="2e239-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="2e239-131">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="2e239-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="2e239-132">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="2e239-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="2e239-133">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="2e239-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2e239-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2e239-134">Request headers</span></span>

| <span data-ttu-id="2e239-135">Name</span><span class="sxs-lookup"><span data-stu-id="2e239-135">Name</span></span>          | <span data-ttu-id="2e239-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e239-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="2e239-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e239-137">Authorization</span></span> | <span data-ttu-id="2e239-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2e239-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="2e239-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="2e239-140">If-None-Match</span></span> | <span data-ttu-id="2e239-141">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2e239-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="2e239-142">Optional.</span><span class="sxs-lookup"><span data-stu-id="2e239-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="2e239-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e239-143">Response</span></span>

<span data-ttu-id="2e239-144">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="2e239-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2e239-145">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2e239-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2e239-146">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="2e239-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2e239-147">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="2e239-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2e239-148">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="2e239-148">Report Refresh Date</span></span>
- <span data-ttu-id="2e239-149">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="2e239-149">User Principal Name</span></span>
- <span data-ttu-id="2e239-150">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="2e239-150">Is Deleted</span></span>
- <span data-ttu-id="2e239-151">Gelöscht am</span><span class="sxs-lookup"><span data-stu-id="2e239-151">Deleted Date</span></span>
- <span data-ttu-id="2e239-152">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="2e239-152">Last Activity Date</span></span>
- <span data-ttu-id="2e239-153">Gesamtzahl Peer-to-Peer-Sitzung</span><span class="sxs-lookup"><span data-stu-id="2e239-153">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="2e239-154">Gesamtzahl Organisierte Konferenz</span><span class="sxs-lookup"><span data-stu-id="2e239-154">Total Organized Conference Count</span></span>
- <span data-ttu-id="2e239-155">Gesamtzahl der teilgenommenen Konferenzen</span><span class="sxs-lookup"><span data-stu-id="2e239-155">Total Participated Conference Count</span></span>
- <span data-ttu-id="2e239-156">Datum der letzten Peer-to-Peer-Aktivität</span><span class="sxs-lookup"><span data-stu-id="2e239-156">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="2e239-157">Datum der letzten Aktivität der organisierten Konferenz</span><span class="sxs-lookup"><span data-stu-id="2e239-157">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="2e239-158">Datum der letzten Aktivität der teilgenommenen Konferenz</span><span class="sxs-lookup"><span data-stu-id="2e239-158">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="2e239-159">Anzahl Peer-to-Peer-Chat</span><span class="sxs-lookup"><span data-stu-id="2e239-159">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="2e239-160">Anzahl Peer-to-Peer-Audio</span><span class="sxs-lookup"><span data-stu-id="2e239-160">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="2e239-161">Peer-to-Peer-Audiominuten</span><span class="sxs-lookup"><span data-stu-id="2e239-161">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="2e239-162">Anzahl Peer-to-Peer-Video</span><span class="sxs-lookup"><span data-stu-id="2e239-162">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="2e239-163">Peer-to-Peer-Videominuten</span><span class="sxs-lookup"><span data-stu-id="2e239-163">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="2e239-164">Anzahl Peer-to-Peer-App-Freigabe</span><span class="sxs-lookup"><span data-stu-id="2e239-164">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="2e239-165">Anzahl Peer-to-Peer-Dateiübertragung</span><span class="sxs-lookup"><span data-stu-id="2e239-165">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="2e239-166">Anzahl Organisierte Konferenz-Chat</span><span class="sxs-lookup"><span data-stu-id="2e239-166">Organized Conference IM Count</span></span>
- <span data-ttu-id="2e239-167">Anzahl Organisierte Konferenz-Audio/Video</span><span class="sxs-lookup"><span data-stu-id="2e239-167">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="2e239-168">Anzahl Organisierte Konferenz-Audio-/Videominuten</span><span class="sxs-lookup"><span data-stu-id="2e239-168">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="2e239-169">Anzahl Organisierte Konferenz-App-Freigabe</span><span class="sxs-lookup"><span data-stu-id="2e239-169">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="2e239-170">Anzahl Organisierte Konferenz-Web</span><span class="sxs-lookup"><span data-stu-id="2e239-170">Organized Conference Web Count</span></span>
- <span data-ttu-id="2e239-171">Anzahl Organisierte Konferenz-Einwahl/Auswahl Drittanbieter</span><span class="sxs-lookup"><span data-stu-id="2e239-171">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="2e239-172">Anzahl Organisierte Konferenz-Einwahl/Auswahl Microsoft</span><span class="sxs-lookup"><span data-stu-id="2e239-172">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="2e239-173">Organisierte Konferenz-Einwahlminuten Microsoft</span><span class="sxs-lookup"><span data-stu-id="2e239-173">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="2e239-174">Organisierte Konferenz-Auswahlminuten Microsoft</span><span class="sxs-lookup"><span data-stu-id="2e239-174">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="2e239-175">Anzahl Teilgenommene Konferenz-Chat</span><span class="sxs-lookup"><span data-stu-id="2e239-175">Paricipated Conference IM Count</span></span>
- <span data-ttu-id="2e239-176">Anzahl Teilgenommene Konferenz-Audio/Video</span><span class="sxs-lookup"><span data-stu-id="2e239-176">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="2e239-177">Teilgenommene Konferenz-Audio-/Videominuten</span><span class="sxs-lookup"><span data-stu-id="2e239-177">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="2e239-178">Anzahl Teilgenommene Konferenz-App-Freigabe</span><span class="sxs-lookup"><span data-stu-id="2e239-178">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="2e239-179">Anzahl Teilgenommene Konferenz-Web</span><span class="sxs-lookup"><span data-stu-id="2e239-179">Participated Conference Web Count</span></span>
- <span data-ttu-id="2e239-180">Anzahl Teilgenommene Konferenz-Einwahl/Auswahl Drittanbieter</span><span class="sxs-lookup"><span data-stu-id="2e239-180">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="2e239-181">Zugewiesene Produkte</span><span class="sxs-lookup"><span data-stu-id="2e239-181">Assigned Products</span></span>
- <span data-ttu-id="2e239-182">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="2e239-182">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="2e239-183">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2e239-183">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2e239-184">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e239-184">Request</span></span>

<span data-ttu-id="2e239-185">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2e239-185">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="2e239-186">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e239-186">Response</span></span>

<span data-ttu-id="2e239-187">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2e239-187">The following is an example of the response.</span></span>

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

<span data-ttu-id="2e239-188">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="2e239-188">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Total Peer-to-peer Session Count,Total Organized Conference Count,Total Participated Conference Count,Peer-to-peer Last Activity Date,Organized Conference Last Activity Date,Participated Conference Last Activity Date,Peer-to-peer IM Count,Peer-to-peer Audio Count,Peer-to-peer Audio Minutes,Peer-to-peer Video Count,Peer-to-peer Video Minutes,Peer-to-peer App Sharing Count,Peer-to-peer File Transfer Count,Organized Conference IM Count,Organized Conference Audio/Video Count,Organized Conference Audio/Video Minutes,Organized Conference App Sharing Count,Organized Conference Web Count,Organized Conference Dial-in/out 3rd Party Count,Organized Conference Dial-in/out Microsoft Count,Organized Conference Dial-in Microsoft Minutes,Organized Conference Dial-out Microsoft Minutes,Paricipated Conference IM Count,Participated Conference Audio/Video Count,Participated Conference Audio/Video Minutes,Participated Conference App Sharing Count,Participated Conference Web Count,Participated Conference Dial-in/out 3rd Party Count,Assigned Products,Report Period
```