---
title: 'reportRoot: getEmailAppUsageAppsUserCounts'
description: Rufen Sie die Anzahl der eindeutigen Benutzer pro E-Mail-App ab.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 6befae80844ca88eb8668564acacac64d3003bb2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912043"
---
# <a name="reportroot-getemailappusageappsusercounts"></a><span data-ttu-id="0f6ff-103">reportRoot: getEmailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="0f6ff-103">reportRoot: getEmailAppUsageAppsUserCounts</span></span>

<span data-ttu-id="0f6ff-104">Rufen Sie die Anzahl der eindeutigen Benutzer pro E-Mail-App ab.</span><span class="sxs-lookup"><span data-stu-id="0f6ff-104">Get the count of unique users per email app.</span></span>

> <span data-ttu-id="0f6ff-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Nutzung von E-Mail-Apps](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="0f6ff-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="0f6ff-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0f6ff-106">Permissions</span></span>

<span data-ttu-id="0f6ff-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f6ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0f6ff-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0f6ff-109">Permission type</span></span>                        | <span data-ttu-id="0f6ff-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0f6ff-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0f6ff-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0f6ff-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0f6ff-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f6ff-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0f6ff-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0f6ff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f6ff-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0f6ff-114">Not supported.</span></span>                           |
| <span data-ttu-id="0f6ff-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0f6ff-115">Application</span></span>                            | <span data-ttu-id="0f6ff-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f6ff-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0f6ff-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f6ff-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageAppsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="0f6ff-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="0f6ff-118">Function parameters</span></span>

<span data-ttu-id="0f6ff-119">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="0f6ff-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0f6ff-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="0f6ff-120">Parameter</span></span> | <span data-ttu-id="0f6ff-121">Typ</span><span class="sxs-lookup"><span data-stu-id="0f6ff-121">Type</span></span>   | <span data-ttu-id="0f6ff-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f6ff-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0f6ff-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="0f6ff-123">period</span></span>    | <span data-ttu-id="0f6ff-124">string</span><span class="sxs-lookup"><span data-stu-id="0f6ff-124">string</span></span> | <span data-ttu-id="0f6ff-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="0f6ff-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0f6ff-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="0f6ff-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0f6ff-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="0f6ff-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0f6ff-128">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="0f6ff-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="0f6ff-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0f6ff-129">Request headers</span></span>

| <span data-ttu-id="0f6ff-130">Name</span><span class="sxs-lookup"><span data-stu-id="0f6ff-130">Name</span></span>          | <span data-ttu-id="0f6ff-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f6ff-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="0f6ff-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f6ff-132">Authorization</span></span> | <span data-ttu-id="0f6ff-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0f6ff-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="0f6ff-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="0f6ff-135">If-None-Match</span></span> | <span data-ttu-id="0f6ff-136">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f6ff-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="0f6ff-137">Optional.</span><span class="sxs-lookup"><span data-stu-id="0f6ff-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="0f6ff-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f6ff-138">Response</span></span>

<span data-ttu-id="0f6ff-139">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="0f6ff-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0f6ff-140">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0f6ff-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0f6ff-141">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="0f6ff-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0f6ff-142">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="0f6ff-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0f6ff-143">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="0f6ff-143">Report Refresh Date</span></span>
- <span data-ttu-id="0f6ff-144">E-Mail für Mac</span><span class="sxs-lookup"><span data-stu-id="0f6ff-144">Mail For Mac</span></span>
- <span data-ttu-id="0f6ff-145">Outlook für Mac</span><span class="sxs-lookup"><span data-stu-id="0f6ff-145">Outlook For Mac</span></span>
- <span data-ttu-id="0f6ff-146">Outlook für Windows</span><span class="sxs-lookup"><span data-stu-id="0f6ff-146">Outlook For Windows</span></span>
- <span data-ttu-id="0f6ff-147">Outlook für mobile Geräte</span><span class="sxs-lookup"><span data-stu-id="0f6ff-147">Outlook For Mobile</span></span>
- <span data-ttu-id="0f6ff-148">Weiteres für mobile Geräte</span><span class="sxs-lookup"><span data-stu-id="0f6ff-148">Other For Mobile</span></span>
- <span data-ttu-id="0f6ff-149">Outlook für Web</span><span class="sxs-lookup"><span data-stu-id="0f6ff-149">Outlook For Web</span></span>
- <span data-ttu-id="0f6ff-150">POP3-App</span><span class="sxs-lookup"><span data-stu-id="0f6ff-150">POP3 App</span></span>
- <span data-ttu-id="0f6ff-151">IMAP4-App</span><span class="sxs-lookup"><span data-stu-id="0f6ff-151">IMAP4 App</span></span>
- <span data-ttu-id="0f6ff-152">SMTP-App</span><span class="sxs-lookup"><span data-stu-id="0f6ff-152">SMTP App</span></span>
- <span data-ttu-id="0f6ff-153">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="0f6ff-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="0f6ff-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0f6ff-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0f6ff-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f6ff-155">Request</span></span>

<span data-ttu-id="0f6ff-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0f6ff-156">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageappsusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageAppsUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="0f6ff-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f6ff-157">Response</span></span>

<span data-ttu-id="0f6ff-158">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0f6ff-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="0f6ff-159">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="0f6ff-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
```
