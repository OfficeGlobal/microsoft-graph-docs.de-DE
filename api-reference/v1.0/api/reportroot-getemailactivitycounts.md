---
title: 'reportRoot: getEmailActivityCounts'
description: Ermöglicht es Ihnen, einen Überblick über die E-Mail-Aktivitäten (z. B. wie viele E-Mails versendet, gelesen und empfangen wurden) in Ihrer Organisation zu gewinnen.
ms.openlocfilehash: 1cd15a10959c3ec4da11b879acf5c617b8cb22dd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016701"
---
# <a name="reportroot-getemailactivitycounts"></a><span data-ttu-id="c6346-103">reportRoot: getEmailActivityCounts</span><span class="sxs-lookup"><span data-stu-id="c6346-103">reportRoot: getEmailActivityCounts</span></span>

<span data-ttu-id="c6346-104">Ermöglicht es Ihnen, einen Überblick über die E-Mail-Aktivitäten (z. B. wie viele E-Mails versendet, gelesen und empfangen wurden) in Ihrer Organisation zu gewinnen.</span><span class="sxs-lookup"><span data-stu-id="c6346-104">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span>

> <span data-ttu-id="c6346-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – E-Mail-Aktivität](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="c6346-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="c6346-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c6346-106">Permissions</span></span>

<span data-ttu-id="c6346-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6346-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c6346-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c6346-109">Permission type</span></span>                        | <span data-ttu-id="c6346-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c6346-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c6346-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c6346-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c6346-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6346-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c6346-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c6346-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6346-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c6346-114">Not supported.</span></span>                           |
| <span data-ttu-id="c6346-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c6346-115">Application</span></span>                            | <span data-ttu-id="c6346-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6346-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c6346-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c6346-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c6346-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="c6346-118">Function parameters</span></span>

<span data-ttu-id="c6346-119">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="c6346-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c6346-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="c6346-120">Parameter</span></span> | <span data-ttu-id="c6346-121">Typ</span><span class="sxs-lookup"><span data-stu-id="c6346-121">Type</span></span>   | <span data-ttu-id="c6346-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6346-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c6346-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="c6346-123">period</span></span>    | <span data-ttu-id="c6346-124">string</span><span class="sxs-lookup"><span data-stu-id="c6346-124">string</span></span> | <span data-ttu-id="c6346-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="c6346-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c6346-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="c6346-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c6346-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="c6346-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c6346-128">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="c6346-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c6346-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c6346-129">Request headers</span></span>

| <span data-ttu-id="c6346-130">Name</span><span class="sxs-lookup"><span data-stu-id="c6346-130">Name</span></span>          | <span data-ttu-id="c6346-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6346-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="c6346-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6346-132">Authorization</span></span> | <span data-ttu-id="c6346-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c6346-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="c6346-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="c6346-135">If-None-Match</span></span> | <span data-ttu-id="c6346-136">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c6346-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="c6346-137">Optional.</span><span class="sxs-lookup"><span data-stu-id="c6346-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c6346-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="c6346-138">Response</span></span>

<span data-ttu-id="c6346-139">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="c6346-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c6346-140">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c6346-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c6346-141">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="c6346-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c6346-142">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="c6346-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c6346-143">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="c6346-143">Report Refresh Date</span></span>
- <span data-ttu-id="c6346-144">Senden</span><span class="sxs-lookup"><span data-stu-id="c6346-144">Send</span></span>
- <span data-ttu-id="c6346-145">Empfangen</span><span class="sxs-lookup"><span data-stu-id="c6346-145">Receive</span></span>
- <span data-ttu-id="c6346-146">Lesen</span><span class="sxs-lookup"><span data-stu-id="c6346-146">Read</span></span>
- <span data-ttu-id="c6346-147">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="c6346-147">Report Date</span></span>
- <span data-ttu-id="c6346-148">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="c6346-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="c6346-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c6346-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c6346-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c6346-150">Request</span></span>

<span data-ttu-id="c6346-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c6346-151">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="c6346-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="c6346-152">Response</span></span>

<span data-ttu-id="c6346-153">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c6346-153">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c6346-154">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="c6346-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "ignored"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Send,Receive,Read,Report Date,Report Period
```