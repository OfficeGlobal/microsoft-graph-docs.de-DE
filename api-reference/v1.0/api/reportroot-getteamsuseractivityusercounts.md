---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: Diese Methode ruft die Anzahl von Microsoft Teams-Benutzern nach Aktivitätstyp ab. Die Aktivitätstypen geben die Anzahl von Chatnachrichten, privaten Chatnachrichten, Anrufen oder Besprechungen der Teams an.
localization_priority: Normal
ms.openlocfilehash: 5db9ccb20d79e487b564487f528c7f90289123e0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831297"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="28116-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="28116-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

<span data-ttu-id="28116-105">Diese Methode ruft die Anzahl von Microsoft Teams-Benutzern nach Aktivitätstyp ab.</span><span class="sxs-lookup"><span data-stu-id="28116-105">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="28116-106">Die Aktivitätstypen geben die Anzahl von Chatnachrichten, privaten Chatnachrichten, Anrufen oder Besprechungen der Teams an.</span><span class="sxs-lookup"><span data-stu-id="28116-106">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="28116-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="28116-107">Permissions</span></span>

<span data-ttu-id="28116-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28116-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="28116-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="28116-110">Permission type</span></span>                        | <span data-ttu-id="28116-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="28116-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="28116-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="28116-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="28116-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="28116-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="28116-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="28116-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28116-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28116-115">Not supported.</span></span>                           |
| <span data-ttu-id="28116-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="28116-116">Application</span></span>                            | <span data-ttu-id="28116-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="28116-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="28116-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="28116-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="28116-119">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="28116-119">Function parameters</span></span>

<span data-ttu-id="28116-120">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="28116-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="28116-121">Parameter</span><span class="sxs-lookup"><span data-stu-id="28116-121">Parameter</span></span> | <span data-ttu-id="28116-122">Typ</span><span class="sxs-lookup"><span data-stu-id="28116-122">Type</span></span>   | <span data-ttu-id="28116-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28116-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="28116-124">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="28116-124">period</span></span>    | <span data-ttu-id="28116-125">string</span><span class="sxs-lookup"><span data-stu-id="28116-125">string</span></span> | <span data-ttu-id="28116-126">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="28116-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="28116-127">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="28116-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="28116-128">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="28116-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="28116-129">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="28116-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="28116-130">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="28116-130">Request headers</span></span>

| <span data-ttu-id="28116-131">Name</span><span class="sxs-lookup"><span data-stu-id="28116-131">Name</span></span>          | <span data-ttu-id="28116-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28116-132">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="28116-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="28116-133">Authorization</span></span> | <span data-ttu-id="28116-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="28116-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="28116-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="28116-136">Response</span></span>

<span data-ttu-id="28116-137">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="28116-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="28116-138">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="28116-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="28116-139">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="28116-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="28116-140">Die CSV-Datei verfügt über die folgenden Spaltenheader:</span><span class="sxs-lookup"><span data-stu-id="28116-140">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="28116-141">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="28116-141">Report Refresh Date</span></span>
- <span data-ttu-id="28116-142">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="28116-142">Report Date</span></span>
- <span data-ttu-id="28116-143">Team-Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="28116-143">Team Chat Messages</span></span>
- <span data-ttu-id="28116-144">Private Chatnachrichten</span><span class="sxs-lookup"><span data-stu-id="28116-144">Private Chat Messages</span></span>
- <span data-ttu-id="28116-145">Anrufe</span><span class="sxs-lookup"><span data-stu-id="28116-145">Calls</span></span>
- <span data-ttu-id="28116-146">Besprechungen</span><span class="sxs-lookup"><span data-stu-id="28116-146">Meetings</span></span>
- <span data-ttu-id="28116-147">Sonstige Aktionen</span><span class="sxs-lookup"><span data-stu-id="28116-147">Other Actions</span></span>
- <span data-ttu-id="28116-148">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="28116-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="28116-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="28116-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="28116-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="28116-150">Request</span></span>

<span data-ttu-id="28116-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="28116-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="28116-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="28116-152">Response</span></span>

<span data-ttu-id="28116-153">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="28116-153">The following is an example of the response.</span></span>

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

<span data-ttu-id="28116-154">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="28116-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Other Actions,Report Period
```
