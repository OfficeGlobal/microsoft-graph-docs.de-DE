---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: Rufen Sie die Anzahl der Benutzer nach Aktivitätstyp und Dienst ab.
ms.openlocfilehash: ce594cc38ba62d70ee0a849342a6c2add0b3e602
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018465"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="88bda-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="88bda-103">reportRoot: getOffice365ServicesUserCounts</span></span>

<span data-ttu-id="88bda-104">Rufen Sie die Anzahl der Benutzer nach Aktivitätstyp und Dienst ab.</span><span class="sxs-lookup"><span data-stu-id="88bda-104">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="88bda-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Aktive Benutzer](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="88bda-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="88bda-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="88bda-106">Permissions</span></span>

<span data-ttu-id="88bda-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88bda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="88bda-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="88bda-109">Permission type</span></span>                        | <span data-ttu-id="88bda-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="88bda-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="88bda-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="88bda-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="88bda-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="88bda-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="88bda-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="88bda-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88bda-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="88bda-114">Not supported.</span></span>                           |
| <span data-ttu-id="88bda-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="88bda-115">Application</span></span>                            | <span data-ttu-id="88bda-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="88bda-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="88bda-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="88bda-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="88bda-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="88bda-118">Function parameters</span></span>

<span data-ttu-id="88bda-119">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="88bda-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="88bda-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="88bda-120">Parameter</span></span> | <span data-ttu-id="88bda-121">Typ</span><span class="sxs-lookup"><span data-stu-id="88bda-121">Type</span></span>   | <span data-ttu-id="88bda-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88bda-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="88bda-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="88bda-123">period</span></span>    | <span data-ttu-id="88bda-124">string</span><span class="sxs-lookup"><span data-stu-id="88bda-124">string</span></span> | <span data-ttu-id="88bda-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="88bda-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="88bda-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="88bda-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="88bda-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="88bda-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="88bda-128">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="88bda-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="88bda-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="88bda-129">Request headers</span></span>

| <span data-ttu-id="88bda-130">Name</span><span class="sxs-lookup"><span data-stu-id="88bda-130">Name</span></span>          | <span data-ttu-id="88bda-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88bda-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="88bda-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="88bda-132">Authorization</span></span> | <span data-ttu-id="88bda-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="88bda-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="88bda-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="88bda-135">If-None-Match</span></span> | <span data-ttu-id="88bda-136">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen Tag in der Datei übereinstimmt, wird ein `304 Not Modified`-Antwortcode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="88bda-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="88bda-137">Optional.</span><span class="sxs-lookup"><span data-stu-id="88bda-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="88bda-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="88bda-138">Response</span></span>

<span data-ttu-id="88bda-139">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="88bda-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="88bda-140">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="88bda-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="88bda-141">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="88bda-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="88bda-142">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="88bda-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="88bda-143">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="88bda-143">Report Refresh Date</span></span>
- <span data-ttu-id="88bda-144">Exchange aktiv</span><span class="sxs-lookup"><span data-stu-id="88bda-144">Exchange Active</span></span>
- <span data-ttu-id="88bda-145">Exchange inaktiv</span><span class="sxs-lookup"><span data-stu-id="88bda-145">Exchange Inactive</span></span>
- <span data-ttu-id="88bda-146">OneDrive aktiv</span><span class="sxs-lookup"><span data-stu-id="88bda-146">OneDrive Active</span></span>
- <span data-ttu-id="88bda-147">OneDrive inaktiv</span><span class="sxs-lookup"><span data-stu-id="88bda-147">OneDrive Inactive</span></span>
- <span data-ttu-id="88bda-148">SharePoint aktiv</span><span class="sxs-lookup"><span data-stu-id="88bda-148">SharePoint Active</span></span>
- <span data-ttu-id="88bda-149">SharePoint inaktiv</span><span class="sxs-lookup"><span data-stu-id="88bda-149">SharePoint Inactive</span></span>
- <span data-ttu-id="88bda-150">Skype for Business aktiv</span><span class="sxs-lookup"><span data-stu-id="88bda-150">Skype For Business Active</span></span>
- <span data-ttu-id="88bda-151">Skype for Business inaktiv</span><span class="sxs-lookup"><span data-stu-id="88bda-151">Skype For Business Inactive</span></span>
- <span data-ttu-id="88bda-152">Yammer aktiv</span><span class="sxs-lookup"><span data-stu-id="88bda-152">Yammer Active</span></span>
- <span data-ttu-id="88bda-153">Yammer inaktiv</span><span class="sxs-lookup"><span data-stu-id="88bda-153">Yammer Inactive</span></span>
- <span data-ttu-id="88bda-154">Teams aktiv</span><span class="sxs-lookup"><span data-stu-id="88bda-154">Teams Active</span></span>
- <span data-ttu-id="88bda-155">Teams inaktiv</span><span class="sxs-lookup"><span data-stu-id="88bda-155">Teams Inactive</span></span>
- <span data-ttu-id="88bda-156">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="88bda-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="88bda-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="88bda-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="88bda-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="88bda-158">Request</span></span>

<span data-ttu-id="88bda-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="88bda-159">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365servicesusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ServicesUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="88bda-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="88bda-160">Response</span></span>

<span data-ttu-id="88bda-161">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="88bda-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="88bda-162">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="88bda-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Report Period
```
