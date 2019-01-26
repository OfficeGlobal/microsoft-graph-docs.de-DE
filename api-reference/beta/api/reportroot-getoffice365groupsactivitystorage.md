---
title: 'reportRoot: getOffice365GroupsActivityStorage'
description: Rufen Sie den insgesamt für alle Gruppenpostfächer und Gruppenwebsites genutzten Speicherplatz ab.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4248251bac7146334dc97e8101f29d53faacf2d5
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571674"
---
# <a name="reportroot-getoffice365groupsactivitystorage"></a><span data-ttu-id="34e3c-103">reportRoot: getOffice365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="34e3c-103">reportRoot: getOffice365GroupsActivityStorage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34e3c-104">Rufen Sie den insgesamt für alle Gruppenpostfächer und Gruppenwebsites genutzten Speicherplatz ab.</span><span class="sxs-lookup"><span data-stu-id="34e3c-104">Get the total storage used across all group mailboxes and group sites.</span></span>

> <span data-ttu-id="34e3c-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Office 365-Gruppen](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="34e3c-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="34e3c-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="34e3c-106">Permissions</span></span>

<span data-ttu-id="34e3c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34e3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="34e3c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="34e3c-109">Permission type</span></span>                        | <span data-ttu-id="34e3c-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="34e3c-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="34e3c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="34e3c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="34e3c-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="34e3c-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="34e3c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="34e3c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34e3c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="34e3c-114">Not supported.</span></span>                           |
| <span data-ttu-id="34e3c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="34e3c-115">Application</span></span>                            | <span data-ttu-id="34e3c-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="34e3c-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="34e3c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="34e3c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="34e3c-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="34e3c-118">Function parameters</span></span>

<span data-ttu-id="34e3c-119">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="34e3c-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="34e3c-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="34e3c-120">Parameter</span></span> | <span data-ttu-id="34e3c-121">Typ</span><span class="sxs-lookup"><span data-stu-id="34e3c-121">Type</span></span>   | <span data-ttu-id="34e3c-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34e3c-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="34e3c-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="34e3c-123">period</span></span>    | <span data-ttu-id="34e3c-124">string</span><span class="sxs-lookup"><span data-stu-id="34e3c-124">string</span></span> | <span data-ttu-id="34e3c-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="34e3c-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="34e3c-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="34e3c-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="34e3c-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="34e3c-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="34e3c-128">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="34e3c-128">Required.</span></span> |

<span data-ttu-id="34e3c-129">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="34e3c-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="34e3c-130">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="34e3c-130">The default output type is text/csv.</span></span> <span data-ttu-id="34e3c-131">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="34e3c-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="34e3c-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="34e3c-132">Request headers</span></span>

| <span data-ttu-id="34e3c-133">Name</span><span class="sxs-lookup"><span data-stu-id="34e3c-133">Name</span></span>          | <span data-ttu-id="34e3c-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34e3c-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="34e3c-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="34e3c-135">Authorization</span></span> | <span data-ttu-id="34e3c-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="34e3c-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="34e3c-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="34e3c-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="34e3c-139">CSV</span><span class="sxs-lookup"><span data-stu-id="34e3c-139">CSV</span></span>

<span data-ttu-id="34e3c-140">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="34e3c-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="34e3c-141">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="34e3c-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="34e3c-142">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="34e3c-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="34e3c-143">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="34e3c-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="34e3c-144">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="34e3c-144">Report Refresh Date</span></span>
- <span data-ttu-id="34e3c-145">Verwendeter Postfachspeicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="34e3c-145">Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="34e3c-146">Verwendeter Websitesspeicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="34e3c-146">Site Storage Used (Byte)</span></span>
- <span data-ttu-id="34e3c-147">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="34e3c-147">Report Date</span></span>
- <span data-ttu-id="34e3c-148">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="34e3c-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="34e3c-149">JSON</span><span class="sxs-lookup"><span data-stu-id="34e3c-149">JSON</span></span>

<span data-ttu-id="34e3c-150">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines **[office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="34e3c-150">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34e3c-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="34e3c-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="34e3c-152">CSV</span><span class="sxs-lookup"><span data-stu-id="34e3c-152">CSV</span></span>

<span data-ttu-id="34e3c-153">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="34e3c-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="34e3c-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="34e3c-154">Request</span></span>

<span data-ttu-id="34e3c-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="34e3c-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitystorage_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityStorage(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="34e3c-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="34e3c-156">Response</span></span>

<span data-ttu-id="34e3c-157">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="34e3c-157">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="34e3c-158">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="34e3c-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mailbox Storage Used (Byte),Site Storage Used (Byte),Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="34e3c-159">JSON</span><span class="sxs-lookup"><span data-stu-id="34e3c-159">JSON</span></span>

<span data-ttu-id="34e3c-160">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="34e3c-160">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="34e3c-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="34e3c-161">Request</span></span>

<span data-ttu-id="34e3c-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="34e3c-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitystorage_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityStorage(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="34e3c-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="34e3c-163">Response</span></span>

<span data-ttu-id="34e3c-164">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="34e3c-164">The following is an example of the response.</span></span>

> <span data-ttu-id="34e3c-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="34e3c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityStorage"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityStorage)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "mailboxStorageUsedInBytes": 523143237898, 
      "siteStorageUsedInBytes": 31124384, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitystorage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
