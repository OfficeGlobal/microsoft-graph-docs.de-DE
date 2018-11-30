---
title: 'reportRoot: getYammerActivityCounts'
description: Gewinnen Sie einen Eindruck der Yammer-Aktivitäten in Ihrer Organisation, indem Sie erfahren, wie viele Nachrichten gepostet, gelesen und gelikt wurden.
ms.openlocfilehash: 17813cd7365afce535c38f993d548a66fda77cc6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016754"
---
# <a name="reportroot-getyammeractivitycounts"></a><span data-ttu-id="d116a-103">reportRoot: getYammerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="d116a-103">reportRoot: getYammerActivityCounts</span></span>

<span data-ttu-id="d116a-104">Gewinnen Sie einen Eindruck der Yammer-Aktivitäten in Ihrer Organisation, indem Sie erfahren, wie viele Nachrichten gepostet, gelesen und gelikt wurden.</span><span class="sxs-lookup"><span data-stu-id="d116a-104">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span>

> <span data-ttu-id="d116a-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Aktivität](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="d116a-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="d116a-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d116a-106">Permissions</span></span>

<span data-ttu-id="d116a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d116a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d116a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d116a-109">Permission type</span></span>                        | <span data-ttu-id="d116a-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d116a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d116a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d116a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d116a-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d116a-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d116a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d116a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d116a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d116a-114">Not supported.</span></span>                           |
| <span data-ttu-id="d116a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d116a-115">Application</span></span>                            | <span data-ttu-id="d116a-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d116a-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d116a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d116a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="d116a-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="d116a-118">Function parameters</span></span>

<span data-ttu-id="d116a-119">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="d116a-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d116a-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="d116a-120">Parameter</span></span> | <span data-ttu-id="d116a-121">Typ</span><span class="sxs-lookup"><span data-stu-id="d116a-121">Type</span></span>   | <span data-ttu-id="d116a-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d116a-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d116a-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="d116a-123">period</span></span>    | <span data-ttu-id="d116a-124">string</span><span class="sxs-lookup"><span data-stu-id="d116a-124">string</span></span> | <span data-ttu-id="d116a-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="d116a-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d116a-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="d116a-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d116a-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="d116a-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d116a-128">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="d116a-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d116a-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d116a-129">Request headers</span></span>

| <span data-ttu-id="d116a-130">Name</span><span class="sxs-lookup"><span data-stu-id="d116a-130">Name</span></span>          | <span data-ttu-id="d116a-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d116a-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="d116a-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="d116a-132">Authorization</span></span> | <span data-ttu-id="d116a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d116a-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="d116a-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="d116a-135">If-None-Match</span></span> | <span data-ttu-id="d116a-136">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d116a-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="d116a-137">Optional.</span><span class="sxs-lookup"><span data-stu-id="d116a-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d116a-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="d116a-138">Response</span></span>

<span data-ttu-id="d116a-139">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="d116a-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d116a-140">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d116a-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d116a-141">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="d116a-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d116a-142">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="d116a-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d116a-143">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="d116a-143">Report Refresh Date</span></span>
- <span data-ttu-id="d116a-144">Gelikt</span><span class="sxs-lookup"><span data-stu-id="d116a-144">Liked</span></span>
- <span data-ttu-id="d116a-145">Gepostet</span><span class="sxs-lookup"><span data-stu-id="d116a-145">Posted</span></span>
- <span data-ttu-id="d116a-146">Gelesen</span><span class="sxs-lookup"><span data-stu-id="d116a-146">Read</span></span>
- <span data-ttu-id="d116a-147">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="d116a-147">Report Date</span></span>
- <span data-ttu-id="d116a-148">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="d116a-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="d116a-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d116a-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d116a-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d116a-150">Request</span></span>

<span data-ttu-id="d116a-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d116a-151">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammeractivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="d116a-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="d116a-152">Response</span></span>

<span data-ttu-id="d116a-153">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d116a-153">The following is an example of the response.</span></span>

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

<span data-ttu-id="d116a-154">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="d116a-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
```
