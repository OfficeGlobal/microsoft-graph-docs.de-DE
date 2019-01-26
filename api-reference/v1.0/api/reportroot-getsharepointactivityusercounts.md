---
title: 'reportRoot: getSharePointActivityUserCounts'
description: Rufen Sie die Anzahl der aktiven Benutzer ab. Ein Benutzer wird als aktiv betrachtet, wenn er innerhalb des angegebenen Zeitraums eine Dateiaktivität ausgeführt (speichern, synchronisieren, ändern oder freigeben) oder eine Seite besucht hat.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 09b0b823858d34212aa0580c3c85f645734bf901
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574369"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="e7300-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="e7300-104">reportRoot: getSharePointActivityUserCounts</span></span>

<span data-ttu-id="e7300-105">Rufen Sie die Anzahl der aktiven Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="e7300-105">Get the trend in the number of active users.</span></span> <span data-ttu-id="e7300-106">Ein Benutzer wird als aktiv betrachtet, wenn er innerhalb des angegebenen Zeitraums eine Dateiaktivität ausgeführt (speichern, synchronisieren, ändern oder freigeben) oder eine Seite besucht hat.</span><span class="sxs-lookup"><span data-stu-id="e7300-106">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="e7300-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – SharePoint-Aktivität](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="e7300-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="e7300-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e7300-108">Permissions</span></span>

<span data-ttu-id="e7300-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7300-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e7300-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e7300-111">Permission type</span></span>                        | <span data-ttu-id="e7300-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e7300-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e7300-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e7300-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e7300-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7300-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e7300-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e7300-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7300-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e7300-116">Not supported.</span></span>                           |
| <span data-ttu-id="e7300-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e7300-117">Application</span></span>                            | <span data-ttu-id="e7300-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7300-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e7300-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e7300-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e7300-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="e7300-120">Function parameters</span></span>

<span data-ttu-id="e7300-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="e7300-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e7300-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="e7300-122">Parameter</span></span> | <span data-ttu-id="e7300-123">Typ</span><span class="sxs-lookup"><span data-stu-id="e7300-123">Type</span></span>   | <span data-ttu-id="e7300-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e7300-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e7300-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="e7300-125">period</span></span>    | <span data-ttu-id="e7300-126">string</span><span class="sxs-lookup"><span data-stu-id="e7300-126">string</span></span> | <span data-ttu-id="e7300-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="e7300-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e7300-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="e7300-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e7300-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="e7300-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e7300-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="e7300-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="e7300-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e7300-131">Request headers</span></span>

| <span data-ttu-id="e7300-132">Name</span><span class="sxs-lookup"><span data-stu-id="e7300-132">Name</span></span>          | <span data-ttu-id="e7300-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e7300-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="e7300-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7300-134">Authorization</span></span> | <span data-ttu-id="e7300-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e7300-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="e7300-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="e7300-137">If-None-Match</span></span> | <span data-ttu-id="e7300-138">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e7300-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="e7300-139">Optional.</span><span class="sxs-lookup"><span data-stu-id="e7300-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="e7300-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="e7300-140">Response</span></span>

<span data-ttu-id="e7300-141">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="e7300-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e7300-142">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e7300-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e7300-143">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="e7300-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e7300-144">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="e7300-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e7300-145">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="e7300-145">Report Refresh Date</span></span>
- <span data-ttu-id="e7300-146">Besuchte Seite</span><span class="sxs-lookup"><span data-stu-id="e7300-146">Visited Page</span></span>
- <span data-ttu-id="e7300-147">Angezeigt oder Bearbeitet</span><span class="sxs-lookup"><span data-stu-id="e7300-147">Viewed Or Edited</span></span>
- <span data-ttu-id="e7300-148">Synchronisiert</span><span class="sxs-lookup"><span data-stu-id="e7300-148">Synced</span></span>
- <span data-ttu-id="e7300-149">Intern freigegeben</span><span class="sxs-lookup"><span data-stu-id="e7300-149">Shared Internally</span></span>
- <span data-ttu-id="e7300-150">Extern freigegeben</span><span class="sxs-lookup"><span data-stu-id="e7300-150">Shared Externally</span></span>
- <span data-ttu-id="e7300-151">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="e7300-151">Report Date</span></span>
- <span data-ttu-id="e7300-152">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="e7300-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="e7300-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e7300-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e7300-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e7300-154">Request</span></span>

<span data-ttu-id="e7300-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e7300-155">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="e7300-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="e7300-156">Response</span></span>

<span data-ttu-id="e7300-157">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e7300-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="e7300-158">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="e7300-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```
