---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: Abrufen von Details zur Microsoft Teams-Benutzeraktivität nach Benutzer.
ms.openlocfilehash: 6905f9a18627a9ebf3c63ca92c111d1518564a3e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017990"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="c235d-103">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="c235d-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

<span data-ttu-id="c235d-104">Abrufen von Details zur Microsoft Teams-Benutzeraktivität nach Benutzer.</span><span class="sxs-lookup"><span data-stu-id="c235d-104">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="c235d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c235d-105">Permissions</span></span>

<span data-ttu-id="c235d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c235d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c235d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c235d-108">Permission type</span></span>                        | <span data-ttu-id="c235d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c235d-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c235d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c235d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c235d-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c235d-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c235d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c235d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c235d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c235d-113">Not supported.</span></span>                           |
| <span data-ttu-id="c235d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c235d-114">Application</span></span>                            | <span data-ttu-id="c235d-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c235d-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c235d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c235d-116">HTTP request</span></span>

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='{period_value}')
GET /reports/getTeamsUserActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="c235d-117">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="c235d-117">Function parameters</span></span>

<span data-ttu-id="c235d-118">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="c235d-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="c235d-119">Parameter</span><span class="sxs-lookup"><span data-stu-id="c235d-119">Parameter</span></span> | <span data-ttu-id="c235d-120">Typ</span><span class="sxs-lookup"><span data-stu-id="c235d-120">Type</span></span>   | <span data-ttu-id="c235d-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c235d-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c235d-122">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="c235d-122">period</span></span>    | <span data-ttu-id="c235d-123">string</span><span class="sxs-lookup"><span data-stu-id="c235d-123">string</span></span> | <span data-ttu-id="c235d-124">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="c235d-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c235d-125">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="c235d-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c235d-126">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="c235d-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="c235d-127">date</span><span class="sxs-lookup"><span data-stu-id="c235d-127">date</span></span>      | <span data-ttu-id="c235d-128">Datum</span><span class="sxs-lookup"><span data-stu-id="c235d-128">Date</span></span>   | <span data-ttu-id="c235d-129">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="c235d-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="c235d-130">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="c235d-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="c235d-131">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="c235d-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="c235d-132">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="c235d-132">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c235d-133">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c235d-133">Request headers</span></span>

| <span data-ttu-id="c235d-134">Name</span><span class="sxs-lookup"><span data-stu-id="c235d-134">Name</span></span>          | <span data-ttu-id="c235d-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c235d-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c235d-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="c235d-136">Authorization</span></span> | <span data-ttu-id="c235d-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c235d-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c235d-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="c235d-139">Response</span></span>

<span data-ttu-id="c235d-140">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="c235d-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c235d-141">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c235d-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c235d-142">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="c235d-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c235d-143">Die CSV-Datei verfügt über die folgenden Spaltenheader:</span><span class="sxs-lookup"><span data-stu-id="c235d-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="c235d-144">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="c235d-144">Report Refresh Date</span></span>
- <span data-ttu-id="c235d-145">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="c235d-145">User Principal Name</span></span>
- <span data-ttu-id="c235d-146">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="c235d-146">Last Activity Date</span></span>
- <span data-ttu-id="c235d-147">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="c235d-147">Is Deleted</span></span>
- <span data-ttu-id="c235d-148">Gelöscht am</span><span class="sxs-lookup"><span data-stu-id="c235d-148">Deleted Date</span></span>
- <span data-ttu-id="c235d-149">Zugewiesene Produkte</span><span class="sxs-lookup"><span data-stu-id="c235d-149">Assigned Products</span></span>
- <span data-ttu-id="c235d-150">Anzahl der Team-Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="c235d-150">Team Chat Message Count</span></span>
- <span data-ttu-id="c235d-151">Anzahl der privaten Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="c235d-151">Private Chat Message Count</span></span>
- <span data-ttu-id="c235d-152">Anzahl der Anrufe</span><span class="sxs-lookup"><span data-stu-id="c235d-152">Call Count</span></span>
- <span data-ttu-id="c235d-153">Anzahl der Besprechung</span><span class="sxs-lookup"><span data-stu-id="c235d-153">Meeting Count</span></span>
- <span data-ttu-id="c235d-154">Andere Aktion</span><span class="sxs-lookup"><span data-stu-id="c235d-154">Has Other Action</span></span>
- <span data-ttu-id="c235d-155">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="c235d-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="c235d-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c235d-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c235d-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c235d-157">Request</span></span>

<span data-ttu-id="c235d-158">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c235d-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="c235d-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="c235d-159">Response</span></span>

<span data-ttu-id="c235d-160">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c235d-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="c235d-161">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="c235d-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Has Other Action,Report Period
```