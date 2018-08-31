# <a name="restore-a-previous-version-of-a-driveitem"></a><span data-ttu-id="62f96-101">Frühere Version eines DriveItem wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="62f96-101">Restore a previous version of a DriveItem</span></span>

<span data-ttu-id="62f96-102">Stellen Sie eine frühere Version eines DriveItem als aktuelle Version wieder her.</span><span class="sxs-lookup"><span data-stu-id="62f96-102">Restore a previous version of a DriveItem to be the current version.</span></span> <span data-ttu-id="62f96-103">Dadurch wird eine neue Version mit dem Inhalt der vorherigen Version erstellt, aber alle vorhandenen Versionen der Datei bleibt erhalten.</span><span class="sxs-lookup"><span data-stu-id="62f96-103">This will create a new version with the contents of the previous version, but preserves all existing versions of the file.</span></span>

## <a name="permissions"></a><span data-ttu-id="62f96-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="62f96-104">Permissions</span></span>

<span data-ttu-id="62f96-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="62f96-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="62f96-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="62f96-107">Permission type</span></span>      | <span data-ttu-id="62f96-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="62f96-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62f96-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="62f96-109">Delegated (work or school account)</span></span> | <span data-ttu-id="62f96-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62f96-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="62f96-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="62f96-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62f96-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62f96-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="62f96-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="62f96-113">Application</span></span> | <span data-ttu-id="62f96-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62f96-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62f96-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="62f96-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/versions/{version-id}/restoreVersion
POST /groups/{groupId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /me/drive/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{siteId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
POST /users/{userId}/drive/items/{itemId}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="62f96-116">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="62f96-116">Request body</span></span>

<span data-ttu-id="62f96-117">Es ist kein Anforderungstexts erforderlich.</span><span class="sxs-lookup"><span data-stu-id="62f96-117">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="62f96-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="62f96-118">Example</span></span>

<span data-ttu-id="62f96-119">In diesem Beispiel wird eine Version einer von `{item-id}` und `{version-id}` identifizierten Datei wiederhergestellt.</span><span class="sxs-lookup"><span data-stu-id="62f96-119">This example restores a version of a file identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="62f96-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="62f96-120">Response</span></span>

<span data-ttu-id="62f96-121">Wenn diese Methode erfolgreich verläuft, gibt der API-Anruf eine `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="62f96-121">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
