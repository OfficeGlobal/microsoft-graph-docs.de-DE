---
title: 'reportRoot: getOneDriveUsageStorage'
description: Verschaffen Sie sich einen Überblick über die Menge an Speicherplatz, die Sie in OneDrive for Business verwenden.
ms.openlocfilehash: 00205de201ef168c0c50cff29f903325411b371c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019620"
---
# <a name="reportroot-getonedriveusagestorage"></a><span data-ttu-id="602a9-103">reportRoot: getOneDriveUsageStorage</span><span class="sxs-lookup"><span data-stu-id="602a9-103">reportRoot: getOneDriveUsageStorage</span></span>

<span data-ttu-id="602a9-104">Verschaffen Sie sich einen Überblick über die Menge an Speicherplatz, die Sie in OneDrive for Business verwenden.</span><span class="sxs-lookup"><span data-stu-id="602a9-104">Get the trend on the amount of storage you are using in OneDrive for Business.</span></span>

> <span data-ttu-id="602a9-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – OneDrive for Business-Nutzung](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="602a9-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="602a9-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="602a9-106">Permissions</span></span>

<span data-ttu-id="602a9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="602a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="602a9-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="602a9-109">Permission type</span></span>                        | <span data-ttu-id="602a9-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="602a9-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="602a9-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="602a9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="602a9-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="602a9-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="602a9-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="602a9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="602a9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="602a9-114">Not supported.</span></span>                           |
| <span data-ttu-id="602a9-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="602a9-115">Application</span></span>                            | <span data-ttu-id="602a9-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="602a9-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="602a9-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="602a9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="602a9-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="602a9-118">Function parameters</span></span>

<span data-ttu-id="602a9-119">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="602a9-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="602a9-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="602a9-120">Parameter</span></span> | <span data-ttu-id="602a9-121">Typ</span><span class="sxs-lookup"><span data-stu-id="602a9-121">Type</span></span>   | <span data-ttu-id="602a9-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="602a9-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="602a9-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="602a9-123">period</span></span>    | <span data-ttu-id="602a9-124">string</span><span class="sxs-lookup"><span data-stu-id="602a9-124">string</span></span> | <span data-ttu-id="602a9-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="602a9-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="602a9-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="602a9-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="602a9-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="602a9-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="602a9-128">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="602a9-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="602a9-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="602a9-129">Request headers</span></span>

| <span data-ttu-id="602a9-130">Name</span><span class="sxs-lookup"><span data-stu-id="602a9-130">Name</span></span>          | <span data-ttu-id="602a9-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="602a9-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="602a9-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="602a9-132">Authorization</span></span> | <span data-ttu-id="602a9-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="602a9-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="602a9-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="602a9-135">If-None-Match</span></span> | <span data-ttu-id="602a9-136">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="602a9-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="602a9-137">Optional.</span><span class="sxs-lookup"><span data-stu-id="602a9-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="602a9-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="602a9-138">Response</span></span>

<span data-ttu-id="602a9-139">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="602a9-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="602a9-140">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="602a9-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="602a9-141">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="602a9-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="602a9-142">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="602a9-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="602a9-143">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="602a9-143">Report Refresh Date</span></span>
- <span data-ttu-id="602a9-144">Websitetyp</span><span class="sxs-lookup"><span data-stu-id="602a9-144">Site Type</span></span>
- <span data-ttu-id="602a9-145">Verwendeter Speicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="602a9-145">Storage Used (Byte)</span></span>
- <span data-ttu-id="602a9-146">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="602a9-146">Report Date</span></span>
- <span data-ttu-id="602a9-147">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="602a9-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="602a9-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="602a9-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="602a9-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="602a9-149">Request</span></span>

<span data-ttu-id="602a9-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="602a9-150">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusagestorage"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageStorage(period='D7')
```

#### <a name="response"></a><span data-ttu-id="602a9-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="602a9-151">Response</span></span>

<span data-ttu-id="602a9-152">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="602a9-152">The following is an example of the response.</span></span>

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

<span data-ttu-id="602a9-153">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="602a9-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Storage Used (Byte),Report Date,Report Period
```