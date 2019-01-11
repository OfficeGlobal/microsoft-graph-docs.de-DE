---
title: Microsoft Graph Sicherheit API Fehlerantworten
description: Fehler in der Microsoft Graph Sicherheit API werden mithilfe des standard 206 teilweise von HTTP-Statuscodes zurückgegeben und über eine Warnung Header übermittelt werden.
author: Preetikr
localization_priority: Normal
ms.openlocfilehash: 16a7153f460b57a74901b0d5c48bdd9004e06bc4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878624"
---
# <a name="microsoft-graph-security-api-error-responses"></a><span data-ttu-id="30d40-103">Microsoft Graph Sicherheit API Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="30d40-103">Microsoft Graph Security API error responses</span></span>

<span data-ttu-id="30d40-104">Fehler in der Microsoft Graph Sicherheit API werden mithilfe des standard 206 teilweise von HTTP-Statuscodes zurückgegeben und über eine Warnung Header übermittelt werden.</span><span class="sxs-lookup"><span data-stu-id="30d40-104">Errors in the Microsoft Graph Security API are returned using the standard HTTP 206 Partial Content status code and are delivered via a warning header.</span></span>

## <a name="errors"></a><span data-ttu-id="30d40-105">Fehler</span><span class="sxs-lookup"><span data-stu-id="30d40-105">Errors</span></span>

<span data-ttu-id="30d40-106">Sicherheit-API von Microsoft Graph ist ein Verbundpartner Dienst, der von allen Datenanbieter mehrere Antworten empfängt.</span><span class="sxs-lookup"><span data-stu-id="30d40-106">The Microsoft Graph Security API is a federated service that receives multiple responses from all data providers.</span></span> <span data-ttu-id="30d40-107">Wenn ein HTTP-Fehler durch die Microsoft Graph Sicherheit API empfangen wird, sendet er wieder eine Warnung Kopfzeile im folgenden Format:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="30d40-107">When an HTTP error is received by the Microsoft Graph Security API, it will send back a warning header in the following format: <!-- { "blockType": "ignored" } --></span></span>

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

<span data-ttu-id="30d40-108">Diese Warnung Kopfzeile ist nur an Clients gesendet, wenn-Datenanbieter einen Fehlercode als 2xx oder 404 zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="30d40-108">This warning header is only sent back to clients when one of the data providers returns an error code other than 2xx or 404.</span></span> <span data-ttu-id="30d40-109">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="30d40-109">For example:</span></span>

- <span data-ttu-id="30d40-110">HttpStatusCode.Forbidden (403) könnte zurückgegeben werden, wenn der Zugriff auf die Ressource nicht gewährt wird.</span><span class="sxs-lookup"><span data-stu-id="30d40-110">HttpStatusCode.Forbidden (403) might be returned if the access to the resource is not granted.</span></span>
- <span data-ttu-id="30d40-111">Wenn ein Anbieter ist ein Timeout aufgetreten, wird in der Kopfzeile Warnung HttpStatusCode.GatewayTimeout (504) zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="30d40-111">If a provider times out, HttpStatusCode.GatewayTimeout (504) is returned in the warning header.</span></span>
- <span data-ttu-id="30d40-112">Wenn ein für internen Anbieterfehler auftritt, wird HttpStatusCode.InternalServerError (500) in der Kopfzeile Warnung verwendet.</span><span class="sxs-lookup"><span data-stu-id="30d40-112">If an internal provider error happens, HttpStatusCode.InternalServerError (500) is used in the warning header.</span></span>

<span data-ttu-id="30d40-113">Wenn ein Datenanbieters 2xx oder 404 zurückgibt, wird er nicht in der Kopfzeile Warnung angezeigt, da diese Codes für den Erfolg erwartet werden oder wenn Daten jeweils nicht gefunden werden kann.</span><span class="sxs-lookup"><span data-stu-id="30d40-113">If a data provider returns 2xx or 404, it’s not shown in the warning header because these codes are expected for success or when data is not found respectively.</span></span> <span data-ttu-id="30d40-114">Eine 404 nicht gefunden wird in einem Verbundpartner System erwartet, wie oft die Daten nur ein oder mehrere, aber nicht alle Anbieter bekannt ist.</span><span class="sxs-lookup"><span data-stu-id="30d40-114">In a federated system, a 404 not found is expected as many times the data is only known to one or several, but not all, providers.</span></span>

## <a name="example"></a><span data-ttu-id="30d40-115">Beispiel</span><span class="sxs-lookup"><span data-stu-id="30d40-115">Example</span></span>

<span data-ttu-id="30d40-116">Ein Benutzer fordert `security/alerts/{alert_id}`.</span><span class="sxs-lookup"><span data-stu-id="30d40-116">A user asks for `security/alerts/{alert_id}`.</span></span>

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

<span data-ttu-id="30d40-117">Da 404 und 200 erwartete Bedingungen sind, enthält die Warnung Kopfzeile Folgendes:</span><span class="sxs-lookup"><span data-stu-id="30d40-117">Because both 404 and 200 are expected conditions, the warning header contains the following:</span></span>

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> <span data-ttu-id="30d40-118">**Hinweis:** Jede HTTP-Header ist eine Auflistung von Unterelemente, sodass Benutzer die Warnung Kopfzeile auflisten und alle Elemente überprüfen können.</span><span class="sxs-lookup"><span data-stu-id="30d40-118">**Note:** Each HTTP header is a collection of subitems, so users can enumerate the Warning header and check all items.</span></span>

## <a name="constraints"></a><span data-ttu-id="30d40-119">Einschränkungen</span><span class="sxs-lookup"><span data-stu-id="30d40-119">Constraints</span></span>

<span data-ttu-id="30d40-120">Die `$top` OData-Abfragezeichenfolgen-Parameter kann maximal 1000 Warnungen und eine Kombination von `$top`  +  `$skip` OData-Abfrage-Parameter können nicht überschreiten 6000 Warnungen.</span><span class="sxs-lookup"><span data-stu-id="30d40-120">The `$top` OData query parameter has a limit of 1000 alerts, and a combination of `$top` + `$skip` OData query parameters cannot exceed 6000 alerts.</span></span> <span data-ttu-id="30d40-121">Beispielsweise `/security/alerts?$top=10&$skip=5990` zurückgegebenen eine `200 OK` Antwortcode, aber `/security/alerts?$top=10&$skip=5991` zurückgegebenen eine `400 Bad Request` Antwortcode.</span><span class="sxs-lookup"><span data-stu-id="30d40-121">For example, `/security/alerts?$top=10&$skip=5990` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=5991` will return a `400 Bad Request` response code.</span></span>

<span data-ttu-id="30d40-122">Eine Umgehung für diese Grenze ist die Verwendung der `$filter` OData-Abfragezeichenfolgen-Parameter mit der `eventDateTime` der Warnung Entität aus der Microsoft Graph-Security-API mit `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` , und ersetzen den DateTime-Wert durch die letzte Benachrichtigung (6000th).</span><span class="sxs-lookup"><span data-stu-id="30d40-122">A work-around for this limit is to use the `$filter` OData query parameter with the `eventDateTime` of the alert entity from the Microsoft Graph Security API, using `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` and replacing the dateTime value with the last (6000th) alert.</span></span> <span data-ttu-id="30d40-123">Sie können auch festlegen, einen Bereich für die `eventDateTime`; beispielsweise *Alerts?$ Filter = Ereignisdatum/-Uhrzeit **Gt** 2018-11 -**11**T00:00:00.000Z & Ereignisdatum/-Uhrzeit **Lt** 2018-11 -**12**T00:00:00.000Z*</span><span class="sxs-lookup"><span data-stu-id="30d40-123">You can also set a range for the `eventDateTime`; for example, *alerts?$filter=eventDateTime **gt** 2018-11-**11**T00:00:00.000Z&eventDateTime **lt** 2018-11-**12**T00:00:00.000Z*</span></span>

## <a name="see-also"></a><span data-ttu-id="30d40-124">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="30d40-124">See also</span></span>

<span data-ttu-id="30d40-125">Wenn Sie Probleme mit Autorisierung haben, finden Sie unter [Authorization and Security-API von Microsoft Graph](/graph/security-authorization).</span><span class="sxs-lookup"><span data-stu-id="30d40-125">If you’re having trouble with authorization, see [Authorization and the Microsoft Graph Security API](/graph/security-authorization).</span></span>
