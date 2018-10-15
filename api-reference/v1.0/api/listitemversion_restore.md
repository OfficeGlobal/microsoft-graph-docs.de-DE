# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="7f87f-101">Frühere Version eines SharePoint-Listenelements wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="7f87f-101">Restore a previous version of a ListItem</span></span>

<span data-ttu-id="7f87f-102">Stellen Sie eine frühere Version eines Listenelements als aktuelle Version wieder her.</span><span class="sxs-lookup"><span data-stu-id="7f87f-102">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="7f87f-103">Dadurch wird eine neue Version mit dem Inhalt der vorherigen Version erstellt, aber alle vorhandenen Versionen des Elements bleiben erhalten.</span><span class="sxs-lookup"><span data-stu-id="7f87f-103">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f87f-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7f87f-104">Permissions</span></span>

<span data-ttu-id="7f87f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7f87f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|            <span data-ttu-id="7f87f-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7f87f-107">Permission type</span></span>             |         <span data-ttu-id="7f87f-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7f87f-108">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="7f87f-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7f87f-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f87f-110">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="7f87f-110">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="7f87f-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7f87f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f87f-112">N/V</span><span class="sxs-lookup"><span data-stu-id="7f87f-112">n/a</span></span>                                                          |
| <span data-ttu-id="7f87f-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7f87f-113">Application</span></span>                            | <span data-ttu-id="7f87f-114">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="7f87f-114">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f87f-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f87f-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="7f87f-116">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7f87f-116">Request body</span></span>

<span data-ttu-id="7f87f-117">Es ist kein Anforderungstexts erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7f87f-117">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="7f87f-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7f87f-118">Example</span></span>

<span data-ttu-id="7f87f-119">In diesem Beispiel wird eine Version eines von `{item-id}` und `{version-id}` identifizierten Listenelements wiederhergestellt.</span><span class="sxs-lookup"><span data-stu-id="7f87f-119">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite sites.readwrite.all", "target": "action", "tags": "service.graph service.sharepoint" } -->

```http
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="7f87f-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f87f-120">Response</span></span>

<span data-ttu-id="7f87f-121">Wenn diese Methode erfolgreich verläuft, gibt der API-Anruf eine `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="7f87f-121">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
