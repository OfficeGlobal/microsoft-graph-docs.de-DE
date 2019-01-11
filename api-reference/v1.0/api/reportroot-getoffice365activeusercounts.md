---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: Rufen Sie die Anzahl der im Berichtszeitraum täglich aktiven Benutzer nach Produkt ab.
localization_priority: Normal
ms.openlocfilehash: 7b128ca1bad8cdf4c086edda2ada285e3910828d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809927"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="f8274-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="f8274-103">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="f8274-104">Rufen Sie die Anzahl der im Berichtszeitraum täglich aktiven Benutzer nach Produkt ab.</span><span class="sxs-lookup"><span data-stu-id="f8274-104">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="f8274-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Aktive Benutzer](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="f8274-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="f8274-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f8274-106">Permissions</span></span>

<span data-ttu-id="f8274-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8274-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f8274-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f8274-109">Permission type</span></span>                        | <span data-ttu-id="f8274-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f8274-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f8274-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f8274-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8274-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8274-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f8274-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f8274-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8274-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8274-114">Not supported.</span></span>                           |
| <span data-ttu-id="f8274-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f8274-115">Application</span></span>                            | <span data-ttu-id="f8274-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8274-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f8274-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8274-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f8274-118">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="f8274-118">Function parameters</span></span>

<span data-ttu-id="f8274-119">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="f8274-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f8274-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="f8274-120">Parameter</span></span> | <span data-ttu-id="f8274-121">Typ</span><span class="sxs-lookup"><span data-stu-id="f8274-121">Type</span></span>   | <span data-ttu-id="f8274-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8274-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f8274-123">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="f8274-123">period</span></span>    | <span data-ttu-id="f8274-124">string</span><span class="sxs-lookup"><span data-stu-id="f8274-124">string</span></span> | <span data-ttu-id="f8274-125">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="f8274-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f8274-126">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="f8274-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f8274-127">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="f8274-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f8274-128">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="f8274-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f8274-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f8274-129">Request headers</span></span>

| <span data-ttu-id="f8274-130">Name</span><span class="sxs-lookup"><span data-stu-id="f8274-130">Name</span></span>          | <span data-ttu-id="f8274-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8274-131">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f8274-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8274-132">Authorization</span></span> | <span data-ttu-id="f8274-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f8274-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f8274-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8274-135">Response</span></span>

<span data-ttu-id="f8274-136">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="f8274-136">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f8274-137">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f8274-137">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f8274-138">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="f8274-138">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f8274-139">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="f8274-139">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f8274-140">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="f8274-140">Report Refresh Date</span></span>
- <span data-ttu-id="f8274-141">Office 365</span><span class="sxs-lookup"><span data-stu-id="f8274-141">Office 365</span></span>
- <span data-ttu-id="f8274-142">Exchange</span><span class="sxs-lookup"><span data-stu-id="f8274-142">Exchange</span></span>
- <span data-ttu-id="f8274-143">OneDrive</span><span class="sxs-lookup"><span data-stu-id="f8274-143">OneDrive</span></span>
- <span data-ttu-id="f8274-144">SharePoint</span><span class="sxs-lookup"><span data-stu-id="f8274-144">SharePoint</span></span>
- <span data-ttu-id="f8274-145">Skype for Business</span><span class="sxs-lookup"><span data-stu-id="f8274-145">Skype For Business</span></span> 
- <span data-ttu-id="f8274-146">Yammer</span><span class="sxs-lookup"><span data-stu-id="f8274-146">Yammer</span></span>
- <span data-ttu-id="f8274-147">Teams</span><span class="sxs-lookup"><span data-stu-id="f8274-147">Teams</span></span>
- <span data-ttu-id="f8274-148">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="f8274-148">Report Date</span></span>
- <span data-ttu-id="f8274-149">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="f8274-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="f8274-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f8274-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f8274-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8274-151">Request</span></span>

<span data-ttu-id="f8274-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f8274-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="f8274-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8274-153">Response</span></span>

<span data-ttu-id="f8274-154">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f8274-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="f8274-155">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="f8274-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
```
