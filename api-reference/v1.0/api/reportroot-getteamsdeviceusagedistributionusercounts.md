---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: Abrufen der Anzahl der täglichen eindeutigen Benutzer des Microsoft Teams nach Gerätetyp im ausgewählten Zeitraum.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5f50634d8107d95af6708361a88284122325b5ef
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574831"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="04596-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="04596-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="04596-104">Abrufen der Anzahl der täglichen eindeutigen Benutzer des Microsoft Teams nach Gerätetyp im ausgewählten Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="04596-104">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="04596-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="04596-105">Permissions</span></span>

<span data-ttu-id="04596-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04596-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="04596-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="04596-108">Permission type</span></span>                        | <span data-ttu-id="04596-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="04596-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="04596-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="04596-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="04596-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="04596-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="04596-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="04596-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04596-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="04596-113">Not supported.</span></span>                           |
| <span data-ttu-id="04596-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="04596-114">Application</span></span>                            | <span data-ttu-id="04596-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="04596-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="04596-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="04596-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="04596-117">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="04596-117">Function parameters</span></span>

<span data-ttu-id="04596-118">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="04596-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="04596-119">Parameter</span><span class="sxs-lookup"><span data-stu-id="04596-119">Parameter</span></span> | <span data-ttu-id="04596-120">Typ</span><span class="sxs-lookup"><span data-stu-id="04596-120">Type</span></span>   | <span data-ttu-id="04596-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04596-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="04596-122">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="04596-122">period</span></span>    | <span data-ttu-id="04596-123">string</span><span class="sxs-lookup"><span data-stu-id="04596-123">string</span></span> | <span data-ttu-id="04596-124">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="04596-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="04596-125">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="04596-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="04596-126">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="04596-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="04596-127">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="04596-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="04596-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="04596-128">Request headers</span></span>

| <span data-ttu-id="04596-129">Name</span><span class="sxs-lookup"><span data-stu-id="04596-129">Name</span></span>          | <span data-ttu-id="04596-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04596-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="04596-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="04596-131">Authorization</span></span> | <span data-ttu-id="04596-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="04596-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="04596-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="04596-134">Response</span></span>

<span data-ttu-id="04596-135">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="04596-135">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="04596-136">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="04596-136">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="04596-137">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="04596-137">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="04596-138">Die CSV-Datei verfügt über die folgenden Spaltenheader:</span><span class="sxs-lookup"><span data-stu-id="04596-138">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="04596-139">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="04596-139">Report Refresh Date</span></span>
- <span data-ttu-id="04596-140">Web</span><span class="sxs-lookup"><span data-stu-id="04596-140">Web</span></span>
- <span data-ttu-id="04596-141">Windows Phone</span><span class="sxs-lookup"><span data-stu-id="04596-141">Windows Phone</span></span>
- <span data-ttu-id="04596-142">Android-Smartphone</span><span class="sxs-lookup"><span data-stu-id="04596-142">Android Phone</span></span>
- <span data-ttu-id="04596-143">iOS</span><span class="sxs-lookup"><span data-stu-id="04596-143">iOS</span></span>
- <span data-ttu-id="04596-144">Mac</span><span class="sxs-lookup"><span data-stu-id="04596-144">Mac</span></span>
- <span data-ttu-id="04596-145">Windows</span><span class="sxs-lookup"><span data-stu-id="04596-145">Windows</span></span>
- <span data-ttu-id="04596-146">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="04596-146">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="04596-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="04596-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="04596-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04596-148">Request</span></span>

<span data-ttu-id="04596-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="04596-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="04596-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="04596-150">Response</span></span>

<span data-ttu-id="04596-151">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="04596-151">The following is an example of the response.</span></span>

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

<span data-ttu-id="04596-152">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="04596-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
```
