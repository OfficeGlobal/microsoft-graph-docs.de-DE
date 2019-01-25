---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: Rufen Sie Details zur Office 365-Gruppenaktivität nach Gruppe ab.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 3d99cd7c80dd16c6ded518f7e1cbe9fecd0b3230
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515447"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="4aca9-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="4aca9-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4aca9-104">Rufen Sie Details zur Office 365-Gruppenaktivität nach Gruppe ab.</span><span class="sxs-lookup"><span data-stu-id="4aca9-104">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="4aca9-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Office 365-Gruppen](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="4aca9-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="4aca9-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4aca9-106">Permissions</span></span>

<span data-ttu-id="4aca9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4aca9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4aca9-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4aca9-109">Permission type</span></span>                        | <span data-ttu-id="4aca9-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4aca9-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4aca9-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4aca9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4aca9-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4aca9-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4aca9-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4aca9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4aca9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4aca9-114">Not supported.</span></span>                           |
| <span data-ttu-id="4aca9-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4aca9-115">Application</span></span>                            | <span data-ttu-id="4aca9-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4aca9-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4aca9-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4aca9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="4aca9-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="4aca9-118">Function parameters</span></span>

<span data-ttu-id="4aca9-119">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="4aca9-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="4aca9-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="4aca9-120">Parameter</span></span> | <span data-ttu-id="4aca9-121">Typ</span><span class="sxs-lookup"><span data-stu-id="4aca9-121">Type</span></span>   | <span data-ttu-id="4aca9-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4aca9-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4aca9-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="4aca9-123">period</span></span>    | <span data-ttu-id="4aca9-124">string</span><span class="sxs-lookup"><span data-stu-id="4aca9-124">string</span></span> | <span data-ttu-id="4aca9-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="4aca9-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4aca9-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="4aca9-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4aca9-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="4aca9-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="4aca9-128">date</span><span class="sxs-lookup"><span data-stu-id="4aca9-128">date</span></span>      | <span data-ttu-id="4aca9-129">Datum</span><span class="sxs-lookup"><span data-stu-id="4aca9-129">Date</span></span>   | <span data-ttu-id="4aca9-130">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="4aca9-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="4aca9-131">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="4aca9-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="4aca9-132">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="4aca9-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="4aca9-133">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="4aca9-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="4aca9-134">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4aca9-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4aca9-135">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="4aca9-135">The default output type is text/csv.</span></span> <span data-ttu-id="4aca9-136">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="4aca9-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4aca9-137">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4aca9-137">Request headers</span></span>

| <span data-ttu-id="4aca9-138">Name</span><span class="sxs-lookup"><span data-stu-id="4aca9-138">Name</span></span>          | <span data-ttu-id="4aca9-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4aca9-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4aca9-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="4aca9-140">Authorization</span></span> | <span data-ttu-id="4aca9-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4aca9-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4aca9-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="4aca9-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4aca9-144">CSV</span><span class="sxs-lookup"><span data-stu-id="4aca9-144">CSV</span></span>

<span data-ttu-id="4aca9-145">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="4aca9-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4aca9-146">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4aca9-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4aca9-147">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="4aca9-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4aca9-148">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="4aca9-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4aca9-149">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="4aca9-149">Report Refresh Date</span></span>
- <span data-ttu-id="4aca9-150">Gruppenanzeigename</span><span class="sxs-lookup"><span data-stu-id="4aca9-150">Group Display Name</span></span>
- <span data-ttu-id="4aca9-151">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="4aca9-151">Is Deleted</span></span>
- <span data-ttu-id="4aca9-152">Besitzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="4aca9-152">Owner Principal Name</span></span>
- <span data-ttu-id="4aca9-153">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="4aca9-153">Last Activity Date</span></span>
- <span data-ttu-id="4aca9-154">Gruppentyp</span><span class="sxs-lookup"><span data-stu-id="4aca9-154">Group Type</span></span>
- <span data-ttu-id="4aca9-155">Mitgliederzahl</span><span class="sxs-lookup"><span data-stu-id="4aca9-155">Member Count</span></span>
- <span data-ttu-id="4aca9-156">Anzahl der externen Mitglieder</span><span class="sxs-lookup"><span data-stu-id="4aca9-156">External Member Count</span></span>
- <span data-ttu-id="4aca9-157">Anzahl der mit Exchange empfangenen E-Mail-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="4aca9-157">Exchange Received Email Count</span></span>
- <span data-ttu-id="4aca9-158">Anzahl der aktiven SharePoint-Dateien</span><span class="sxs-lookup"><span data-stu-id="4aca9-158">SharePoint Active File Count</span></span>
- <span data-ttu-id="4aca9-159">Anzahl der veröffentlichten Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="4aca9-159">Yammer Posted Message Count</span></span>
- <span data-ttu-id="4aca9-160">Anzahl der gelesenen Yammer-Nachricht</span><span class="sxs-lookup"><span data-stu-id="4aca9-160">Yammer Read Message Count</span></span>
- <span data-ttu-id="4aca9-161">Anzahl der gelikten Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="4aca9-161">Yammer Liked Message Count</span></span>
- <span data-ttu-id="4aca9-162">Gesamtanzahl der Exchange-Postfachelemente</span><span class="sxs-lookup"><span data-stu-id="4aca9-162">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="4aca9-163">Verwendeter Exchange-Postfachspeicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="4aca9-163">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="4aca9-164">Gesamtzahl der SharePoint-Dateien</span><span class="sxs-lookup"><span data-stu-id="4aca9-164">SharePoint Total File Count</span></span>
- <span data-ttu-id="4aca9-165">Verwendeter SharePoint-Websitesspeicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="4aca9-165">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="4aca9-166">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="4aca9-166">Report Period</span></span>

<span data-ttu-id="4aca9-167">Die folgenden Spalten werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt:</span><span class="sxs-lookup"><span data-stu-id="4aca9-167">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="4aca9-168">Anzahl der veröffentlichten Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="4aca9-168">Yammer Posted Message Count</span></span>
- <span data-ttu-id="4aca9-169">Anzahl der gelesenen Yammer-Nachricht</span><span class="sxs-lookup"><span data-stu-id="4aca9-169">Yammer Read Message Count</span></span>
- <span data-ttu-id="4aca9-170">Anzahl der gelikten Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="4aca9-170">Yammer Liked Message Count</span></span>

### <a name="json"></a><span data-ttu-id="4aca9-171">JSON</span><span class="sxs-lookup"><span data-stu-id="4aca9-171">JSON</span></span>

<span data-ttu-id="4aca9-172">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4aca9-172">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="4aca9-173">Die folgenden Eigenschaften im **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** -Objekt werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt:</span><span class="sxs-lookup"><span data-stu-id="4aca9-173">The following properties in **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="4aca9-174">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="4aca9-174">yammerPostedMessageCount</span></span>
- <span data-ttu-id="4aca9-175">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="4aca9-175">yammerReadMessageCount</span></span>
- <span data-ttu-id="4aca9-176">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="4aca9-176">yammerLikedMessageCount</span></span>

<span data-ttu-id="4aca9-177">Die Seite Standardgröße für diese Anforderung ist 200 Elemente.</span><span class="sxs-lookup"><span data-stu-id="4aca9-177">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="4aca9-178">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4aca9-178">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4aca9-179">CSV</span><span class="sxs-lookup"><span data-stu-id="4aca9-179">CSV</span></span>

<span data-ttu-id="4aca9-180">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="4aca9-180">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4aca9-181">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4aca9-181">Request</span></span>

<span data-ttu-id="4aca9-182">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4aca9-182">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="4aca9-183">Antwort</span><span class="sxs-lookup"><span data-stu-id="4aca9-183">Response</span></span>

<span data-ttu-id="4aca9-184">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4aca9-184">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4aca9-185">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="4aca9-185">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,External Member Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Report Period
```

### <a name="json"></a><span data-ttu-id="4aca9-186">JSON</span><span class="sxs-lookup"><span data-stu-id="4aca9-186">JSON</span></span>

<span data-ttu-id="4aca9-187">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4aca9-187">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4aca9-188">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4aca9-188">Request</span></span>

<span data-ttu-id="4aca9-189">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4aca9-189">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="4aca9-190">Antwort</span><span class="sxs-lookup"><span data-stu-id="4aca9-190">Response</span></span>

<span data-ttu-id="4aca9-191">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4aca9-191">The following is an example of the response.</span></span>

> <span data-ttu-id="4aca9-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="4aca9-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 674

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "groupDisplayName": "groupDisplayName-value", 
      "isDeleted": false, 
      "ownerPrincipalName": "ownerDisplayName-value", 
      "lastActivityDate": "2017-08-31", 
      "groupType": "Private", 
      "memberCount": 5, 
      "externalMemberCount": 0, 
      "exchangeReceivedEmailCount": 341, 
      "sharePointActiveFileCount": 0, 
      "yammerPostedMessageCount": 0, 
      "yammerReadMessageCount": 0, 
      "yammerLikedMessageCount": 0, 
      "exchangeMailboxTotalItemCount": 343, 
      "exchangeMailboxStorageUsedInBytes": 3724609, 
      "sharePointTotalFileCount": 0, 
      "sharePointSiteStorageUsedInBytes": 0, 
      "reportPeriod": "30"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitydetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
