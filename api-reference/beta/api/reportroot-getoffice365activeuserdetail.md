---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: Rufen Sie Details zu aktiven Office 365-Benutzern ab.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: ba73993ffdf205e197058afa2d9aea2648e7c877
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518149"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="3f412-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="3f412-103">reportRoot: getOffice365ActiveUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f412-104">Rufen Sie Details zu aktiven Office 365-Benutzern ab.</span><span class="sxs-lookup"><span data-stu-id="3f412-104">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="3f412-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Aktive Benutzer](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="3f412-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="3f412-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3f412-106">Permissions</span></span>

<span data-ttu-id="3f412-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f412-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3f412-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3f412-109">Permission type</span></span>                        | <span data-ttu-id="3f412-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3f412-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3f412-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3f412-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3f412-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f412-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3f412-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3f412-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f412-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3f412-114">Not supported.</span></span>                           |
| <span data-ttu-id="3f412-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3f412-115">Application</span></span>                            | <span data-ttu-id="3f412-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f412-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3f412-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3f412-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="3f412-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="3f412-118">Function parameters</span></span>

<span data-ttu-id="3f412-119">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="3f412-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="3f412-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="3f412-120">Parameter</span></span> | <span data-ttu-id="3f412-121">Typ</span><span class="sxs-lookup"><span data-stu-id="3f412-121">Type</span></span>   | <span data-ttu-id="3f412-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3f412-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3f412-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="3f412-123">period</span></span>    | <span data-ttu-id="3f412-124">string</span><span class="sxs-lookup"><span data-stu-id="3f412-124">string</span></span> | <span data-ttu-id="3f412-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="3f412-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3f412-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="3f412-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3f412-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="3f412-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="3f412-128">date</span><span class="sxs-lookup"><span data-stu-id="3f412-128">date</span></span>      | <span data-ttu-id="3f412-129">Datum</span><span class="sxs-lookup"><span data-stu-id="3f412-129">Date</span></span>   | <span data-ttu-id="3f412-130">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="3f412-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="3f412-131">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="3f412-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="3f412-132">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="3f412-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="3f412-133">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="3f412-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="3f412-134">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3f412-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3f412-135">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="3f412-135">The default output type is text/csv.</span></span> <span data-ttu-id="3f412-136">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="3f412-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3f412-137">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3f412-137">Request headers</span></span>

| <span data-ttu-id="3f412-138">Name</span><span class="sxs-lookup"><span data-stu-id="3f412-138">Name</span></span>          | <span data-ttu-id="3f412-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3f412-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3f412-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f412-140">Authorization</span></span> | <span data-ttu-id="3f412-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3f412-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3f412-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="3f412-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="3f412-144">CSV</span><span class="sxs-lookup"><span data-stu-id="3f412-144">CSV</span></span>

<span data-ttu-id="3f412-145">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="3f412-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3f412-146">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3f412-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3f412-147">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="3f412-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3f412-148">Die CSV-Datei verfügt über die folgenden Spaltenheader:</span><span class="sxs-lookup"><span data-stu-id="3f412-148">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="3f412-149">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="3f412-149">Report Refresh Date</span></span>
- <span data-ttu-id="3f412-150">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="3f412-150">User Principal Name</span></span>
- <span data-ttu-id="3f412-151">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="3f412-151">Display Name</span></span>
- <span data-ttu-id="3f412-152">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="3f412-152">Is Deleted</span></span>
- <span data-ttu-id="3f412-153">Gelöscht am</span><span class="sxs-lookup"><span data-stu-id="3f412-153">Deleted Date</span></span>
- <span data-ttu-id="3f412-154">Besitzt Exchange-Lizenz</span><span class="sxs-lookup"><span data-stu-id="3f412-154">Has Exchange License</span></span>
- <span data-ttu-id="3f412-155">Besitzt OneDrive-Lizenz</span><span class="sxs-lookup"><span data-stu-id="3f412-155">Has OneDrive License</span></span>
- <span data-ttu-id="3f412-156">Besitzt SharePoint-Lizenz</span><span class="sxs-lookup"><span data-stu-id="3f412-156">Has SharePoint License</span></span>
- <span data-ttu-id="3f412-157">Besitzt Skype For Business-Lizenz</span><span class="sxs-lookup"><span data-stu-id="3f412-157">Has Skype For Business License</span></span>
- <span data-ttu-id="3f412-158">Besitzt Yammer-Lizenz</span><span class="sxs-lookup"><span data-stu-id="3f412-158">Has Yammer License</span></span>
- <span data-ttu-id="3f412-159">Besitzt Teams-Lizenz</span><span class="sxs-lookup"><span data-stu-id="3f412-159">Has Teams License</span></span>
- <span data-ttu-id="3f412-160">Datum der letzten Exchange-Aktivität</span><span class="sxs-lookup"><span data-stu-id="3f412-160">Exchange Last Activity Date</span></span>
- <span data-ttu-id="3f412-161">Datum der letzten OneDrive-Aktivität</span><span class="sxs-lookup"><span data-stu-id="3f412-161">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="3f412-162">Datum der letzten SharePoint-Aktivität</span><span class="sxs-lookup"><span data-stu-id="3f412-162">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="3f412-163">Datum der letzten Skype for Business-Aktivität</span><span class="sxs-lookup"><span data-stu-id="3f412-163">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="3f412-164">Datum der letzten Yammer-Aktivität</span><span class="sxs-lookup"><span data-stu-id="3f412-164">Yammer Last Activity Date</span></span>
- <span data-ttu-id="3f412-165">Datum der letzten Teams-Aktivität</span><span class="sxs-lookup"><span data-stu-id="3f412-165">Teams Last Activity Date</span></span>
- <span data-ttu-id="3f412-166">Datum der Exchange-Lizenzzuweisung</span><span class="sxs-lookup"><span data-stu-id="3f412-166">Exchange License Assign Date</span></span>
- <span data-ttu-id="3f412-167">Datum der OneDrive-Lizenzzuweisung</span><span class="sxs-lookup"><span data-stu-id="3f412-167">OneDrive License Assign Date</span></span>
- <span data-ttu-id="3f412-168">Datum der SharePoint-Lizenzzuweisung</span><span class="sxs-lookup"><span data-stu-id="3f412-168">SharePoint License Assign Date</span></span>
- <span data-ttu-id="3f412-169">Datum der Skype For Business-Lizenzzuweisung</span><span class="sxs-lookup"><span data-stu-id="3f412-169">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="3f412-170">Datum der Yammer-Lizenzzuweisung</span><span class="sxs-lookup"><span data-stu-id="3f412-170">Yammer License Assign Date</span></span>
- <span data-ttu-id="3f412-171">Datum der Teams-Lizenzzuweisung</span><span class="sxs-lookup"><span data-stu-id="3f412-171">Teams License Assign Date</span></span>
- <span data-ttu-id="3f412-172">Zugewiesene Produkte</span><span class="sxs-lookup"><span data-stu-id="3f412-172">Assigned Products</span></span>

<span data-ttu-id="3f412-173">Die folgenden Spalten werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt:</span><span class="sxs-lookup"><span data-stu-id="3f412-173">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="3f412-174">Besitzt Yammer-Lizenz</span><span class="sxs-lookup"><span data-stu-id="3f412-174">Has Yammer License</span></span>
- <span data-ttu-id="3f412-175">Besitzt Teams-Lizenz</span><span class="sxs-lookup"><span data-stu-id="3f412-175">Has Teams License</span></span>
- <span data-ttu-id="3f412-176">Datum der letzten Yammer-Aktivität</span><span class="sxs-lookup"><span data-stu-id="3f412-176">Yammer Last Activity Date</span></span>
- <span data-ttu-id="3f412-177">Datum der letzten Teams-Aktivität</span><span class="sxs-lookup"><span data-stu-id="3f412-177">Teams Last Activity Date</span></span>
- <span data-ttu-id="3f412-178">Datum der Yammer-Lizenzzuweisung</span><span class="sxs-lookup"><span data-stu-id="3f412-178">Yammer License Assign Date</span></span>
- <span data-ttu-id="3f412-179">Datum der Teams-Lizenzzuweisung</span><span class="sxs-lookup"><span data-stu-id="3f412-179">Teams License Assign Date</span></span>

### <a name="json"></a><span data-ttu-id="3f412-180">JSON</span><span class="sxs-lookup"><span data-stu-id="3f412-180">JSON</span></span>

<span data-ttu-id="3f412-181">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3f412-181">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="3f412-182">Die folgenden Eigenschaften im **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** -Objekt werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt:</span><span class="sxs-lookup"><span data-stu-id="3f412-182">The following properties in **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="3f412-183">hasYammerLicense</span><span class="sxs-lookup"><span data-stu-id="3f412-183">hasYammerLicense</span></span>
- <span data-ttu-id="3f412-184">hasTeamsLicense</span><span class="sxs-lookup"><span data-stu-id="3f412-184">hasTeamsLicense</span></span>
- <span data-ttu-id="3f412-185">yammerLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="3f412-185">yammerLastActivityDate</span></span>
- <span data-ttu-id="3f412-186">teamsLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="3f412-186">teamsLastActivityDate</span></span>
- <span data-ttu-id="3f412-187">yammerLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="3f412-187">yammerLicenseAssignDate</span></span>
- <span data-ttu-id="3f412-188">teamsLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="3f412-188">teamsLicenseAssignDate</span></span>

<span data-ttu-id="3f412-189">Die Seite Standardgröße für diese Anforderung ist 200 Elemente.</span><span class="sxs-lookup"><span data-stu-id="3f412-189">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="3f412-190">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3f412-190">Example</span></span>

### <a name="csv"></a><span data-ttu-id="3f412-191">CSV</span><span class="sxs-lookup"><span data-stu-id="3f412-191">CSV</span></span>

<span data-ttu-id="3f412-192">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="3f412-192">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3f412-193">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3f412-193">Request</span></span>

<span data-ttu-id="3f412-194">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3f412-194">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="3f412-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="3f412-195">Response</span></span>

<span data-ttu-id="3f412-196">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3f412-196">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3f412-197">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="3f412-197">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Has Exchange License,Has OneDrive License,Has SharePoint License,Has Skype For Business License,Has Yammer License,Has Teams License,Exchange Last Activity Date,OneDrive Last Activity Date,SharePoint Last Activity Date,Skype For Business Last Activity Date,Yammer Last Activity Date,Teams Last Activity Date,Exchange License Assign Date,OneDrive License Assign Date,SharePoint License Assign Date,Skype For Business License Assign Date,Yammer License Assign Date,Teams License Assign Date,Assigned Products
```

### <a name="json"></a><span data-ttu-id="3f412-198">JSON</span><span class="sxs-lookup"><span data-stu-id="3f412-198">JSON</span></span>

<span data-ttu-id="3f412-199">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3f412-199">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3f412-200">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3f412-200">Request</span></span>

<span data-ttu-id="3f412-201">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3f412-201">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="3f412-202">Antwort</span><span class="sxs-lookup"><span data-stu-id="3f412-202">Response</span></span>

<span data-ttu-id="3f412-203">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3f412-203">The following is an example of the response.</span></span>

> <span data-ttu-id="3f412-p107">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="3f412-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActiveUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 853

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActiveUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userprincipalname-value", 
      "displayName": "displayname-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "hasExchangeLicense": true, 
      "hasOneDriveLicense": false, 
      "hasSharePointLicense": false, 
      "hasSkypeForBusinessLicense": false, 
      "hasYammerLicense": false, 
      "hasTeamsLicense": false, 
      "exchangeLastActivityDate": "2017-08-30", 
      "oneDriveLastActivityDate": null, 
      "sharePointLastActivityDate": null, 
      "skypeForBusinessLastActivityDate": null, 
      "yammerLastActivityDate": null, 
      "teamsLastActivityDate": null, 
      "exchangeLicenseAssignDate": "2016-05-03", 
      "oneDriveLicenseAssignDate": null, 
      "sharePointLicenseAssignDate": null, 
      "skypeForBusinessLicenseAssignDate": null, 
      "yammerLicenseAssignDate": null, 
      "teamsLicenseAssignDate": null, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ]
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365activeuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
