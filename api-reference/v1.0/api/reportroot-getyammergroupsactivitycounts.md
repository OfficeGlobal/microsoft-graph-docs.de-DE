---
title: 'reportRoot: getYammerGroupsActivityCounts'
description: Rufen Sie die Anzahl der in Gruppen veröffentlichten, gelesenen und gelikten Yammer-Nachrichten ab.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d1509747798507d10588f05ebeb4d9b5efec2b97
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577277"
---
# <a name="reportroot-getyammergroupsactivitycounts"></a><span data-ttu-id="5d7b5-103">reportRoot: getYammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="5d7b5-103">reportRoot: getYammerGroupsActivityCounts</span></span>

<span data-ttu-id="5d7b5-104">Rufen Sie die Anzahl der in Gruppen veröffentlichten, gelesenen und gelikten Yammer-Nachrichten ab.</span><span class="sxs-lookup"><span data-stu-id="5d7b5-104">Get the number of Yammer messages posted, read, and liked in groups.</span></span>

> <span data-ttu-id="5d7b5-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Gruppenaktivität](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="5d7b5-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="5d7b5-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5d7b5-106">Permissions</span></span>

<span data-ttu-id="5d7b5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d7b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5d7b5-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5d7b5-109">Permission type</span></span>                        | <span data-ttu-id="5d7b5-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5d7b5-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5d7b5-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5d7b5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5d7b5-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d7b5-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5d7b5-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5d7b5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d7b5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5d7b5-114">Not supported.</span></span>                           |
| <span data-ttu-id="5d7b5-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5d7b5-115">Application</span></span>                            | <span data-ttu-id="5d7b5-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d7b5-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5d7b5-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d7b5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="5d7b5-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="5d7b5-118">Function parameters</span></span>

<span data-ttu-id="5d7b5-119">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="5d7b5-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5d7b5-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="5d7b5-120">Parameter</span></span> | <span data-ttu-id="5d7b5-121">Typ</span><span class="sxs-lookup"><span data-stu-id="5d7b5-121">Type</span></span>   | <span data-ttu-id="5d7b5-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d7b5-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5d7b5-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="5d7b5-123">period</span></span>    | <span data-ttu-id="5d7b5-124">string</span><span class="sxs-lookup"><span data-stu-id="5d7b5-124">string</span></span> | <span data-ttu-id="5d7b5-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="5d7b5-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5d7b5-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="5d7b5-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5d7b5-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="5d7b5-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5d7b5-128">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="5d7b5-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="5d7b5-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5d7b5-129">Request headers</span></span>

| <span data-ttu-id="5d7b5-130">Name</span><span class="sxs-lookup"><span data-stu-id="5d7b5-130">Name</span></span>          | <span data-ttu-id="5d7b5-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d7b5-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="5d7b5-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d7b5-132">Authorization</span></span> | <span data-ttu-id="5d7b5-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5d7b5-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="5d7b5-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="5d7b5-135">If-None-Match</span></span> | <span data-ttu-id="5d7b5-136">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5d7b5-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="5d7b5-137">Optional.</span><span class="sxs-lookup"><span data-stu-id="5d7b5-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5d7b5-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d7b5-138">Response</span></span>

<span data-ttu-id="5d7b5-139">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="5d7b5-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5d7b5-140">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5d7b5-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5d7b5-141">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="5d7b5-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5d7b5-142">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="5d7b5-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5d7b5-143">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="5d7b5-143">Report Refresh Date</span></span>
- <span data-ttu-id="5d7b5-144">Gelikt</span><span class="sxs-lookup"><span data-stu-id="5d7b5-144">Liked</span></span>
- <span data-ttu-id="5d7b5-145">Gepostet</span><span class="sxs-lookup"><span data-stu-id="5d7b5-145">Posted</span></span>
- <span data-ttu-id="5d7b5-146">Gelesen</span><span class="sxs-lookup"><span data-stu-id="5d7b5-146">Read</span></span>
- <span data-ttu-id="5d7b5-147">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="5d7b5-147">Report Date</span></span>
- <span data-ttu-id="5d7b5-148">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="5d7b5-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="5d7b5-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5d7b5-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5d7b5-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5d7b5-150">Request</span></span>

<span data-ttu-id="5d7b5-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5d7b5-151">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="5d7b5-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="5d7b5-152">Response</span></span>

<span data-ttu-id="5d7b5-153">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5d7b5-153">The following is an example of the response.</span></span>

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

<span data-ttu-id="5d7b5-154">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="5d7b5-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
```
