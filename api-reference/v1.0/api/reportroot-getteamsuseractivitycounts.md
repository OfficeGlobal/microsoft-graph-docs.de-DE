---
title: 'reportRoot: getTeamsUserActivityCounts'
description: Diese Methode ruft die Anzahl von Microsoft Teams-Aktivitäten nach Aktivitätstyp ab. Die Aktivitätstypen sind Chatnachricht, private Chatnachricht, Anruf und Besprechung.
ms.openlocfilehash: 58d0ddd884fed70e9fc5cbdd1c3d97c8a5463ccc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019617"
---
# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="c8794-104">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="c8794-104">reportRoot: getTeamsUserActivityCounts</span></span>

<span data-ttu-id="c8794-105">Diese Methode ruft die Anzahl von Microsoft Teams-Aktivitäten nach Aktivitätstyp ab.</span><span class="sxs-lookup"><span data-stu-id="c8794-105">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="c8794-106">Die Aktivitätstypen sind Chatnachricht, private Chatnachricht, Anruf und Besprechung.</span><span class="sxs-lookup"><span data-stu-id="c8794-106">The activity types are team chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8794-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c8794-107">Permissions</span></span>

<span data-ttu-id="c8794-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8794-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c8794-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c8794-110">Permission type</span></span>                        | <span data-ttu-id="c8794-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c8794-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c8794-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c8794-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c8794-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8794-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c8794-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c8794-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8794-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8794-115">Not supported.</span></span>                           |
| <span data-ttu-id="c8794-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c8794-116">Application</span></span>                            | <span data-ttu-id="c8794-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8794-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c8794-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8794-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c8794-119">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="c8794-119">Function parameters</span></span>

<span data-ttu-id="c8794-120">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="c8794-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c8794-121">Parameter</span><span class="sxs-lookup"><span data-stu-id="c8794-121">Parameter</span></span> | <span data-ttu-id="c8794-122">Typ</span><span class="sxs-lookup"><span data-stu-id="c8794-122">Type</span></span>   | <span data-ttu-id="c8794-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c8794-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c8794-124">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="c8794-124">period</span></span>    | <span data-ttu-id="c8794-125">string</span><span class="sxs-lookup"><span data-stu-id="c8794-125">string</span></span> | <span data-ttu-id="c8794-126">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="c8794-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c8794-127">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="c8794-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c8794-128">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="c8794-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c8794-129">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="c8794-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c8794-130">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c8794-130">Request headers</span></span>

| <span data-ttu-id="c8794-131">Name</span><span class="sxs-lookup"><span data-stu-id="c8794-131">Name</span></span>          | <span data-ttu-id="c8794-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c8794-132">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c8794-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8794-133">Authorization</span></span> | <span data-ttu-id="c8794-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c8794-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c8794-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8794-136">Response</span></span>

<span data-ttu-id="c8794-137">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="c8794-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c8794-138">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c8794-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c8794-139">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="c8794-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c8794-140">Die CSV-Datei verfügt über die folgenden Spaltenheader:</span><span class="sxs-lookup"><span data-stu-id="c8794-140">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="c8794-141">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="c8794-141">Report Refresh Date</span></span>
- <span data-ttu-id="c8794-142">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="c8794-142">Report Date</span></span>
- <span data-ttu-id="c8794-143">Team-Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="c8794-143">Team Chat Messages</span></span>
- <span data-ttu-id="c8794-144">Private Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="c8794-144">Private Chat Messages</span></span>
- <span data-ttu-id="c8794-145">Anrufe</span><span class="sxs-lookup"><span data-stu-id="c8794-145">Calls</span></span>
- <span data-ttu-id="c8794-146">Meetings</span><span class="sxs-lookup"><span data-stu-id="c8794-146">Meetings</span></span>
- <span data-ttu-id="c8794-147">Report Period</span><span class="sxs-lookup"><span data-stu-id="c8794-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="c8794-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c8794-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c8794-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8794-149">Request</span></span>

<span data-ttu-id="c8794-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c8794-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="c8794-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8794-151">Response</span></span>

<span data-ttu-id="c8794-152">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c8794-152">The following is an example of the response.</span></span>

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
<span data-ttu-id="c8794-153">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="c8794-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Report Period
```
