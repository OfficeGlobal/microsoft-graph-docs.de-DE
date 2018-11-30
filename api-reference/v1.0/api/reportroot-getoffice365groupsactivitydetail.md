---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: Rufen Sie Details zur Office 365-Gruppenaktivität nach Gruppe ab.
ms.openlocfilehash: 18ff1ea1ee3bfc90cbf86bb4e99321198c583f06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018691"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="7b058-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="7b058-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

<span data-ttu-id="7b058-104">Rufen Sie Details zur Office 365-Gruppenaktivität nach Gruppe ab.</span><span class="sxs-lookup"><span data-stu-id="7b058-104">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="7b058-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Office 365-Gruppen](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="7b058-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="7b058-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7b058-106">Permissions</span></span>

<span data-ttu-id="7b058-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b058-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7b058-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7b058-109">Permission type</span></span>                        | <span data-ttu-id="7b058-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7b058-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7b058-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7b058-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7b058-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b058-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7b058-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7b058-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b058-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b058-114">Not supported.</span></span>                           |
| <span data-ttu-id="7b058-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7b058-115">Application</span></span>                            | <span data-ttu-id="7b058-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b058-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7b058-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b058-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="7b058-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="7b058-118">Function parameters</span></span>

<span data-ttu-id="7b058-119">Geben Sie in der Anforderungs-URL einen der folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="7b058-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="7b058-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="7b058-120">Parameter</span></span> | <span data-ttu-id="7b058-121">Typ</span><span class="sxs-lookup"><span data-stu-id="7b058-121">Type</span></span>   | <span data-ttu-id="7b058-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b058-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7b058-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="7b058-123">period</span></span>    | <span data-ttu-id="7b058-124">string</span><span class="sxs-lookup"><span data-stu-id="7b058-124">string</span></span> | <span data-ttu-id="7b058-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="7b058-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7b058-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="7b058-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7b058-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="7b058-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="7b058-128">date</span><span class="sxs-lookup"><span data-stu-id="7b058-128">date</span></span>      | <span data-ttu-id="7b058-129">Datum</span><span class="sxs-lookup"><span data-stu-id="7b058-129">Date</span></span>   | <span data-ttu-id="7b058-130">Gibt das Datum an, für das die Benutzer angezeigt werden sollen, die Aktivitäten durchgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="7b058-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="7b058-131">{date_value} muss im Format JJJJ-MM-TT vorliegen.</span><span class="sxs-lookup"><span data-stu-id="7b058-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="7b058-132">Da dieser Bericht nur für die letzten 30 Tage verfügbar ist, sollte {date_value} ein Datum aus diesem Zeitraum sein.</span><span class="sxs-lookup"><span data-stu-id="7b058-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="7b058-133">**Hinweis:** Sie müssen in der URL entweder einen Zeitraum oder ein Datum festlegen.</span><span class="sxs-lookup"><span data-stu-id="7b058-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b058-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7b058-134">Request headers</span></span>

| <span data-ttu-id="7b058-135">Name</span><span class="sxs-lookup"><span data-stu-id="7b058-135">Name</span></span>          | <span data-ttu-id="7b058-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b058-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="7b058-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b058-137">Authorization</span></span> | <span data-ttu-id="7b058-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7b058-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="7b058-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="7b058-140">If-None-Match</span></span> | <span data-ttu-id="7b058-141">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7b058-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="7b058-142">Optional.</span><span class="sxs-lookup"><span data-stu-id="7b058-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="7b058-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b058-143">Response</span></span>

<span data-ttu-id="7b058-144">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="7b058-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7b058-145">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7b058-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7b058-146">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="7b058-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7b058-147">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="7b058-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7b058-148">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="7b058-148">Report Refresh Date</span></span>
- <span data-ttu-id="7b058-149">Gruppenanzeigename</span><span class="sxs-lookup"><span data-stu-id="7b058-149">Group Display Name</span></span>
- <span data-ttu-id="7b058-150">Ist gelöscht</span><span class="sxs-lookup"><span data-stu-id="7b058-150">Is Deleted</span></span>
- <span data-ttu-id="7b058-151">Besitzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="7b058-151">Owner Principal Name</span></span>
- <span data-ttu-id="7b058-152">Datum der letzten Aktivität</span><span class="sxs-lookup"><span data-stu-id="7b058-152">Last Activity Date</span></span>
- <span data-ttu-id="7b058-153">Gruppentyp</span><span class="sxs-lookup"><span data-stu-id="7b058-153">Group Type</span></span>
- <span data-ttu-id="7b058-154">Mitgliederzahl</span><span class="sxs-lookup"><span data-stu-id="7b058-154">Member Count</span></span>
- <span data-ttu-id="7b058-155">Anzahl der externen Mitglieder</span><span class="sxs-lookup"><span data-stu-id="7b058-155">External Member Count</span></span>
- <span data-ttu-id="7b058-156">Anzahl der mit Exchange empfangenen E-Mail-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="7b058-156">Exchange Received Email Count</span></span>
- <span data-ttu-id="7b058-157">Anzahl der aktiven SharePoint-Dateien</span><span class="sxs-lookup"><span data-stu-id="7b058-157">SharePoint Active File Count</span></span>
- <span data-ttu-id="7b058-158">Anzahl der veröffentlichten Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="7b058-158">Yammer Posted Message Count</span></span>
- <span data-ttu-id="7b058-159">Anzahl der gelesenen Yammer-Nachricht</span><span class="sxs-lookup"><span data-stu-id="7b058-159">Yammer Read Message Count</span></span>
- <span data-ttu-id="7b058-160">Anzahl der gelikten Yammer-Nachrichten</span><span class="sxs-lookup"><span data-stu-id="7b058-160">Yammer Liked Message Count</span></span>
- <span data-ttu-id="7b058-161">Gesamtanzahl der Exchange-Postfachelemente</span><span class="sxs-lookup"><span data-stu-id="7b058-161">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="7b058-162">Verwendeter Exchange-Postfachspeicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="7b058-162">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="7b058-163">Gesamtzahl der SharePoint-Dateien</span><span class="sxs-lookup"><span data-stu-id="7b058-163">SharePoint Total File Count</span></span>
- <span data-ttu-id="7b058-164">Verwendeter SharePoint-Websitesspeicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="7b058-164">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="7b058-165">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="7b058-165">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="7b058-166">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7b058-166">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7b058-167">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b058-167">Request</span></span>

<span data-ttu-id="7b058-168">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7b058-168">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="7b058-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b058-169">Response</span></span>

<span data-ttu-id="7b058-170">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7b058-170">The following is an example of the response.</span></span>

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

<span data-ttu-id="7b058-171">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="7b058-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,Guest Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Report Period
```