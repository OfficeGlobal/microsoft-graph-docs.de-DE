---
title: 'reportRoot: getYammerDeviceUsageDistributionUserCounts'
description: Erhalten Sie die Anzahl der Benutzer nach Gerätetyp.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 749f24f7c24d3e903e00c5208133527741d8517c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930817"
---
# <a name="reportroot-getyammerdeviceusagedistributionusercounts"></a><span data-ttu-id="790d4-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="790d4-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="790d4-104">Erhalten Sie die Anzahl der Benutzer nach Gerätetyp.</span><span class="sxs-lookup"><span data-stu-id="790d4-104">Get the number of users by device type.</span></span>

> <span data-ttu-id="790d4-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Gerätenutzung](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="790d4-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="790d4-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="790d4-106">Permissions</span></span>

<span data-ttu-id="790d4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="790d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="790d4-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="790d4-109">Permission type</span></span>                        | <span data-ttu-id="790d4-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="790d4-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="790d4-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="790d4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="790d4-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="790d4-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="790d4-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="790d4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="790d4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="790d4-114">Not supported.</span></span>                           |
| <span data-ttu-id="790d4-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="790d4-115">Application</span></span>                            | <span data-ttu-id="790d4-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="790d4-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="790d4-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="790d4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="790d4-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="790d4-118">Function parameters</span></span>

<span data-ttu-id="790d4-119">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="790d4-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="790d4-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="790d4-120">Parameter</span></span> | <span data-ttu-id="790d4-121">Typ</span><span class="sxs-lookup"><span data-stu-id="790d4-121">Type</span></span>   | <span data-ttu-id="790d4-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="790d4-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="790d4-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="790d4-123">period</span></span>    | <span data-ttu-id="790d4-124">string</span><span class="sxs-lookup"><span data-stu-id="790d4-124">string</span></span> | <span data-ttu-id="790d4-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="790d4-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="790d4-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="790d4-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="790d4-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="790d4-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="790d4-128">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="790d4-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="790d4-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="790d4-129">Request headers</span></span>

| <span data-ttu-id="790d4-130">Name</span><span class="sxs-lookup"><span data-stu-id="790d4-130">Name</span></span>          | <span data-ttu-id="790d4-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="790d4-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="790d4-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="790d4-132">Authorization</span></span> | <span data-ttu-id="790d4-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="790d4-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="790d4-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="790d4-135">If-None-Match</span></span> | <span data-ttu-id="790d4-136">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="790d4-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="790d4-137">Optional.</span><span class="sxs-lookup"><span data-stu-id="790d4-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="790d4-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="790d4-138">Response</span></span>

<span data-ttu-id="790d4-139">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="790d4-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="790d4-140">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="790d4-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="790d4-141">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="790d4-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="790d4-142">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="790d4-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="790d4-143">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="790d4-143">Report Refresh Date</span></span>
- <span data-ttu-id="790d4-144">Web</span><span class="sxs-lookup"><span data-stu-id="790d4-144">Web</span></span>
- <span data-ttu-id="790d4-145">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="790d4-145">Windows Phone</span></span>
- <span data-ttu-id="790d4-146">Android-Smartphone</span><span class="sxs-lookup"><span data-stu-id="790d4-146">Android Phone</span></span>
- <span data-ttu-id="790d4-147">iPhone</span><span class="sxs-lookup"><span data-stu-id="790d4-147">iPhone</span></span>
- <span data-ttu-id="790d4-148">iPad</span><span class="sxs-lookup"><span data-stu-id="790d4-148">iPad</span></span>
- <span data-ttu-id="790d4-149">Andere</span><span class="sxs-lookup"><span data-stu-id="790d4-149">Other</span></span>
- <span data-ttu-id="790d4-150">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="790d4-150">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="790d4-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="790d4-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="790d4-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="790d4-152">Request</span></span>

<span data-ttu-id="790d4-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="790d4-153">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="790d4-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="790d4-154">Response</span></span>

<span data-ttu-id="790d4-155">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="790d4-155">The following is an example of the response.</span></span>

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

<span data-ttu-id="790d4-156">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="790d4-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Period
```
