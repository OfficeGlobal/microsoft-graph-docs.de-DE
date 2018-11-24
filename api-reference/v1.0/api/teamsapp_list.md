# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="9ac75-101">Liste der veröffentlichten apps aus dem Microsoft-Teams, app-Katalog</span><span class="sxs-lookup"><span data-stu-id="9ac75-101">List the published apps from the Microsoft Teams app catalog</span></span>



<span data-ttu-id="9ac75-102">Liste der [apps](../resources/teamsapp.md) aus dem Microsoft-Teams, app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="9ac75-102">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span> <span data-ttu-id="9ac75-103">Dazu gehören apps aus dem Microsoft-Teams Store als auch apps aus Ihrer Organisation app-Katalog (die Mandanten-app-Katalog).</span><span class="sxs-lookup"><span data-stu-id="9ac75-103">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="9ac75-104">Wenn Sie apps aus app-Katalog nur Ihrer Organisation erhalten möchten, geben Sie `Organization` als die **DistributionMethod** in der [TeamsCatalogApp](../resources/teamsapp.md) -Ressource.</span><span class="sxs-lookup"><span data-stu-id="9ac75-104">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ac75-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9ac75-105">Permissions</span></span>

<span data-ttu-id="9ac75-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="9ac75-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="9ac75-108">**Hinweis:** Nur globale Administratoren können diese API aufrufen.</span><span class="sxs-lookup"><span data-stu-id="9ac75-108">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="9ac75-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9ac75-109">Permission Type</span></span>                        | <span data-ttu-id="9ac75-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9ac75-110">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="9ac75-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9ac75-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ac75-112">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ac75-112">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="9ac75-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9ac75-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ac75-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ac75-114">Not supported</span></span>|
| <span data-ttu-id="9ac75-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9ac75-115">Application</span></span>                            | <span data-ttu-id="9ac75-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ac75-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ac75-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ac75-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9ac75-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9ac75-118">Optional query parameters</span></span>
<span data-ttu-id="9ac75-119">Diese Methode unterstützt die $filter $select, und $erweitern [OData-Abfrageparameter](../../../concepts/query_parameters.md) helfen, die Antwort anzupassen.</span><span class="sxs-lookup"><span data-stu-id="9ac75-119">This method supports the $filter, $select, and $expand [OData query parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ac75-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9ac75-120">Request headers</span></span>

| <span data-ttu-id="9ac75-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9ac75-121">Header</span></span>        | <span data-ttu-id="9ac75-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9ac75-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="9ac75-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ac75-123">Authorization</span></span> | <span data-ttu-id="9ac75-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9ac75-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9ac75-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9ac75-126">Request body</span></span>
<span data-ttu-id="9ac75-127">Keine.</span><span class="sxs-lookup"><span data-stu-id="9ac75-127">None.</span></span>

><span data-ttu-id="9ac75-128">**Hinweis:** Sie können die Felder des [TeamsCatalogApp](../resources/teamsapp.md) -Objekts in der Ergebnisliste verkürzte filtern.</span><span class="sxs-lookup"><span data-stu-id="9ac75-128">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="9ac75-129">Sie können eine der folgenden Filter Vorgänge verwenden: gleich, nicht gleich, und, oder, und nicht.</span><span class="sxs-lookup"><span data-stu-id="9ac75-129">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="9ac75-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ac75-130">Response</span></span>
<span data-ttu-id="9ac75-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Liste von Objekten im Antworttext [TeamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="9ac75-131">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9ac75-132">Beispiele</span><span class="sxs-lookup"><span data-stu-id="9ac75-132">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="9ac75-133">Beispiel 1</span><span class="sxs-lookup"><span data-stu-id="9ac75-133">Example 1</span></span>
<span data-ttu-id="9ac75-134">Das folgende Beispiel listet alle Anwendungen, die für Ihre Mandanten spezifisch sind.</span><span class="sxs-lookup"><span data-stu-id="9ac75-134">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="9ac75-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ac75-135">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

#### <a name="response"></a><span data-ttu-id="9ac75-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ac75-136">Response</span></span>
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

### <a name="example-2"></a><span data-ttu-id="9ac75-137">Beispiel 2</span><span class="sxs-lookup"><span data-stu-id="9ac75-137">Example 2</span></span>

<span data-ttu-id="9ac75-138">Das folgende Beispiel listet Applikationen mit einer bestimmten ID.</span><span class="sxs-lookup"><span data-stu-id="9ac75-138">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="9ac75-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ac75-139">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="9ac75-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ac75-140">Response</span></span>
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

