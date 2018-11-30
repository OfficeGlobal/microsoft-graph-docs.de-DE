---
title: 'reportRoot: getOffice365GroupsActivityStorage'
description: Rufen Sie den insgesamt für alle Gruppenpostfächer und Gruppenwebsites genutzten Speicherplatz ab.
ms.openlocfilehash: 636a23e8bb094e31c648a701a59f55a8c7c6c73d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019293"
---
# <a name="reportroot-getoffice365groupsactivitystorage"></a><span data-ttu-id="16c79-103">reportRoot: getOffice365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="16c79-103">reportRoot: getOffice365GroupsActivityStorage</span></span>

<span data-ttu-id="16c79-104">Rufen Sie den insgesamt für alle Gruppenpostfächer und Gruppenwebsites genutzten Speicherplatz ab.</span><span class="sxs-lookup"><span data-stu-id="16c79-104">Get the total storage used across all group mailboxes and group sites.</span></span>

> <span data-ttu-id="16c79-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Office 365-Gruppen](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="16c79-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="16c79-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="16c79-106">Permissions</span></span>

<span data-ttu-id="16c79-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16c79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="16c79-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="16c79-109">Permission type</span></span>                        | <span data-ttu-id="16c79-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="16c79-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="16c79-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="16c79-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="16c79-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="16c79-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="16c79-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="16c79-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16c79-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="16c79-114">Not supported.</span></span>                           |
| <span data-ttu-id="16c79-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="16c79-115">Application</span></span>                            | <span data-ttu-id="16c79-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="16c79-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="16c79-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="16c79-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="16c79-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="16c79-118">Function parameters</span></span>

<span data-ttu-id="16c79-119">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="16c79-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="16c79-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="16c79-120">Parameter</span></span> | <span data-ttu-id="16c79-121">Typ</span><span class="sxs-lookup"><span data-stu-id="16c79-121">Type</span></span>   | <span data-ttu-id="16c79-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16c79-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="16c79-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="16c79-123">period</span></span>    | <span data-ttu-id="16c79-124">string</span><span class="sxs-lookup"><span data-stu-id="16c79-124">string</span></span> | <span data-ttu-id="16c79-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="16c79-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="16c79-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="16c79-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="16c79-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="16c79-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="16c79-128">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="16c79-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="16c79-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="16c79-129">Request headers</span></span>

| <span data-ttu-id="16c79-130">Name</span><span class="sxs-lookup"><span data-stu-id="16c79-130">Name</span></span>          | <span data-ttu-id="16c79-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16c79-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="16c79-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="16c79-132">Authorization</span></span> | <span data-ttu-id="16c79-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="16c79-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="16c79-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="16c79-135">If-None-Match</span></span> | <span data-ttu-id="16c79-136">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="16c79-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="16c79-137">Optional.</span><span class="sxs-lookup"><span data-stu-id="16c79-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="16c79-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="16c79-138">Response</span></span>

<span data-ttu-id="16c79-139">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="16c79-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="16c79-140">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="16c79-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="16c79-141">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="16c79-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="16c79-142">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="16c79-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="16c79-143">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="16c79-143">Report Refresh Date</span></span>
- <span data-ttu-id="16c79-144">Verwendeter Postfachspeicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="16c79-144">Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="16c79-145">Verwendeter Websitesspeicherplatz (Byte)</span><span class="sxs-lookup"><span data-stu-id="16c79-145">Site Storage Used (Byte)</span></span>
- <span data-ttu-id="16c79-146">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="16c79-146">Report Date</span></span>
- <span data-ttu-id="16c79-147">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="16c79-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="16c79-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="16c79-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="16c79-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="16c79-149">Request</span></span>

<span data-ttu-id="16c79-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="16c79-150">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivitystorage"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityStorage(period='D7')
```

#### <a name="response"></a><span data-ttu-id="16c79-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="16c79-151">Response</span></span>

<span data-ttu-id="16c79-152">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="16c79-152">The following is an example of the response.</span></span>

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

<span data-ttu-id="16c79-153">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="16c79-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mailbox Storage Used (Byte),Site Storage Used (Byte),Report Date,Report Period
```