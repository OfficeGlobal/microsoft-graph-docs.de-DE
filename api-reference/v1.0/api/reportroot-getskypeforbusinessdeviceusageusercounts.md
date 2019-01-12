---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserCounts'
description: Erfahren Sie mehr über Auslastungstrends, indem Sie sich ansehen, wie viele Benutzer in Ihrer Organisation sich über die Skype for Business-App verbunden haben. Außerdem erhalten Sie eine Auflistung des Gerätetyps (Windows, Windows Phone, Android-Smartphone, iPhone oder iPad) auf dem die Skype for Business-Client-App installiert und in Ihrer Organisation verwendet wird.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 4ed52939486348046b2b3c2d1000aa1024e041a6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968603"
---
# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="bf010-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="bf010-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

<span data-ttu-id="bf010-105">Erfahren Sie mehr über Auslastungstrends, indem Sie sich ansehen, wie viele Benutzer in Ihrer Organisation sich über die Skype for Business-App verbunden haben.</span><span class="sxs-lookup"><span data-stu-id="bf010-105">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="bf010-106">Außerdem erhalten Sie eine Auflistung des Gerätetyps (Windows, Windows Phone, Android-Smartphone, iPhone oder iPad) auf dem die Skype for Business-Client-App installiert und in Ihrer Organisation verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="bf010-106">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="bf010-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Verwendete Skype for Business-Clients](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="bf010-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="bf010-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bf010-108">Permissions</span></span>

<span data-ttu-id="bf010-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf010-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bf010-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bf010-111">Permission type</span></span>                        | <span data-ttu-id="bf010-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bf010-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bf010-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bf010-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="bf010-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf010-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bf010-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bf010-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf010-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bf010-116">Not supported.</span></span>                           |
| <span data-ttu-id="bf010-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bf010-117">Application</span></span>                            | <span data-ttu-id="bf010-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf010-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bf010-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bf010-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="bf010-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="bf010-120">Function parameters</span></span>

<span data-ttu-id="bf010-121">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="bf010-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="bf010-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="bf010-122">Parameter</span></span> | <span data-ttu-id="bf010-123">Typ</span><span class="sxs-lookup"><span data-stu-id="bf010-123">Type</span></span>   | <span data-ttu-id="bf010-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bf010-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bf010-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="bf010-125">period</span></span>    | <span data-ttu-id="bf010-126">string</span><span class="sxs-lookup"><span data-stu-id="bf010-126">string</span></span> | <span data-ttu-id="bf010-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="bf010-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bf010-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="bf010-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bf010-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="bf010-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="bf010-130">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="bf010-130">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="bf010-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bf010-131">Request headers</span></span>

| <span data-ttu-id="bf010-132">Name</span><span class="sxs-lookup"><span data-stu-id="bf010-132">Name</span></span>          | <span data-ttu-id="bf010-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bf010-133">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="bf010-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf010-134">Authorization</span></span> | <span data-ttu-id="bf010-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bf010-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="bf010-137">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="bf010-137">If-None-Match</span></span> | <span data-ttu-id="bf010-138">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bf010-138">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="bf010-139">Optional.</span><span class="sxs-lookup"><span data-stu-id="bf010-139">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="bf010-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="bf010-140">Response</span></span>

<span data-ttu-id="bf010-141">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="bf010-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bf010-142">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bf010-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bf010-143">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="bf010-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bf010-144">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="bf010-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bf010-145">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="bf010-145">Report Refresh Date</span></span>
- <span data-ttu-id="bf010-146">Windows</span><span class="sxs-lookup"><span data-stu-id="bf010-146">Windows</span></span>
- <span data-ttu-id="bf010-147">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="bf010-147">Windows Phone</span></span>
- <span data-ttu-id="bf010-148">Android-Smartphone</span><span class="sxs-lookup"><span data-stu-id="bf010-148">Android Phone</span></span>
- <span data-ttu-id="bf010-149">iPhone</span><span class="sxs-lookup"><span data-stu-id="bf010-149">iPhone</span></span>
- <span data-ttu-id="bf010-150">iPad</span><span class="sxs-lookup"><span data-stu-id="bf010-150">iPad</span></span>
- <span data-ttu-id="bf010-151">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="bf010-151">Report Date</span></span>
- <span data-ttu-id="bf010-152">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="bf010-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="bf010-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bf010-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bf010-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bf010-154">Request</span></span>

<span data-ttu-id="bf010-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bf010-155">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="bf010-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="bf010-156">Response</span></span>

<span data-ttu-id="bf010-157">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bf010-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="bf010-158">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="bf010-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Date,Report Period
```
