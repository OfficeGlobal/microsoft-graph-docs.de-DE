---
title: 'reportRoot: getMailboxUsageMailboxCounts'
description: Rufen Sie die Gesamtzahl der Postfächer in Ihrem Unternehmen ab und erfahren Sie, wie viele Postfächer im Berichtszeitraum täglich aktiv sind. Ein Postfach wird als aktiv betrachtet, wenn der Benutzer eine E-Mail sendet oder liest.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4896ca7cbe76ec9b0d730cc67faaafb78023ebae
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572108"
---
# <a name="reportroot-getmailboxusagemailboxcounts"></a><span data-ttu-id="e1931-104">reportRoot: getMailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="e1931-104">reportRoot: getMailboxUsageMailboxCounts</span></span>

<span data-ttu-id="e1931-105">Rufen Sie die Gesamtzahl der Postfächer in Ihrem Unternehmen ab und erfahren Sie, wie viele Postfächer im Berichtszeitraum täglich aktiv sind.</span><span class="sxs-lookup"><span data-stu-id="e1931-105">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="e1931-106">Ein Postfach wird als aktiv betrachtet, wenn der Benutzer eine E-Mail sendet oder liest.</span><span class="sxs-lookup"><span data-stu-id="e1931-106">A mailbox is considered active if the user sent or read any email.</span></span>

> <span data-ttu-id="e1931-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Postfachnutzung](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="e1931-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="e1931-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e1931-108">Permissions</span></span>

<span data-ttu-id="e1931-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1931-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e1931-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e1931-111">Permission type</span></span>                        | <span data-ttu-id="e1931-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e1931-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e1931-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e1931-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e1931-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1931-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e1931-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e1931-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1931-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e1931-116">Not supported.</span></span>                           |
| <span data-ttu-id="e1931-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e1931-117">Application</span></span>                            | <span data-ttu-id="e1931-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1931-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e1931-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1931-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e1931-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="e1931-120">Function parameters</span></span>

<span data-ttu-id="e1931-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="e1931-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e1931-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="e1931-122">Parameter</span></span> | <span data-ttu-id="e1931-123">Typ</span><span class="sxs-lookup"><span data-stu-id="e1931-123">Type</span></span>   | <span data-ttu-id="e1931-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e1931-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e1931-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="e1931-125">period</span></span>    | <span data-ttu-id="e1931-126">string</span><span class="sxs-lookup"><span data-stu-id="e1931-126">string</span></span> | <span data-ttu-id="e1931-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="e1931-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e1931-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="e1931-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e1931-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="e1931-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e1931-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="e1931-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="e1931-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e1931-131">Request headers</span></span>

| <span data-ttu-id="e1931-132">Name</span><span class="sxs-lookup"><span data-stu-id="e1931-132">Name</span></span>          | <span data-ttu-id="e1931-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e1931-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="e1931-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1931-134">Authorization</span></span> | <span data-ttu-id="e1931-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e1931-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="e1931-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="e1931-137">If-None-Match</span></span> | <span data-ttu-id="e1931-138">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e1931-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="e1931-139">Optional.</span><span class="sxs-lookup"><span data-stu-id="e1931-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="e1931-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1931-140">Response</span></span>

<span data-ttu-id="e1931-141">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="e1931-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e1931-142">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e1931-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e1931-143">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="e1931-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e1931-144">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="e1931-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e1931-145">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="e1931-145">Report Refresh Date</span></span>
- <span data-ttu-id="e1931-146">Gesamt</span><span class="sxs-lookup"><span data-stu-id="e1931-146">Total</span></span>
- <span data-ttu-id="e1931-147">Aktiv</span><span class="sxs-lookup"><span data-stu-id="e1931-147">Active</span></span>
- <span data-ttu-id="e1931-148">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="e1931-148">Report Date</span></span>
- <span data-ttu-id="e1931-149">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="e1931-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="e1931-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e1931-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e1931-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e1931-151">Request</span></span>

<span data-ttu-id="e1931-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e1931-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusagemailboxcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageMailboxCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="e1931-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="e1931-153">Response</span></span>

<span data-ttu-id="e1931-154">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e1931-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="e1931-155">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="e1931-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```
