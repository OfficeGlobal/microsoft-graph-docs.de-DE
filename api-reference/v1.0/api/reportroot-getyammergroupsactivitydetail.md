---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: Rufen Sie Details zur Yammer-Gruppenaktivität nach Gruppe ab.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 538b0f28591a2b7b301f6a1dafd0c6d58d11460a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945608"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="bbffe-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="bbffe-103">reportRoot: getYammerGroupsActivityDetail</span></span>

<span data-ttu-id="bbffe-104">Rufen Sie Details zur Yammer-Gruppenaktivität nach Gruppe ab.</span><span class="sxs-lookup"><span data-stu-id="bbffe-104">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="bbffe-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Gruppenaktivität](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="bbffe-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="bbffe-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bbffe-106">Permissions</span></span>

<span data-ttu-id="bbffe-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbffe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bbffe-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bbffe-109">Permission type</span></span>                        | <span data-ttu-id="bbffe-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bbffe-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bbffe-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bbffe-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bbffe-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbffe-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bbffe-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bbffe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbffe-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bbffe-114">Not supported.</span></span>                           |
| <span data-ttu-id="bbffe-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bbffe-115">Application</span></span>                            | <span data-ttu-id="bbffe-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbffe-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bbffe-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bbffe-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="bbffe-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="bbffe-118">Function parameters</span></span>

<span data-ttu-id="bbffe-119">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="bbffe-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="bbffe-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="bbffe-120">Parameter</span></span> | <span data-ttu-id="bbffe-121">Typ</span><span class="sxs-lookup"><span data-stu-id="bbffe-121">Type</span></span>   | <span data-ttu-id="bbffe-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bbffe-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bbffe-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="bbffe-123">period</span></span>    | <span data-ttu-id="bbffe-124">string</span><span class="sxs-lookup"><span data-stu-id="bbffe-124">string</span></span> | <span data-ttu-id="bbffe-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="bbffe-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bbffe-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="bbffe-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bbffe-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="bbffe-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="bbffe-128">date</span><span class="sxs-lookup"><span data-stu-id="bbffe-128">date</span></span>      | <span data-ttu-id="bbffe-129">Datum</span><span class="sxs-lookup"><span data-stu-id="bbffe-129">Date</span></span>   | <span data-ttu-id="bbffe-130">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="bbffe-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="bbffe-131">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="bbffe-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="bbffe-132">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="bbffe-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="bbffe-133">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="bbffe-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bbffe-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bbffe-134">Request headers</span></span>

| <span data-ttu-id="bbffe-135">Name</span><span class="sxs-lookup"><span data-stu-id="bbffe-135">Name</span></span>          | <span data-ttu-id="bbffe-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bbffe-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="bbffe-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbffe-137">Authorization</span></span> | <span data-ttu-id="bbffe-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bbffe-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="bbffe-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="bbffe-140">If-None-Match</span></span> | <span data-ttu-id="bbffe-141">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bbffe-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="bbffe-142">Optional.</span><span class="sxs-lookup"><span data-stu-id="bbffe-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="bbffe-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="bbffe-143">Response</span></span>

<span data-ttu-id="bbffe-144">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="bbffe-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bbffe-145">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bbffe-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bbffe-146">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="bbffe-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bbffe-147">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="bbffe-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bbffe-148">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="bbffe-148">Report Refresh Date</span></span>
- <span data-ttu-id="bbffe-149">Gruppenanzeigename</span><span class="sxs-lookup"><span data-stu-id="bbffe-149">Group Display Name</span></span>
- <span data-ttu-id="bbffe-150">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="bbffe-150">Is Deleted</span></span>
- <span data-ttu-id="bbffe-151">Besitzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="bbffe-151">Owner Principal Name</span></span>
- <span data-ttu-id="bbffe-152">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="bbffe-152">Last Activity Date</span></span>
- <span data-ttu-id="bbffe-153">Gruppentyp</span><span class="sxs-lookup"><span data-stu-id="bbffe-153">Group Type</span></span>
- <span data-ttu-id="bbffe-154">Mit Office 365 verbunden</span><span class="sxs-lookup"><span data-stu-id="bbffe-154">Office 365 Connected</span></span>
- <span data-ttu-id="bbffe-155">Mitgliederzahl</span><span class="sxs-lookup"><span data-stu-id="bbffe-155">Member Count</span></span>
- <span data-ttu-id="bbffe-156">Anzahl veröffentlicht</span><span class="sxs-lookup"><span data-stu-id="bbffe-156">Posted Count</span></span>
- <span data-ttu-id="bbffe-157">Anzahl gelesen</span><span class="sxs-lookup"><span data-stu-id="bbffe-157">Read Count</span></span>
- <span data-ttu-id="bbffe-158">Anzahl gelikt</span><span class="sxs-lookup"><span data-stu-id="bbffe-158">Liked Count</span></span>
- <span data-ttu-id="bbffe-159">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="bbffe-159">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="bbffe-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bbffe-160">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bbffe-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bbffe-161">Request</span></span>

<span data-ttu-id="bbffe-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bbffe-162">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="bbffe-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="bbffe-163">Response</span></span>

<span data-ttu-id="bbffe-164">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bbffe-164">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="bbffe-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bbffe-165">Request</span></span>
<span data-ttu-id="bbffe-166">Wenn aufgerufen, wobei ein `date`, der Bericht auf das angegebene Datum der Aktivität Gültigkeitsbereich ist.</span><span class="sxs-lookup"><span data-stu-id="bbffe-166">If called with a `date`, the report is scoped to activity on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="bbffe-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="bbffe-167">Response</span></span>

<span data-ttu-id="bbffe-168">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bbffe-168">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="bbffe-169">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="bbffe-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "ignored"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
```
