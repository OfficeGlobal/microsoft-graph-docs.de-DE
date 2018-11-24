# <a name="list-apps-in-team"></a><span data-ttu-id="ac874-101">Liste apps im team</span><span class="sxs-lookup"><span data-stu-id="ac874-101">List apps in team</span></span>



<span data-ttu-id="ac874-102">Abrufen der Liste der in das angegebene [Team](../resources/team.md) [apps installiert](../resources/teamsappinstallation.md) .</span><span class="sxs-lookup"><span data-stu-id="ac874-102">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ac874-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ac874-103">Permissions</span></span>

<span data-ttu-id="ac874-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ac874-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ac874-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ac874-106">Permission type</span></span>      | <span data-ttu-id="ac874-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ac874-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac874-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ac874-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ac874-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac874-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ac874-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ac874-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac874-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ac874-111">Not supported.</span></span>    |
|<span data-ttu-id="ac874-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ac874-112">Application</span></span> | <span data-ttu-id="ac874-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ac874-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac874-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ac874-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ac874-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ac874-115">Optional query parameters</span></span>

<span data-ttu-id="ac874-116">Diese Methode unterstützt die $filter $select, und $erweitern [OData-Abfrageparameter](../../../concepts/query_parameters.md) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="ac874-116">This method supports the $filter, $select, and $expand [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac874-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ac874-117">Request headers</span></span>

| <span data-ttu-id="ac874-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ac874-118">Header</span></span>       | <span data-ttu-id="ac874-119">Wert</span><span class="sxs-lookup"><span data-stu-id="ac874-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ac874-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac874-120">Authorization</span></span>  | <span data-ttu-id="ac874-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ac874-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ac874-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ac874-123">Request body</span></span>

<span data-ttu-id="ac874-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ac874-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac874-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="ac874-125">Response</span></span>

<span data-ttu-id="ac874-126">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [TeamsApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="ac874-126">If successful, this method returns a `200 OK` response code and collection of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac874-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ac874-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac874-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ac874-128">Request</span></span>

<span data-ttu-id="ac874-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ac874-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps
```

### <a name="response"></a><span data-ttu-id="ac874-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="ac874-130">Response</span></span>

<span data-ttu-id="ac874-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ac874-131">The following is an example of the response.</span></span>
><span data-ttu-id="ac874-132">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="ac874-132">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ac874-133">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="ac874-133">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

## <a name="example----getting-the-names-of-the-installed-apps"></a><span data-ttu-id="ac874-134">Beispiel: Abrufen der Namen der installierten apps</span><span class="sxs-lookup"><span data-stu-id="ac874-134">Example -- getting the names of the installed apps</span></span>

### <a name="request"></a><span data-ttu-id="ac874-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ac874-135">Request</span></span>

<span data-ttu-id="ac874-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ac874-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps?$expand=teamsAppDefinition
```

### <a name="response"></a><span data-ttu-id="ac874-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="ac874-137">Response</span></span>

<span data-ttu-id="ac874-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ac874-138">The following is an example of the response.</span></span>

><span data-ttu-id="ac874-139">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="ac874-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ac874-140">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="ac874-140">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
    "value": [
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=",
            "teamsAppDefinition": {
                "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
                "teamsAppId": "0d820ecd-def2-4297-adad-78056cde7c78",
                "displayName": "OneNote",
                "version": "1.0.0"
            }
        },
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZmQ5MjVhMC0zNTdmLTRkMjUtODQ1Ni1iMzAyMmFhYTQxYTk=",
            "teamsAppDefinition": {
                "id": "MGZkOTI1YTAtMzU3Zi00ZDI1LTg0NTYtYjMwMjJhYWE0MWE5IyMxLjc=",
                "teamsAppId": "0fd925a0-357f-4d25-8456-b3022aaa41a9",
                "displayName": "SurveyMonkey",
                "version": "1.7"
            }
        },
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMyYTUyNzcwMy0xZjZmLTQ1NTktYTMzMi1kOGE3ZDI4OGNkODg=",
            "teamsAppDefinition": {
                "id": "MmE1Mjc3MDMtMWY2Zi00NTU5LWEzMzItZDhhN2QyODhjZDg4IyMxLjA=",
                "teamsAppId": "2a527703-1f6f-4559-a332-d8a7d288cd88",
                "displayName": "SharePoint",
                "version": "1.0"
            }
        }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->