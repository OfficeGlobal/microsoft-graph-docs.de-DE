---
title: 'reportRoot: getSkypeForBusinessActivityCounts'
description: Rufen Sie die Trends dazu ab, wie viele Benutzer Konferenzsitzungen, die in Ihrem Unternehmen mit Skype for Business abgehalten wurden, organisiert und daran teilgenommen haben. Der Bericht enthält auch die Anzahl von Peer-to-Peer-Sitzungen.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 320cc1743c854d2569bfb651da386f2529002f5c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574635"
---
# <a name="reportroot-getskypeforbusinessactivitycounts"></a><span data-ttu-id="ee48a-104">reportRoot: getSkypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="ee48a-104">reportRoot: getSkypeForBusinessActivityCounts</span></span>

<span data-ttu-id="ee48a-105">Rufen Sie die Trends dazu ab, wie viele Benutzer Konferenzsitzungen, die in Ihrem Unternehmen mit Skype for Business abgehalten wurden, organisiert und daran teilgenommen haben.</span><span class="sxs-lookup"><span data-stu-id="ee48a-105">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="ee48a-106">Der Bericht enthält auch die Anzahl von Peer-to-Peer-Sitzungen.</span><span class="sxs-lookup"><span data-stu-id="ee48a-106">The report also includes the number of peer-to-peer sessions.</span></span>

> <span data-ttu-id="ee48a-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Aktivität](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="ee48a-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="ee48a-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ee48a-108">Permissions</span></span>

<span data-ttu-id="ee48a-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee48a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ee48a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ee48a-111">Permission type</span></span>                        | <span data-ttu-id="ee48a-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ee48a-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ee48a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ee48a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ee48a-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee48a-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ee48a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ee48a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee48a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ee48a-116">Not supported.</span></span>                           |
| <span data-ttu-id="ee48a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ee48a-117">Application</span></span>                            | <span data-ttu-id="ee48a-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee48a-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ee48a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ee48a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ee48a-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="ee48a-120">Function parameters</span></span>

<span data-ttu-id="ee48a-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="ee48a-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ee48a-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="ee48a-122">Parameter</span></span> | <span data-ttu-id="ee48a-123">Typ</span><span class="sxs-lookup"><span data-stu-id="ee48a-123">Type</span></span>   | <span data-ttu-id="ee48a-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee48a-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ee48a-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="ee48a-125">period</span></span>    | <span data-ttu-id="ee48a-126">string</span><span class="sxs-lookup"><span data-stu-id="ee48a-126">string</span></span> | <span data-ttu-id="ee48a-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="ee48a-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ee48a-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="ee48a-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ee48a-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="ee48a-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ee48a-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="ee48a-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="ee48a-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ee48a-131">Request headers</span></span>

| <span data-ttu-id="ee48a-132">Name</span><span class="sxs-lookup"><span data-stu-id="ee48a-132">Name</span></span>          | <span data-ttu-id="ee48a-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee48a-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ee48a-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee48a-134">Authorization</span></span> | <span data-ttu-id="ee48a-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ee48a-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ee48a-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ee48a-137">If-None-Match</span></span> | <span data-ttu-id="ee48a-138">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ee48a-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ee48a-139">Optional.</span><span class="sxs-lookup"><span data-stu-id="ee48a-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ee48a-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="ee48a-140">Response</span></span>

<span data-ttu-id="ee48a-141">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="ee48a-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ee48a-142">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ee48a-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ee48a-143">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="ee48a-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ee48a-144">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="ee48a-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ee48a-145">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="ee48a-145">Report Refresh Date</span></span>
- <span data-ttu-id="ee48a-146">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="ee48a-146">Report Date</span></span>
- <span data-ttu-id="ee48a-147">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="ee48a-147">Report Period</span></span>
- <span data-ttu-id="ee48a-148">Peer-to-Peer</span><span class="sxs-lookup"><span data-stu-id="ee48a-148">Peer-to-peer</span></span>
- <span data-ttu-id="ee48a-149">Organisiert</span><span class="sxs-lookup"><span data-stu-id="ee48a-149">Organized</span></span>
- <span data-ttu-id="ee48a-150">Teilgenommen</span><span class="sxs-lookup"><span data-stu-id="ee48a-150">Participated</span></span>

## <a name="example"></a><span data-ttu-id="ee48a-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ee48a-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ee48a-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ee48a-152">Request</span></span>

<span data-ttu-id="ee48a-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ee48a-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="ee48a-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="ee48a-154">Response</span></span>

<span data-ttu-id="ee48a-155">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ee48a-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="ee48a-156">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="ee48a-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Peer-to-peer,Organized,Participated
```
