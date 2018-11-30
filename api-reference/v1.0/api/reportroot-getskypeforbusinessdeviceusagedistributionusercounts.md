---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: Rufen Sie die Anzahl der Benutzer ab, die eigene Geräte in Ihrer Organisation verwenden. Der Bericht enthält die Anzahl der Benutzer pro Gerät, einschließlich Windows, Windows Phone, Android-Smartphone, iPhone und iPad.
ms.openlocfilehash: a911cc4cac8d7c6f2465f0d7f3220770ca21f351
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019664"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="eea64-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="eea64-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="eea64-105">Rufen Sie die Anzahl der Benutzer ab, die eigene Geräte in Ihrer Organisation verwenden.</span><span class="sxs-lookup"><span data-stu-id="eea64-105">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="eea64-106">Der Bericht enthält die Anzahl der Benutzer pro Gerät, einschließlich Windows, Windows Phone, Android-Smartphone, iPhone und iPad.</span><span class="sxs-lookup"><span data-stu-id="eea64-106">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="eea64-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Verwendete Skype for Business-Clients](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="eea64-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="eea64-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="eea64-108">Permissions</span></span>

<span data-ttu-id="eea64-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eea64-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eea64-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eea64-111">Permission type</span></span>                        | <span data-ttu-id="eea64-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eea64-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="eea64-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eea64-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="eea64-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="eea64-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="eea64-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eea64-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eea64-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eea64-116">Not supported.</span></span>                           |
| <span data-ttu-id="eea64-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eea64-117">Application</span></span>                            | <span data-ttu-id="eea64-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="eea64-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="eea64-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eea64-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="eea64-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="eea64-120">Function parameters</span></span>

<span data-ttu-id="eea64-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="eea64-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="eea64-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="eea64-122">Parameter</span></span> | <span data-ttu-id="eea64-123">Typ</span><span class="sxs-lookup"><span data-stu-id="eea64-123">Type</span></span>   | <span data-ttu-id="eea64-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eea64-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="eea64-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="eea64-125">period</span></span>    | <span data-ttu-id="eea64-126">string</span><span class="sxs-lookup"><span data-stu-id="eea64-126">string</span></span> | <span data-ttu-id="eea64-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="eea64-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="eea64-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="eea64-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="eea64-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="eea64-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="eea64-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="eea64-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="eea64-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eea64-131">Request headers</span></span>

| <span data-ttu-id="eea64-132">Name</span><span class="sxs-lookup"><span data-stu-id="eea64-132">Name</span></span>          | <span data-ttu-id="eea64-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eea64-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="eea64-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="eea64-134">Authorization</span></span> | <span data-ttu-id="eea64-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="eea64-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="eea64-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="eea64-137">If-None-Match</span></span> | <span data-ttu-id="eea64-138">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eea64-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="eea64-139">Optional.</span><span class="sxs-lookup"><span data-stu-id="eea64-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="eea64-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="eea64-140">Response</span></span>

<span data-ttu-id="eea64-141">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="eea64-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="eea64-142">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="eea64-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="eea64-143">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="eea64-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="eea64-144">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="eea64-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="eea64-145">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="eea64-145">Report Refresh Date</span></span>
- <span data-ttu-id="eea64-146">Windows</span><span class="sxs-lookup"><span data-stu-id="eea64-146">Windows</span></span>
- <span data-ttu-id="eea64-147">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="eea64-147">Windows Phone</span></span>
- <span data-ttu-id="eea64-148">Android-Smartphone</span><span class="sxs-lookup"><span data-stu-id="eea64-148">Android Phone</span></span>
- <span data-ttu-id="eea64-149">iPhone</span><span class="sxs-lookup"><span data-stu-id="eea64-149">iPhone</span></span>
- <span data-ttu-id="eea64-150">iPad</span><span class="sxs-lookup"><span data-stu-id="eea64-150">iPad</span></span>
- <span data-ttu-id="eea64-151">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="eea64-151">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="eea64-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eea64-152">Example</span></span>

#### <a name="request"></a><span data-ttu-id="eea64-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eea64-153">Request</span></span>

<span data-ttu-id="eea64-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eea64-154">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="eea64-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="eea64-155">Response</span></span>

<span data-ttu-id="eea64-156">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="eea64-156">The following is an example of the response.</span></span>

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

<span data-ttu-id="eea64-157">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="eea64-157">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Period
```