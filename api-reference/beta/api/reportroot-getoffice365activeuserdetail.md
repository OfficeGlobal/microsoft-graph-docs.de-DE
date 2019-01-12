---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: Rufen Sie Details zu aktiven Office 365-Benutzern ab.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: ff9df2d2eb6c00990ac93e324f47f92fea8003de
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934709"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="b28c5-103">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="b28c5-103">reportRoot: getOffice365ActiveUserDetail</span></span>

> <span data-ttu-id="b28c5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b28c5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b28c5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b28c5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b28c5-106">Rufen Sie Details zu aktiven Office 365-Benutzern ab.</span><span class="sxs-lookup"><span data-stu-id="b28c5-106">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="b28c5-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Aktive Benutzer](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="b28c5-107">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="b28c5-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b28c5-108">Permissions</span></span>

<span data-ttu-id="b28c5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b28c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b28c5-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b28c5-111">Permission type</span></span>                        | <span data-ttu-id="b28c5-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b28c5-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b28c5-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b28c5-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b28c5-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b28c5-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b28c5-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b28c5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b28c5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b28c5-116">Not supported.</span></span>                           |
| <span data-ttu-id="b28c5-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b28c5-117">Application</span></span>                            | <span data-ttu-id="b28c5-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b28c5-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b28c5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b28c5-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="b28c5-120">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="b28c5-120">Function parameters</span></span>

<span data-ttu-id="b28c5-121">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="b28c5-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="b28c5-122">Parameter</span><span class="sxs-lookup"><span data-stu-id="b28c5-122">Parameter</span></span> | <span data-ttu-id="b28c5-123">Typ</span><span class="sxs-lookup"><span data-stu-id="b28c5-123">Type</span></span>   | <span data-ttu-id="b28c5-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b28c5-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b28c5-125">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="b28c5-125">period</span></span>    | <span data-ttu-id="b28c5-126">string</span><span class="sxs-lookup"><span data-stu-id="b28c5-126">string</span></span> | <span data-ttu-id="b28c5-127">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="b28c5-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b28c5-128">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="b28c5-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b28c5-129">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="b28c5-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="b28c5-130">date</span><span class="sxs-lookup"><span data-stu-id="b28c5-130">date</span></span>      | <span data-ttu-id="b28c5-131">Datum</span><span class="sxs-lookup"><span data-stu-id="b28c5-131">Date</span></span>   | <span data-ttu-id="b28c5-132">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="b28c5-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="b28c5-133">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="b28c5-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="b28c5-134">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="b28c5-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="b28c5-135">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="b28c5-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="b28c5-136">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von  `$format`, `$top` und `$skipToken` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b28c5-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b28c5-137">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="b28c5-137">The default output type is text/csv.</span></span> <span data-ttu-id="b28c5-138">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="b28c5-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b28c5-139">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b28c5-139">Request headers</span></span>

| <span data-ttu-id="b28c5-140">Name</span><span class="sxs-lookup"><span data-stu-id="b28c5-140">Name</span></span>          | <span data-ttu-id="b28c5-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b28c5-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b28c5-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="b28c5-142">Authorization</span></span> | <span data-ttu-id="b28c5-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b28c5-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b28c5-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="b28c5-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b28c5-146">CSV</span><span class="sxs-lookup"><span data-stu-id="b28c5-146">CSV</span></span>

<span data-ttu-id="b28c5-147">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="b28c5-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b28c5-148">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b28c5-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b28c5-149">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="b28c5-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b28c5-150">Die CSV-Datei verfügt über die folgenden Spaltenheader:</span><span class="sxs-lookup"><span data-stu-id="b28c5-150">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="b28c5-151">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="b28c5-151">Report Refresh Date</span></span>
- <span data-ttu-id="b28c5-152">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="b28c5-152">User Principal Name</span></span>
- <span data-ttu-id="b28c5-153">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="b28c5-153">Display Name</span></span>
- <span data-ttu-id="b28c5-154">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="b28c5-154">Is Deleted</span></span>
- <span data-ttu-id="b28c5-155">Gelöscht am</span><span class="sxs-lookup"><span data-stu-id="b28c5-155">Deleted Date</span></span>
- <span data-ttu-id="b28c5-156">Besitzt Exchange-Lizenz</span><span class="sxs-lookup"><span data-stu-id="b28c5-156">Has Exchange License</span></span>
- <span data-ttu-id="b28c5-157">Besitzt OneDrive-Lizenz</span><span class="sxs-lookup"><span data-stu-id="b28c5-157">Has OneDrive License</span></span>
- <span data-ttu-id="b28c5-158">Besitzt SharePoint-Lizenz</span><span class="sxs-lookup"><span data-stu-id="b28c5-158">Has SharePoint License</span></span>
- <span data-ttu-id="b28c5-159">Besitzt Skype For Business-Lizenz</span><span class="sxs-lookup"><span data-stu-id="b28c5-159">Has Skype For Business License</span></span>
- <span data-ttu-id="b28c5-160">Besitzt Yammer-Lizenz</span><span class="sxs-lookup"><span data-stu-id="b28c5-160">Has Yammer License</span></span>
- <span data-ttu-id="b28c5-161">Besitzt Teams-Lizenz</span><span class="sxs-lookup"><span data-stu-id="b28c5-161">Has Teams License</span></span>
- <span data-ttu-id="b28c5-162">Datum der letzten Exchange-Aktivität</span><span class="sxs-lookup"><span data-stu-id="b28c5-162">Exchange Last Activity Date</span></span>
- <span data-ttu-id="b28c5-163">Datum der letzten OneDrive-Aktivität</span><span class="sxs-lookup"><span data-stu-id="b28c5-163">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="b28c5-164">Datum der letzten SharePoint-Aktivität</span><span class="sxs-lookup"><span data-stu-id="b28c5-164">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="b28c5-165">Datum der letzten Skype for Business-Aktivität</span><span class="sxs-lookup"><span data-stu-id="b28c5-165">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="b28c5-166">Datum der letzten Yammer-Aktivität</span><span class="sxs-lookup"><span data-stu-id="b28c5-166">Yammer Last Activity Date</span></span>
- <span data-ttu-id="b28c5-167">Datum der letzten Teams-Aktivität</span><span class="sxs-lookup"><span data-stu-id="b28c5-167">Teams Last Activity Date</span></span>
- <span data-ttu-id="b28c5-168">Datum der Exchange-Lizenzzuweisung</span><span class="sxs-lookup"><span data-stu-id="b28c5-168">Exchange License Assign Date</span></span>
- <span data-ttu-id="b28c5-169">Datum der OneDrive-Lizenzzuweisung</span><span class="sxs-lookup"><span data-stu-id="b28c5-169">OneDrive License Assign Date</span></span>
- <span data-ttu-id="b28c5-170">Datum der SharePoint-Lizenzzuweisung</span><span class="sxs-lookup"><span data-stu-id="b28c5-170">SharePoint License Assign Date</span></span>
- <span data-ttu-id="b28c5-171">Datum der Skype For Business-Lizenzzuweisung</span><span class="sxs-lookup"><span data-stu-id="b28c5-171">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="b28c5-172">Datum der Yammer-Lizenzzuweisung</span><span class="sxs-lookup"><span data-stu-id="b28c5-172">Yammer License Assign Date</span></span>
- <span data-ttu-id="b28c5-173">Datum der Teams-Lizenzzuweisung</span><span class="sxs-lookup"><span data-stu-id="b28c5-173">Teams License Assign Date</span></span>
- <span data-ttu-id="b28c5-174">Zugewiesene Produkte</span><span class="sxs-lookup"><span data-stu-id="b28c5-174">Assigned Products</span></span>

<span data-ttu-id="b28c5-175">Die folgenden Spalten werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt:</span><span class="sxs-lookup"><span data-stu-id="b28c5-175">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="b28c5-176">Besitzt Yammer-Lizenz</span><span class="sxs-lookup"><span data-stu-id="b28c5-176">Has Yammer License</span></span>
- <span data-ttu-id="b28c5-177">Besitzt Teams-Lizenz</span><span class="sxs-lookup"><span data-stu-id="b28c5-177">Has Teams License</span></span>
- <span data-ttu-id="b28c5-178">Datum der letzten Yammer-Aktivität</span><span class="sxs-lookup"><span data-stu-id="b28c5-178">Yammer Last Activity Date</span></span>
- <span data-ttu-id="b28c5-179">Datum der letzten Teams-Aktivität</span><span class="sxs-lookup"><span data-stu-id="b28c5-179">Teams Last Activity Date</span></span>
- <span data-ttu-id="b28c5-180">Datum der Yammer-Lizenzzuweisung</span><span class="sxs-lookup"><span data-stu-id="b28c5-180">Yammer License Assign Date</span></span>
- <span data-ttu-id="b28c5-181">Datum der Teams-Lizenzzuweisung</span><span class="sxs-lookup"><span data-stu-id="b28c5-181">Teams License Assign Date</span></span>

### <a name="json"></a><span data-ttu-id="b28c5-182">JSON</span><span class="sxs-lookup"><span data-stu-id="b28c5-182">JSON</span></span>

<span data-ttu-id="b28c5-183">Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Antwortcode und eines **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b28c5-183">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="b28c5-184">Die folgenden Eigenschaften im **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** -Objekt werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt:</span><span class="sxs-lookup"><span data-stu-id="b28c5-184">The following properties in **[office365ActiveUserDetail](../resources/office365activeuserdetail.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="b28c5-185">hasYammerLicense</span><span class="sxs-lookup"><span data-stu-id="b28c5-185">hasYammerLicense</span></span>
- <span data-ttu-id="b28c5-186">hasTeamsLicense</span><span class="sxs-lookup"><span data-stu-id="b28c5-186">hasTeamsLicense</span></span>
- <span data-ttu-id="b28c5-187">yammerLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="b28c5-187">yammerLastActivityDate</span></span>
- <span data-ttu-id="b28c5-188">teamsLastActivityDate</span><span class="sxs-lookup"><span data-stu-id="b28c5-188">teamsLastActivityDate</span></span>
- <span data-ttu-id="b28c5-189">yammerLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="b28c5-189">yammerLicenseAssignDate</span></span>
- <span data-ttu-id="b28c5-190">teamsLicenseAssignDate</span><span class="sxs-lookup"><span data-stu-id="b28c5-190">teamsLicenseAssignDate</span></span>

<span data-ttu-id="b28c5-191">Die Seite Standardgröße für diese Anforderung ist 200 Elemente.</span><span class="sxs-lookup"><span data-stu-id="b28c5-191">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="b28c5-192">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b28c5-192">Example</span></span>

### <a name="csv"></a><span data-ttu-id="b28c5-193">CSV</span><span class="sxs-lookup"><span data-stu-id="b28c5-193">CSV</span></span>

<span data-ttu-id="b28c5-194">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="b28c5-194">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="b28c5-195">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b28c5-195">Request</span></span>

<span data-ttu-id="b28c5-196">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b28c5-196">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="b28c5-197">Antwort</span><span class="sxs-lookup"><span data-stu-id="b28c5-197">Response</span></span>

<span data-ttu-id="b28c5-198">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b28c5-198">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b28c5-199">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="b28c5-199">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="b28c5-200">JSON</span><span class="sxs-lookup"><span data-stu-id="b28c5-200">JSON</span></span>

<span data-ttu-id="b28c5-201">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b28c5-201">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b28c5-202">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b28c5-202">Request</span></span>

<span data-ttu-id="b28c5-203">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b28c5-203">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="b28c5-204">Antwort</span><span class="sxs-lookup"><span data-stu-id="b28c5-204">Response</span></span>

<span data-ttu-id="b28c5-205">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b28c5-205">The following is an example of the response.</span></span>

> <span data-ttu-id="b28c5-p108">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="b28c5-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
