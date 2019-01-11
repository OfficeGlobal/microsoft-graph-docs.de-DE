---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: Rufen Sie Details zur Office 365-Gruppenaktivität nach Gruppe ab.
localization_priority: Normal
ms.openlocfilehash: 02def0c4c2c54a6379ca5770f36d1f7fe5cfa925
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871680"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="44d9d-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="44d9d-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

> <span data-ttu-id="44d9d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="44d9d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44d9d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="44d9d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="44d9d-106">Rufen Sie Details zur Office 365-Gruppenaktivität nach Gruppe ab.</span><span class="sxs-lookup"><span data-stu-id="44d9d-106">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="44d9d-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Office 365-Gruppen](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="44d9d-107">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="44d9d-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="44d9d-108">Permissions</span></span>

<span data-ttu-id="44d9d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44d9d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="44d9d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="44d9d-111">Permission type</span></span>                        | <span data-ttu-id="44d9d-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="44d9d-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="44d9d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="44d9d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="44d9d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="44d9d-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="44d9d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="44d9d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44d9d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="44d9d-116">Not supported.</span></span>                           |
| <span data-ttu-id="44d9d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="44d9d-117">Application</span></span>                            | <span data-ttu-id="44d9d-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="44d9d-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="44d9d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="44d9d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="44d9d-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="44d9d-120">Function parameters</span></span>

<span data-ttu-id="44d9d-121">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="44d9d-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="44d9d-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="44d9d-122">Parameter</span></span> | <span data-ttu-id="44d9d-123">Typ</span><span class="sxs-lookup"><span data-stu-id="44d9d-123">Type</span></span>   | <span data-ttu-id="44d9d-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="44d9d-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="44d9d-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="44d9d-125">period</span></span>    | <span data-ttu-id="44d9d-126">string</span><span class="sxs-lookup"><span data-stu-id="44d9d-126">string</span></span> | <span data-ttu-id="44d9d-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="44d9d-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="44d9d-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="44d9d-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="44d9d-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="44d9d-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="44d9d-130">date</span><span class="sxs-lookup"><span data-stu-id="44d9d-130">date</span></span>      | <span data-ttu-id="44d9d-131">Datum</span><span class="sxs-lookup"><span data-stu-id="44d9d-131">Date</span></span>   | <span data-ttu-id="44d9d-132">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="44d9d-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="44d9d-133">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="44d9d-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="44d9d-134">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="44d9d-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="44d9d-135">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="44d9d-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="44d9d-136">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="44d9d-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="44d9d-137">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="44d9d-137">The default output type is text/csv.</span></span> <span data-ttu-id="44d9d-138">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="44d9d-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="44d9d-139">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="44d9d-139">Request headers</span></span>

| <span data-ttu-id="44d9d-140">Name</span><span class="sxs-lookup"><span data-stu-id="44d9d-140">Name</span></span>          | <span data-ttu-id="44d9d-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="44d9d-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="44d9d-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="44d9d-142">Authorization</span></span> | <span data-ttu-id="44d9d-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="44d9d-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="44d9d-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="44d9d-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="44d9d-146">CSV</span><span class="sxs-lookup"><span data-stu-id="44d9d-146">CSV</span></span>

<span data-ttu-id="44d9d-147">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="44d9d-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="44d9d-148">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="44d9d-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="44d9d-149">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="44d9d-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="44d9d-150">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="44d9d-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="44d9d-151">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="44d9d-151">Report Refresh Date</span></span>
- <span data-ttu-id="44d9d-152">Gruppenanzeigename</span><span class="sxs-lookup"><span data-stu-id="44d9d-152">Group Display Name</span></span>
- <span data-ttu-id="44d9d-153">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="44d9d-153">Is Deleted</span></span>
- <span data-ttu-id="44d9d-154">Besitzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="44d9d-154">Owner Principal Name</span></span>
- <span data-ttu-id="44d9d-155">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="44d9d-155">Last Activity Date</span></span>
- <span data-ttu-id="44d9d-156">Gruppentyp</span><span class="sxs-lookup"><span data-stu-id="44d9d-156">Group Type</span></span>
- <span data-ttu-id="44d9d-157">Mitgliederzahl</span><span class="sxs-lookup"><span data-stu-id="44d9d-157">Member Count</span></span>
- <span data-ttu-id="44d9d-158">Anzahl der externen Mitglieder</span><span class="sxs-lookup"><span data-stu-id="44d9d-158">External Member Count</span></span>
- <span data-ttu-id="44d9d-159">Anzahl der mit Exchange empfangenen E-Mail-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="44d9d-159">Exchange Received Email Count</span></span>
- <span data-ttu-id="44d9d-160">Anzahl der aktiven SharePoint-Dateien</span><span class="sxs-lookup"><span data-stu-id="44d9d-160">SharePoint Active File Count</span></span>
- <span data-ttu-id="44d9d-161">Anzahl der veröffentlichten Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="44d9d-161">Yammer Posted Message Count</span></span>
- <span data-ttu-id="44d9d-162">Anzahl der gelesenen Yammer-Nachricht</span><span class="sxs-lookup"><span data-stu-id="44d9d-162">Yammer Read Message Count</span></span>
- <span data-ttu-id="44d9d-163">Anzahl der gelikten Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="44d9d-163">Yammer Liked Message Count</span></span>
- <span data-ttu-id="44d9d-164">Gesamtanzahl der Exchange-Postfachelemente</span><span class="sxs-lookup"><span data-stu-id="44d9d-164">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="44d9d-165">Verwendeter Exchange-Postfachspeicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="44d9d-165">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="44d9d-166">Gesamtzahl der SharePoint-Dateien</span><span class="sxs-lookup"><span data-stu-id="44d9d-166">SharePoint Total File Count</span></span>
- <span data-ttu-id="44d9d-167">Verwendeter SharePoint-Websitesspeicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="44d9d-167">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="44d9d-168">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="44d9d-168">Report Period</span></span>

<span data-ttu-id="44d9d-169">Die folgenden Spalten werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt:</span><span class="sxs-lookup"><span data-stu-id="44d9d-169">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="44d9d-170">Anzahl der veröffentlichten Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="44d9d-170">Yammer Posted Message Count</span></span>
- <span data-ttu-id="44d9d-171">Anzahl der gelesenen Yammer-Nachricht</span><span class="sxs-lookup"><span data-stu-id="44d9d-171">Yammer Read Message Count</span></span>
- <span data-ttu-id="44d9d-172">Anzahl der gelikten Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="44d9d-172">Yammer Liked Message Count</span></span>

### <a name="json"></a><span data-ttu-id="44d9d-173">JSON</span><span class="sxs-lookup"><span data-stu-id="44d9d-173">JSON</span></span>

<span data-ttu-id="44d9d-174">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="44d9d-174">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="44d9d-175">Die folgenden Eigenschaften im **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** -Objekt werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt:</span><span class="sxs-lookup"><span data-stu-id="44d9d-175">The following properties in **[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="44d9d-176">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="44d9d-176">yammerPostedMessageCount</span></span>
- <span data-ttu-id="44d9d-177">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="44d9d-177">yammerReadMessageCount</span></span>
- <span data-ttu-id="44d9d-178">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="44d9d-178">yammerLikedMessageCount</span></span>

<span data-ttu-id="44d9d-179">Die Seite Standardgröße für diese Anforderung ist 200 Elemente.</span><span class="sxs-lookup"><span data-stu-id="44d9d-179">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="44d9d-180">Beispiel</span><span class="sxs-lookup"><span data-stu-id="44d9d-180">Example</span></span>

### <a name="csv"></a><span data-ttu-id="44d9d-181">CSV</span><span class="sxs-lookup"><span data-stu-id="44d9d-181">CSV</span></span>

<span data-ttu-id="44d9d-182">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="44d9d-182">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="44d9d-183">Anforderung</span><span class="sxs-lookup"><span data-stu-id="44d9d-183">Request</span></span>

<span data-ttu-id="44d9d-184">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="44d9d-184">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="44d9d-185">Antwort</span><span class="sxs-lookup"><span data-stu-id="44d9d-185">Response</span></span>

<span data-ttu-id="44d9d-186">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="44d9d-186">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="44d9d-187">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="44d9d-187">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="44d9d-188">JSON</span><span class="sxs-lookup"><span data-stu-id="44d9d-188">JSON</span></span>

<span data-ttu-id="44d9d-189">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="44d9d-189">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="44d9d-190">Anforderung</span><span class="sxs-lookup"><span data-stu-id="44d9d-190">Request</span></span>

<span data-ttu-id="44d9d-191">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="44d9d-191">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="44d9d-192">Antwort</span><span class="sxs-lookup"><span data-stu-id="44d9d-192">Response</span></span>

<span data-ttu-id="44d9d-193">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="44d9d-193">The following is an example of the response.</span></span>

> <span data-ttu-id="44d9d-p108">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="44d9d-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
