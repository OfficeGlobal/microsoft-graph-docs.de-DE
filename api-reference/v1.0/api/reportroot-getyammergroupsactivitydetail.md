---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: Rufen Sie Details zur Yammer-Gruppenaktivität nach Gruppe ab.
ms.openlocfilehash: 927d9511a5190b2aa5540c6046c8162e5fa5f9e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018185"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="7c167-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="7c167-103">reportRoot: getYammerGroupsActivityDetail</span></span>

<span data-ttu-id="7c167-104">Rufen Sie Details zur Yammer-Gruppenaktivität nach Gruppe ab.</span><span class="sxs-lookup"><span data-stu-id="7c167-104">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="7c167-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Gruppenaktivität](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="7c167-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="7c167-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7c167-106">Permissions</span></span>

<span data-ttu-id="7c167-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c167-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7c167-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7c167-109">Permission type</span></span>                        | <span data-ttu-id="7c167-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7c167-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7c167-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7c167-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7c167-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c167-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7c167-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7c167-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c167-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c167-114">Not supported.</span></span>                           |
| <span data-ttu-id="7c167-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7c167-115">Application</span></span>                            | <span data-ttu-id="7c167-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c167-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7c167-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c167-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="7c167-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="7c167-118">Function parameters</span></span>

<span data-ttu-id="7c167-119">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="7c167-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="7c167-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="7c167-120">Parameter</span></span> | <span data-ttu-id="7c167-121">Typ</span><span class="sxs-lookup"><span data-stu-id="7c167-121">Type</span></span>   | <span data-ttu-id="7c167-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c167-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7c167-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="7c167-123">period</span></span>    | <span data-ttu-id="7c167-124">string</span><span class="sxs-lookup"><span data-stu-id="7c167-124">string</span></span> | <span data-ttu-id="7c167-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="7c167-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7c167-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="7c167-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7c167-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="7c167-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="7c167-128">date</span><span class="sxs-lookup"><span data-stu-id="7c167-128">date</span></span>      | <span data-ttu-id="7c167-129">Datum</span><span class="sxs-lookup"><span data-stu-id="7c167-129">Date</span></span>   | <span data-ttu-id="7c167-130">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="7c167-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="7c167-131">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="7c167-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="7c167-132">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="7c167-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="7c167-133">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="7c167-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c167-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7c167-134">Request headers</span></span>

| <span data-ttu-id="7c167-135">Name</span><span class="sxs-lookup"><span data-stu-id="7c167-135">Name</span></span>          | <span data-ttu-id="7c167-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7c167-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="7c167-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c167-137">Authorization</span></span> | <span data-ttu-id="7c167-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7c167-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="7c167-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="7c167-140">If-None-Match</span></span> | <span data-ttu-id="7c167-141">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7c167-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="7c167-142">Optional.</span><span class="sxs-lookup"><span data-stu-id="7c167-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="7c167-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c167-143">Response</span></span>

<span data-ttu-id="7c167-144">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="7c167-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7c167-145">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7c167-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7c167-146">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="7c167-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7c167-147">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="7c167-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7c167-148">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="7c167-148">Report Refresh Date</span></span>
- <span data-ttu-id="7c167-149">Gruppenanzeigename</span><span class="sxs-lookup"><span data-stu-id="7c167-149">Group Display Name</span></span>
- <span data-ttu-id="7c167-150">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="7c167-150">Is Deleted</span></span>
- <span data-ttu-id="7c167-151">Besitzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="7c167-151">Owner Principal Name</span></span>
- <span data-ttu-id="7c167-152">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="7c167-152">Last Activity Date</span></span>
- <span data-ttu-id="7c167-153">Gruppentyp</span><span class="sxs-lookup"><span data-stu-id="7c167-153">Group Type</span></span>
- <span data-ttu-id="7c167-154">Mit Office 365 verbunden</span><span class="sxs-lookup"><span data-stu-id="7c167-154">Office 365 Connected</span></span>
- <span data-ttu-id="7c167-155">Mitgliederzahl</span><span class="sxs-lookup"><span data-stu-id="7c167-155">Member Count</span></span>
- <span data-ttu-id="7c167-156">Anzahl veröffentlicht</span><span class="sxs-lookup"><span data-stu-id="7c167-156">Posted Count</span></span>
- <span data-ttu-id="7c167-157">Anzahl gelesen</span><span class="sxs-lookup"><span data-stu-id="7c167-157">Read Count</span></span>
- <span data-ttu-id="7c167-158">Anzahl gelikt</span><span class="sxs-lookup"><span data-stu-id="7c167-158">Liked Count</span></span>
- <span data-ttu-id="7c167-159">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="7c167-159">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="7c167-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7c167-160">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7c167-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c167-161">Request</span></span>

<span data-ttu-id="7c167-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7c167-162">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="7c167-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c167-163">Response</span></span>

<span data-ttu-id="7c167-164">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7c167-164">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="7c167-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c167-165">Request</span></span>
<span data-ttu-id="7c167-166">Wenn aufgerufen, wobei ein `date`, der Bericht auf das angegebene Datum der Aktivität Gültigkeitsbereich ist.</span><span class="sxs-lookup"><span data-stu-id="7c167-166">If called with a `date`, the report is scoped to activity on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="7c167-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c167-167">Response</span></span>

<span data-ttu-id="7c167-168">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7c167-168">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7c167-169">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="7c167-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "ignored"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
```