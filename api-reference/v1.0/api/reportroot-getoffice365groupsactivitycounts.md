---
title: 'reportRoot: getOffice365GroupsActivityCounts'
description: Rufen Sie die Anzahl der Gruppenaktivitäten für Gruppenarbeitslasten ab.
ms.openlocfilehash: 02bb861dbd26981d0d9190a3d82f2693f4ad3752
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017318"
---
# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="b7eb3-103">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="b7eb3-103">reportRoot: getOffice365GroupsActivityCounts</span></span>

<span data-ttu-id="b7eb3-104">Rufen Sie die Anzahl der Gruppenaktivitäten für Gruppenarbeitslasten ab.</span><span class="sxs-lookup"><span data-stu-id="b7eb3-104">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="b7eb3-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Office 365-Gruppen](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="b7eb3-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="b7eb3-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b7eb3-106">Permissions</span></span>

<span data-ttu-id="b7eb3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7eb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b7eb3-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b7eb3-109">Permission type</span></span>                        | <span data-ttu-id="b7eb3-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b7eb3-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b7eb3-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b7eb3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b7eb3-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7eb3-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b7eb3-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b7eb3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7eb3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b7eb3-114">Not supported.</span></span>                           |
| <span data-ttu-id="b7eb3-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b7eb3-115">Application</span></span>                            | <span data-ttu-id="b7eb3-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7eb3-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b7eb3-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b7eb3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b7eb3-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="b7eb3-118">Function parameters</span></span>

<span data-ttu-id="b7eb3-119">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="b7eb3-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b7eb3-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="b7eb3-120">Parameter</span></span> | <span data-ttu-id="b7eb3-121">Typ</span><span class="sxs-lookup"><span data-stu-id="b7eb3-121">Type</span></span>   | <span data-ttu-id="b7eb3-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b7eb3-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b7eb3-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="b7eb3-123">period</span></span>    | <span data-ttu-id="b7eb3-124">string</span><span class="sxs-lookup"><span data-stu-id="b7eb3-124">string</span></span> | <span data-ttu-id="b7eb3-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="b7eb3-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b7eb3-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="b7eb3-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b7eb3-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="b7eb3-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b7eb3-128">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="b7eb3-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="b7eb3-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b7eb3-129">Request headers</span></span>

| <span data-ttu-id="b7eb3-130">Name</span><span class="sxs-lookup"><span data-stu-id="b7eb3-130">Name</span></span>          | <span data-ttu-id="b7eb3-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b7eb3-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b7eb3-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7eb3-132">Authorization</span></span> | <span data-ttu-id="b7eb3-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b7eb3-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b7eb3-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b7eb3-135">If-None-Match</span></span> | <span data-ttu-id="b7eb3-136">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b7eb3-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b7eb3-137">Optional.</span><span class="sxs-lookup"><span data-stu-id="b7eb3-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b7eb3-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="b7eb3-138">Response</span></span>

<span data-ttu-id="b7eb3-139">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="b7eb3-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b7eb3-140">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b7eb3-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b7eb3-141">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="b7eb3-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b7eb3-142">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="b7eb3-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b7eb3-143">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="b7eb3-143">Report Refresh Date</span></span>
- <span data-ttu-id="b7eb3-144">Empfangene Exchange-E-Mails</span><span class="sxs-lookup"><span data-stu-id="b7eb3-144">Exchange Emails Received</span></span>
- <span data-ttu-id="b7eb3-145">Veröffentlichte Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="b7eb3-145">Yammer Messages Posted</span></span>
- <span data-ttu-id="b7eb3-146">Gelesene Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="b7eb3-146">Yammer Messages Read</span></span>
- <span data-ttu-id="b7eb3-147">Gelikte Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="b7eb3-147">Yammer Messages Liked</span></span>
- <span data-ttu-id="b7eb3-148">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="b7eb3-148">Report Date</span></span>
- <span data-ttu-id="b7eb3-149">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="b7eb3-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b7eb3-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b7eb3-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b7eb3-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b7eb3-151">Request</span></span>

<span data-ttu-id="b7eb3-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b7eb3-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="b7eb3-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="b7eb3-153">Response</span></span>

<span data-ttu-id="b7eb3-154">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b7eb3-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="b7eb3-155">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="b7eb3-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Emails Received,Yammer Messages Posted,Yammer Messages Read,Yammer Messages Liked,Report Date,Report Period
```