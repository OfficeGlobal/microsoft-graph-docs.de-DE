# <a name="download-contents-of-a-driveitemversion-resource"></a><span data-ttu-id="003e4-101">Inhalt einer DriveItemVersion-Ressource herunterladen (Vorschau)</span><span class="sxs-lookup"><span data-stu-id="003e4-101">Download contents of a DriveItemVersion resource (preview)</span></span>

<span data-ttu-id="003e4-102">Rufen Sie die Inhalte einer bestimmten [DriveItem](../resources/driveitem.md)-Version ab.</span><span class="sxs-lookup"><span data-stu-id="003e4-102">Retrieve the contents of a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="003e4-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="003e4-103">Permissions</span></span>

<span data-ttu-id="003e4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="003e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="003e4-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="003e4-106">Permission type</span></span>      | <span data-ttu-id="003e4-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="003e4-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="003e4-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="003e4-108">Delegated (work or school account)</span></span> | <span data-ttu-id="003e4-109">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="003e4-109">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="003e4-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="003e4-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="003e4-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="003e4-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="003e4-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="003e4-112">Application</span></span> | <span data-ttu-id="003e4-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="003e4-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="003e4-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="003e4-114">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}/content
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}/content
GET /me/drive/items/{item-id}/versions/{version-id}/content
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}/content
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}/content
```

## <a name="response"></a><span data-ttu-id="003e4-115">Antwort</span><span class="sxs-lookup"><span data-stu-id="003e4-115">Response</span></span>

<span data-ttu-id="003e4-116">Die Methode gibt eine Antwort `302 Found` zurück, die auf eine vorab authentifizierte URL zum Download der Bytes der Datei umleitet.</span><span class="sxs-lookup"><span data-stu-id="003e4-116">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the bytes of the file.</span></span>

<span data-ttu-id="003e4-p102">Zum Herunterladen der Inhalte der Datei muss die Anwendung dem `Location`-Header in der Antwort folgen. Viele HTTP-Clientbibliotheken folgen automatisch der 302-Umleitung und beginnen sofort mit dem Download der Datei.</span><span class="sxs-lookup"><span data-stu-id="003e4-p102">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="003e4-119">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header für den Download.</span><span class="sxs-lookup"><span data-stu-id="003e4-119">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

## <a name="example"></a><span data-ttu-id="003e4-120">Beispiel</span><span class="sxs-lookup"><span data-stu-id="003e4-120">Example</span></span>

<span data-ttu-id="003e4-121">In diesem Beispiel wird die Version einer Datei auf dem Laufwerk des aktuellen Benutzers abgerufen.</span><span class="sxs-lookup"><span data-stu-id="003e4-121">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="003e4-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="003e4-122">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-version-contents", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}/content
```

### <a name="response"></a><span data-ttu-id="003e4-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="003e4-123">Response</span></span>

<span data-ttu-id="003e4-124">Diese Methode gibt eine Umleitung zurück, über die der Inhalt der Version heruntergeladen werden kann.</span><span class="sxs-lookup"><span data-stu-id="003e4-124">This returns a redirect to where the contents of the version can be downloaded.</span></span>

<!-- { "blockType": "response", "isEmpty": true  } -->

```http
HTTP/1.1 302 Found
Location: https://onedrive.com/34FF49D6...
```


## <a name="remarks"></a><span data-ttu-id="003e4-125">Hinweise</span><span class="sxs-lookup"><span data-stu-id="003e4-125">Remarks</span></span>

<span data-ttu-id="003e4-126">OneDrive behält nicht die kompletten Metadaten für vorherige Versionen einer Datei bei.</span><span class="sxs-lookup"><span data-stu-id="003e4-126">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="003e4-127">Wenn Ihre App die Liste verfügbarer Versionen für eine Datei abruft, wird eine [DriveItemVersion](../resources/driveItemVersion.md)-Ressource zurückgegeben, welche die verfügbaren Informationen zu der jeweiligen Version bereitstellt.</span><span class="sxs-lookup"><span data-stu-id="003e4-127">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveItemVersion.md) resource is returned that provides the available information about the specific version.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
