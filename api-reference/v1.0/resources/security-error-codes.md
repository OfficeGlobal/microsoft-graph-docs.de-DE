---
title: Microsoft Graph Sicherheit API Fehlerantworten
description: Fehler in der Microsoft Graph Security-API in Microsoft Graph werden mithilfe der standard-HTTP-206 teilweise Content Statuscode zurückgegeben und über eine Warnung Kopfzeile übermittelt werden.
ms.openlocfilehash: 35af0a1ed4c4bf7f6e1afb36039f812ab59f64dd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019824"
---
# <a name="microsoft-graph-security-api-error-responses"></a><span data-ttu-id="0b568-103">Microsoft Graph Sicherheit API Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="0b568-103">Microsoft Graph Security API error responses</span></span>

<span data-ttu-id="0b568-104">Fehler in der Microsoft Graph Security-API in Microsoft Graph werden mithilfe der standard-HTTP-206 teilweise Content Statuscode zurückgegeben und über eine Warnung Kopfzeile übermittelt werden.</span><span class="sxs-lookup"><span data-stu-id="0b568-104">Errors in the Microsoft Graph Security API in Microsoft Graph are returned using standard HTTP 206 Partial Content status code and are delivered by way of a warning header.</span></span>

<span data-ttu-id="0b568-105">Sicherheit-API von Microsoft Graph ist ein Verbundpartner Dienst, der von allen Datenanbieter mehrere Antworten empfängt.</span><span class="sxs-lookup"><span data-stu-id="0b568-105">The Microsoft Graph Security API is a federated service that receives multiple responses from all data providers.</span></span> <span data-ttu-id="0b568-106">Wenn ein HTTP-Fehler durch die Microsoft Graph Sicherheit API empfangen wird, sendet er wieder eine Warnung Kopfzeile im folgenden Format:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="0b568-106">When an HTTP error is received by the Microsoft Graph Security API, it will send back a warning header in the following format: <!-- { "blockType": "ignored" } --></span></span>

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

<span data-ttu-id="0b568-107">Diese Warnung Kopfzeile ist nur an Clients gesendet, wenn-Datenanbieter einen Fehlercode als 2xx oder 404 zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="0b568-107">This warning header is only sent back to clients when one of the data providers returns an error code other than 2xx or 404.</span></span> <span data-ttu-id="0b568-108">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="0b568-108">For example:</span></span>

- <span data-ttu-id="0b568-109">HttpStatusCode.Forbidden (403) könnte zurückgegeben werden, wenn der Zugriff auf die Ressource nicht gewährt wird.</span><span class="sxs-lookup"><span data-stu-id="0b568-109">HttpStatusCode.Forbidden (403) might be returned if the access to the resource is not granted.</span></span>
- <span data-ttu-id="0b568-110">Wenn ein Anbieter ist ein Timeout aufgetreten, wird in der Kopfzeile Warnung HttpStatusCode.GatewayTimeout (504) zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0b568-110">If a provider times out, HttpStatusCode.GatewayTimeout (504) is returned in the warning header.</span></span>
- <span data-ttu-id="0b568-111">Wenn ein für internen Anbieterfehler auftritt, wird HttpStatusCode.InternalServerError (500) in der Kopfzeile Warnung verwendet.</span><span class="sxs-lookup"><span data-stu-id="0b568-111">If an internal provider error happens, HttpStatusCode.InternalServerError (500) is used in the warning header.</span></span>

<span data-ttu-id="0b568-112">Wenn ein Datenanbieters 2xx oder 404 zurückgibt, wird er nicht in der Kopfzeile Warnung angezeigt, da diese Codes für den Erfolg erwartet werden oder wenn Daten jeweils nicht gefunden werden kann.</span><span class="sxs-lookup"><span data-stu-id="0b568-112">If a data provider returns 2xx or 404, it’s not shown in the warning header because these codes are expected for success or when data is not found respectively.</span></span> <span data-ttu-id="0b568-113">Eine 404 nicht gefunden wird in einem Verbundpartner System erwartet, wie oft die Daten nur ein oder mehrere, aber nicht alle Anbieter bekannt ist.</span><span class="sxs-lookup"><span data-stu-id="0b568-113">In a federated system, a 404 not found is expected as many times the data is only known to one or several, but not all, providers.</span></span>

## <a name="example"></a><span data-ttu-id="0b568-114">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0b568-114">Example</span></span>

<span data-ttu-id="0b568-115">Ein Benutzer fordert `security/alerts/{alert_id}`.</span><span class="sxs-lookup"><span data-stu-id="0b568-115">A user asks for `security/alerts/{alert_id}`.</span></span>

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

<span data-ttu-id="0b568-116">Da 404 und 200 erwartete Bedingungen sind, enthält die Warnung Kopfzeile Folgendes:</span><span class="sxs-lookup"><span data-stu-id="0b568-116">Because both 404 and 200 are expected conditions, the warning header contains the following:</span></span> 

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> <span data-ttu-id="0b568-117">**Hinweis:** Jede HTTP-Header ist eine Auflistung von Unterelemente, sodass Benutzer die Warnung Kopfzeile auflisten und alle Elemente überprüfen können.</span><span class="sxs-lookup"><span data-stu-id="0b568-117">**Note:** Each HTTP header is a collection of subitems, so users can enumerate the Warning header and check all items.</span></span>

## <a name="see-also"></a><span data-ttu-id="0b568-118">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="0b568-118">See also</span></span>

<span data-ttu-id="0b568-119">Wenn Sie Probleme mit Autorisierung haben, finden Sie in unserem [Blog veröffentlichen](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2).</span><span class="sxs-lookup"><span data-stu-id="0b568-119">If you’re having trouble with authorization, see our [blog post](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2).</span></span>
