# <a name="security-api-error-responses"></a><span data-ttu-id="f1972-101">Sicherheits-API-Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="f1972-101">Security API error responses</span></span>

<span data-ttu-id="f1972-102">Fehler in der Sicherheits-API von Microsoft Graph werden mithilfe der Standard-HTTP-Statuscodes zurückgegeben und über einen Warnungsheader übermittelt.</span><span class="sxs-lookup"><span data-stu-id="f1972-102">Errors in the security API in Microsoft Graph are returned using standard HTTP status codes and are delivered by way of a warning header.</span></span>

<span data-ttu-id="f1972-103">Die Sicherheits-API ist ein Verbunddienst, der von allen Datenanbieter mehrere Antworten empfängt.</span><span class="sxs-lookup"><span data-stu-id="f1972-103">The security API is a federated service that receives multiple responses from all data providers.</span></span> <span data-ttu-id="f1972-104">Wenn ein HTTP-Fehler durch die Sicherheits-API empfangen wird, sendet sie wieder einen Warnungsheader im folgenden Format: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="f1972-104">When an HTTP error is received by the security API, it will send back a warning header in the following format: <!-- { "blockType": "ignored" } --></span></span>

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

<span data-ttu-id="f1972-105">Dieser Warnungsheader wird nur an Clients zurückgesendet, wenn einer der Datenanbieter einen anderen Fehlercode als 2xx oder 404 zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="f1972-105">This warning header is only sent back to clients when one of the data providers returns an error code other than 2xx or 404.</span></span> <span data-ttu-id="f1972-106">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="f1972-106">For example:</span></span>

- <span data-ttu-id="f1972-107">HttpStatusCode.Forbidden (403) könnte zurückgegeben werden, wenn der Zugriff auf die Ressource nicht gewährt wird.</span><span class="sxs-lookup"><span data-stu-id="f1972-107">HttpStatusCode.Forbidden (403) might be returned if the access to the resource is not granted.</span></span>
- <span data-ttu-id="f1972-108">Wenn ein Anbieter ein Zeitlimit überschreitet, wird im Warnungsheader HttpStatusCode.GatewayTimeout (504) zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f1972-108">If a provider times out, HttpStatusCode.GatewayTimeout (504) is returned in the warning header.</span></span>
- <span data-ttu-id="f1972-109">Wenn ein interner Anbieterfehler auftritt, wird im Warnungsheader HttpStatusCode.InternalServerError (500) verwendet.</span><span class="sxs-lookup"><span data-stu-id="f1972-109">If an internal provider error happens, HttpStatusCode.InternalServerError (500) is used in the warning header.</span></span>

<span data-ttu-id="f1972-110">Wenn ein Datenanbieter 2xx oder 404 zurückgibt, wird es nicht im Warnungsheader angezeigt, da diese Codes für den Erfolg erwartet werden oder wenn entsprechend Daten nicht gefunden werden.</span><span class="sxs-lookup"><span data-stu-id="f1972-110">If a data provider returns 2xx or 404, it’s not shown in the warning header because these codes are expected for success or when data is not found respectively.</span></span> <span data-ttu-id="f1972-111">Ein "404 nicht gefunden" wird in einem Verbundsystem so oft erwartet, wie die Daten nur einem oder mehreren, aber nicht allen Anbieter bekannt sind.</span><span class="sxs-lookup"><span data-stu-id="f1972-111">In a federated system, a 404 not found is expected as many times the data is only known to one or several, but not all, providers.</span></span>

## <a name="example"></a><span data-ttu-id="f1972-112">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f1972-112">Example</span></span>

<span data-ttu-id="f1972-113">Ein Benutzer fordert `security/alerts/{alert_id}` an.</span><span class="sxs-lookup"><span data-stu-id="f1972-113">A user asks for `security/alerts/{alert_id}`.</span></span>

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

<span data-ttu-id="f1972-114">Da 404 und 200 erwartete Bedingungen sind, enthält der Warnungsheader Folgendes:</span><span class="sxs-lookup"><span data-stu-id="f1972-114">Because both 404 and 200 are expected conditions, the warning header contains the following:</span></span> 

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/29000",    (usual timeout limit is set at 29 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> <span data-ttu-id="f1972-115">**Hinweis:** Jeder HTTP-Header ist eine Sammlung von Unterelementen, sodass die Benutzer den Warnungsheader aufzählen und alle Elemente überprüfen können.</span><span class="sxs-lookup"><span data-stu-id="f1972-115">**Note:** Each HTTP header is a collection of subitems, so users can enumerate the Warning header and check all items.</span></span>

## <a name="see-also"></a><span data-ttu-id="f1972-116">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="f1972-116">See also</span></span>

<span data-ttu-id="f1972-117">Wenn Probleme bei der Autorisierung auftreten, beziehen Sie sich auf unseren [Blogbeitrag](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2).</span><span class="sxs-lookup"><span data-stu-id="f1972-117">If you’re having trouble with authorization, see our [blog post](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2).</span></span>
