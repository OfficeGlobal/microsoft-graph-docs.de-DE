# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="62914-101">Entfernen einer app aus Ihrer Organisation app-Katalog</span><span class="sxs-lookup"><span data-stu-id="62914-101">Remove an app from your organization's app catalog</span></span>



<span data-ttu-id="62914-102">Entfernen Sie die [app](../resources/teamsapp.md) aus Ihrer Organisation app-Katalog (die Mandanten-app-Katalog).</span><span class="sxs-lookup"><span data-stu-id="62914-102">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="62914-103">Wenn Ihre app aus Ihrer Organisation app-Katalog entfernen möchten, geben Sie `organization` als die **DistributionMethod** in der [TeamsCatalogApp](../resources/teamsapp.md) -Ressource.</span><span class="sxs-lookup"><span data-stu-id="62914-103">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="62914-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="62914-104">Permissions</span></span>

<span data-ttu-id="62914-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="62914-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="62914-107">**Hinweis:** Nur globale Administratoren können diese API aufrufen.</span><span class="sxs-lookup"><span data-stu-id="62914-107">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="62914-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="62914-108">Permission Type</span></span>                        | <span data-ttu-id="62914-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="62914-109">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="62914-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="62914-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="62914-111">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62914-111">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="62914-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="62914-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62914-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="62914-113">Not supported</span></span>|
| <span data-ttu-id="62914-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="62914-114">Application</span></span>                            | <span data-ttu-id="62914-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="62914-115">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="62914-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="62914-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="62914-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="62914-117">Request headers</span></span>

| <span data-ttu-id="62914-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="62914-118">Header</span></span>        | <span data-ttu-id="62914-119">Wert</span><span class="sxs-lookup"><span data-stu-id="62914-119">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="62914-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="62914-120">Authorization</span></span> | <span data-ttu-id="62914-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="62914-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="62914-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="62914-123">Request body</span></span>

<span data-ttu-id="62914-124">Keine.</span><span class="sxs-lookup"><span data-stu-id="62914-124">None.</span></span>

><span data-ttu-id="62914-125">**Hinweis:** Verwenden Sie die ID aus der [Liste apps veröffentlicht](./teamsapp_list.md) Aufruf für zurückgegeben, auf um die app zu verweisen, die Sie aktualisieren möchten.</span><span class="sxs-lookup"><span data-stu-id="62914-125">**Note:** Use the ID returned from the [List published apps](./teamsapp_list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="62914-126">Verwenden Sie nicht die in der Manifestdatei der app Zip-Paket-ID ein.</span><span class="sxs-lookup"><span data-stu-id="62914-126">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="62914-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="62914-127">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="62914-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="62914-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="62914-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="62914-129">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="62914-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="62914-130">Response</span></span>

```http
HTTP/1.1 204 No Content
```
