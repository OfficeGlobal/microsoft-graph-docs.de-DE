---
title: 'reportRoot: getSkypeForBusinessParticipantActivityUserCounts'
description: Erhalten Sie einen Überblick über die Anzahl der eindeutigen Benutzer und die Art von Konferenzsitzungen, an denen Benutzer aus Ihrer Organisation teilgenommen haben. Zu den Arten von Konferenzsitzungen gehören Chat, Audio/Video, Anwendungsfreigabe, Web und Einwahl/Auswahl (Drittanbieter).
ms.openlocfilehash: 25488376ddeb67a90623caa620dc71fe4c8fa7f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063701"
---
# <a name="reportroot-getskypeforbusinessparticipantactivityusercounts"></a><span data-ttu-id="9362b-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="9362b-104">reportRoot: getSkypeForBusinessParticipantActivityUserCounts</span></span>

> <span data-ttu-id="9362b-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9362b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9362b-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9362b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9362b-107">Erhalten Sie einen Überblick über die Anzahl der eindeutigen Benutzer und die Art von Konferenzsitzungen, an denen Benutzer aus Ihrer Organisation teilgenommen haben.</span><span class="sxs-lookup"><span data-stu-id="9362b-107">Get usage trends on the number of unique users and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="9362b-108">Zu den Arten von Konferenzsitzungen gehören Chat, Audio/Video, Anwendungsfreigabe, Web und Einwahl/Auswahl (Drittanbieter).</span><span class="sxs-lookup"><span data-stu-id="9362b-108">Types of conference sessions include IM, audio/video, application sharing, web, and dial-in/out - 3rd party.</span></span>

> <span data-ttu-id="9362b-109">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Konferenzteilnehmeraktivität](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span><span class="sxs-lookup"><span data-stu-id="9362b-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="9362b-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9362b-110">Permissions</span></span>

<span data-ttu-id="9362b-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9362b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9362b-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9362b-113">Permission type</span></span>                        | <span data-ttu-id="9362b-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9362b-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9362b-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9362b-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="9362b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9362b-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9362b-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9362b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9362b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9362b-118">Not supported.</span></span>                           |
| <span data-ttu-id="9362b-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9362b-119">Application</span></span>                            | <span data-ttu-id="9362b-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9362b-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9362b-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9362b-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="9362b-122">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="9362b-122">Function parameters</span></span>

<span data-ttu-id="9362b-123">Geben Sie in der Anforderungs-URL den folgenden Parameter mit einem gültigen Wert an.</span><span class="sxs-lookup"><span data-stu-id="9362b-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="9362b-124">Parameter</span><span class="sxs-lookup"><span data-stu-id="9362b-124">Parameter</span></span> | <span data-ttu-id="9362b-125">Typ</span><span class="sxs-lookup"><span data-stu-id="9362b-125">Type</span></span>   | <span data-ttu-id="9362b-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9362b-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9362b-127">Zeitraum</span><span class="sxs-lookup"><span data-stu-id="9362b-127">period</span></span>    | <span data-ttu-id="9362b-128">string</span><span class="sxs-lookup"><span data-stu-id="9362b-128">string</span></span> | <span data-ttu-id="9362b-129">Gibt die Zeitspanne an, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="9362b-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9362b-130">Die unterstützten Werte für {period_value} sind: D7, D30, D90 und D180.</span><span class="sxs-lookup"><span data-stu-id="9362b-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9362b-131">Diese Werte folgen dem Format D*n*, wobei *n* die Anzahl der Tage angibt, für die der Bericht aggregiert wird.</span><span class="sxs-lookup"><span data-stu-id="9362b-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="9362b-132">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="9362b-132">Required.</span></span> |

<span data-ttu-id="9362b-133">Diese Methode unterstützt die `$format` [OData-Abfragezeichenfolgen-Parameter](/graph/query-parameters) zum Anpassen der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9362b-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="9362b-134">Der Typ der Standardwert ist Text/Csv.</span><span class="sxs-lookup"><span data-stu-id="9362b-134">The default output type is text/csv.</span></span> <span data-ttu-id="9362b-135">Wenn Sie den Ausgabetyp angeben möchten, können Sie auf Text/Csv "oder" Application/Json festgelegt OData $format Abfragezeichenfolgen-Parameter verwenden.</span><span class="sxs-lookup"><span data-stu-id="9362b-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9362b-136">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9362b-136">Request headers</span></span>

| <span data-ttu-id="9362b-137">Name</span><span class="sxs-lookup"><span data-stu-id="9362b-137">Name</span></span>          | <span data-ttu-id="9362b-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9362b-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9362b-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="9362b-139">Authorization</span></span> | <span data-ttu-id="9362b-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9362b-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="9362b-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="9362b-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="9362b-143">CSV</span><span class="sxs-lookup"><span data-stu-id="9362b-143">CSV</span></span>

<span data-ttu-id="9362b-144">Wenn diese Methode erfolgreich ist, wird eine `302 Found`-Antwort zurückgegeben, die zu einer vorauthentifizierten Download-URL für den Bericht umleitet.</span><span class="sxs-lookup"><span data-stu-id="9362b-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9362b-145">Die URL finden Sie in der `Location`-Kopfzeile der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9362b-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9362b-146">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header.</span><span class="sxs-lookup"><span data-stu-id="9362b-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9362b-147">Die CSV-Datei verfügt über die folgenden Kopfzeilen für Spalten.</span><span class="sxs-lookup"><span data-stu-id="9362b-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9362b-148">Berichtsaktualisierungsdatum</span><span class="sxs-lookup"><span data-stu-id="9362b-148">Report Refresh Date</span></span>
- <span data-ttu-id="9362b-149">Berichtsdatum</span><span class="sxs-lookup"><span data-stu-id="9362b-149">Report Date</span></span>
- <span data-ttu-id="9362b-150">Berichtszeitraum</span><span class="sxs-lookup"><span data-stu-id="9362b-150">Report Period</span></span>
- <span data-ttu-id="9362b-151">Chat</span><span class="sxs-lookup"><span data-stu-id="9362b-151">IM</span></span>
- <span data-ttu-id="9362b-152">Audio/Video</span><span class="sxs-lookup"><span data-stu-id="9362b-152">Audio/Video</span></span>
- <span data-ttu-id="9362b-153">Gemeinsame Nutzung von Anwendungen</span><span class="sxs-lookup"><span data-stu-id="9362b-153">App Sharing</span></span>
- <span data-ttu-id="9362b-154">Web</span><span class="sxs-lookup"><span data-stu-id="9362b-154">Web</span></span>
- <span data-ttu-id="9362b-155">Einwahl/Auswahl Drittanbieter</span><span class="sxs-lookup"><span data-stu-id="9362b-155">Dial-in/out 3rd Party</span></span>

### <a name="json"></a><span data-ttu-id="9362b-156">JSON</span><span class="sxs-lookup"><span data-stu-id="9362b-156">JSON</span></span>

<span data-ttu-id="9362b-157">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines **[SkypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md)** -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="9362b-157">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9362b-158">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9362b-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="9362b-159">CSV</span><span class="sxs-lookup"><span data-stu-id="9362b-159">CSV</span></span>

<span data-ttu-id="9362b-160">Es folgt ein Beispiel, das CSV ausgibt.</span><span class="sxs-lookup"><span data-stu-id="9362b-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="9362b-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9362b-161">Request</span></span>

<span data-ttu-id="9362b-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9362b-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="9362b-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="9362b-163">Response</span></span>

<span data-ttu-id="9362b-164">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9362b-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="9362b-165">Führen Sie die Umleitung 302 aus, und die heruntergeladene CSV-Datei besitzt das folgende Format.</span><span class="sxs-lookup"><span data-stu-id="9362b-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party
```

### <a name="json"></a><span data-ttu-id="9362b-166">JSON</span><span class="sxs-lookup"><span data-stu-id="9362b-166">JSON</span></span>

<span data-ttu-id="9362b-167">Es folgt ein Beispiel, das JSON zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9362b-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="9362b-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9362b-168">Request</span></span>

<span data-ttu-id="9362b-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9362b-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="9362b-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="9362b-170">Response</span></span>

<span data-ttu-id="9362b-171">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9362b-171">The following is an example of the response.</span></span>

> <span data-ttu-id="9362b-p109">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="9362b-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 301

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessParticipantActivityUserCounts)", 
  "value": [
    {
      "im": 137, 
      "audioVideo": 196, 
      "appSharing": 214, 
      "web": 30, 
      "dialInOut3rdParty": 2, 
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
