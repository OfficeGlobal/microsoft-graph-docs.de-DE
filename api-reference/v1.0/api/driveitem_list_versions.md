# <a name="listing-versions-of-a-driveitem"></a><span data-ttu-id="f1789-101">Listing von Versionen einer DriveItem</span><span class="sxs-lookup"><span data-stu-id="f1789-101">Listing versions of a DriveItem (preview)</span></span>

<span data-ttu-id="f1789-102">OneDrive und SharePoint können auch so konfiguriert werden, dass für Dateien ein Verlauf beibehalten wird.</span><span class="sxs-lookup"><span data-stu-id="f1789-102">OneDrive and SharePoint can be configured to retain the history for files.</span></span>
<span data-ttu-id="f1789-103">Je nach Dienst und Konfiguration kann für jede Änderung beim Speichern der Datei eine neue Version erstellt werden, manuell oder nie.</span><span class="sxs-lookup"><span data-stu-id="f1789-103">Depending on the service and configuration, a new version can be created for each edit, each time the file is saved, manually, or never.</span></span>

<span data-ttu-id="f1789-104">Vorherige Versionen eines Dokuments können je nach Administratoreinstellungen für einen begrenzten Zeitraum beibehalten werden, diese können pro Benutzer oder Speicherort eindeutig sein.</span><span class="sxs-lookup"><span data-stu-id="f1789-104">Previous versions of a document may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1789-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f1789-105">Permissions</span></span>

<span data-ttu-id="f1789-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f1789-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f1789-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f1789-108">Permission type</span></span>      | <span data-ttu-id="f1789-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f1789-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1789-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f1789-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f1789-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1789-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f1789-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f1789-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1789-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1789-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f1789-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f1789-114">Application</span></span> | <span data-ttu-id="f1789-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1789-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="f1789-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1789-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions
GET /groups/{group-id}/drive/{item-id}/versions
GET /me/drive/items/{item-id}/versions
GET /sites/{site-id}/drive/items/{item-id}/versions
GET /users/{user-id}/drive/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="f1789-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1789-117">Response</span></span>

<span data-ttu-id="f1789-118">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [DriveItemVersion](../resources/driveitemversion.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f1789-118">If successful, this method returns a `200 OK` response code and collection of [DriveItemVersion](../resources/driveitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="f1789-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f1789-119">Example</span></span>

<span data-ttu-id="f1789-120">In diesem Beispiel werden die Versionen einer Datei auf dem Laufwerk des aktuellen Benutzers abgerufen.</span><span class="sxs-lookup"><span data-stu-id="f1789-120">This example retrieves the versions of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="f1789-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1789-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="f1789-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1789-122">Response</span></span>

<span data-ttu-id="f1789-123">Dadurch wird eine Sammlung von Versionen zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="f1789-123">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItemVersion)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value":
  [
    {
      "id": "3.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
      "size": 123
    },
    {
      "id": "2.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-11T10:21:03.000Z",
      "size": 62
    },
    {
      "id": "1.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-10T15:20:01.125Z",
      "size": 16
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="f1789-124">Hinweise</span><span class="sxs-lookup"><span data-stu-id="f1789-124">Remarks</span></span>

<span data-ttu-id="f1789-125">OneDrive behält nicht die kompletten Metadaten für vorherige Versionen einer Datei bei.</span><span class="sxs-lookup"><span data-stu-id="f1789-125">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="f1789-126">Wenn Ihre App die Liste verfügbarer Versionen für eine Datei abruft, wird eine [DriveItemVersion](../resources/driveItemVersion.md)-Ressource zurückgegeben, welche die verfügbaren Informationen zu der jeweiligen Version bereitstellt.</span><span class="sxs-lookup"><span data-stu-id="f1789-126">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveItemVersion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
