# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="30e96-101">Aktualisieren von apps in Ihrer Organisation app-Katalog veröffentlicht</span><span class="sxs-lookup"><span data-stu-id="30e96-101">Update apps published to your organization's app catalog</span></span>



<span data-ttu-id="30e96-102">Aktualisieren einer [app](../resources/teamsapp.md) veröffentlicht zuvor in der Microsoft-Teams, app-Katalog.</span><span class="sxs-lookup"><span data-stu-id="30e96-102">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="30e96-103">Diese API aktualisiert speziell eine app in Ihrer Organisation app-Katalog (die Mandanten-app-Katalog) veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="30e96-103">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="30e96-104">Geben Sie zum Veröffentlichen in Ihrer Organisation app-Katalog `organization` als die **DistributionMethod** in der [TeamsCatalogApp](../resources/teamsapp.md) -Ressource.</span><span class="sxs-lookup"><span data-stu-id="30e96-104">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="30e96-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="30e96-105">Permissions</span></span>

<span data-ttu-id="30e96-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="30e96-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="30e96-108">**Hinweis:** Nur globale Administratoren können diese API aufrufen.</span><span class="sxs-lookup"><span data-stu-id="30e96-108">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="30e96-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="30e96-109">Permission Type</span></span>                        | <span data-ttu-id="30e96-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="30e96-110">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="30e96-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="30e96-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="30e96-112">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30e96-112">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="30e96-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="30e96-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30e96-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="30e96-114">Not supported</span></span>|
| <span data-ttu-id="30e96-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="30e96-115">Application</span></span>                            | <span data-ttu-id="30e96-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="30e96-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="30e96-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="30e96-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="30e96-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="30e96-118">Request headers</span></span>

| <span data-ttu-id="30e96-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="30e96-119">Header</span></span>        | <span data-ttu-id="30e96-120">Wert</span><span class="sxs-lookup"><span data-stu-id="30e96-120">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="30e96-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="30e96-121">Authorization</span></span> | <span data-ttu-id="30e96-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="30e96-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="30e96-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="30e96-124">Content-Type</span></span>  | <span data-ttu-id="30e96-125">Anwendung/zip</span><span class="sxs-lookup"><span data-stu-id="30e96-125">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="30e96-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="30e96-126">Request body</span></span>

<span data-ttu-id="30e96-127">Manifest Teams Zip-Nutzlast: Für Teams Anwendung zip-Datei [Erstellen eines app-Pakets finden Sie unter](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="30e96-127">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="30e96-128">**Hinweis:** Verwenden Sie die ID aus der [Liste apps veröffentlicht](./teamsapp_list.md) Aufruf für zurückgegeben, auf um die app zu verweisen, die Sie aktualisieren möchten.</span><span class="sxs-lookup"><span data-stu-id="30e96-128">**Note:** Use the ID returned from the [List published apps](./teamsapp_list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="30e96-129">Verwenden Sie nicht die in der Manifestdatei der app Zip-Paket-ID ein.</span><span class="sxs-lookup"><span data-stu-id="30e96-129">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="30e96-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="30e96-130">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="30e96-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="30e96-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="30e96-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="30e96-132">Request</span></span>

```
PUT https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="30e96-133">Für Teams Anwendung zip-Datei [finden Sie unter Erstellen von app-Paket](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="30e96-133">For Teams application zip file [see Create app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="30e96-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="30e96-134">Response</span></span>

```
HTTP/1.1 204 No Content
```
