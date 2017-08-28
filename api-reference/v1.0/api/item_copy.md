# <a name="copy-a-driveitem"></a><span data-ttu-id="b925d-101">DriveItem kopieren</span><span class="sxs-lookup"><span data-stu-id="b925d-101">Copy a DriveItem</span></span>

<span data-ttu-id="b925d-102">Mit dieser API können Sie eine Kopie einer Ressource des Typs [driveItem](../resources/driveitem.md) (einschließlich aller untergeordneten Elemente) unter einem neuen übergeordneten Element oder mit einem neuen Namen erstellen.</span><span class="sxs-lookup"><span data-stu-id="b925d-102">Creates a copy of a [driveItem](../resources/driveitem.md) (including any children) under a new parent or with a new name.</span></span>

## <a name="permissions"></a><span data-ttu-id="b925d-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b925d-103">Permissions</span></span>
<span data-ttu-id="b925d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b925d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b925d-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b925d-106">Permission type</span></span>      | <span data-ttu-id="b925d-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b925d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b925d-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b925d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b925d-109">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b925d-109">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b925d-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b925d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b925d-111">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b925d-111">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b925d-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b925d-112">Application</span></span> | <span data-ttu-id="b925d-113">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b925d-113">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b925d-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b925d-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```
POST /me/drive/items/{item-id}/copy
POST /me/drive/root:/{path}:/copy
POST /groups/{group-id}/drive/items/{item-id}/copy
```

## <a name="request-body"></a><span data-ttu-id="b925d-115">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b925d-115">Request body</span></span>
<span data-ttu-id="b925d-116">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="b925d-116">In the request body, provide a JSON object with the following parameters.</span></span>


| <span data-ttu-id="b925d-117">Name</span><span class="sxs-lookup"><span data-stu-id="b925d-117">Name</span></span>            | <span data-ttu-id="b925d-118">Wert</span><span class="sxs-lookup"><span data-stu-id="b925d-118">Value</span></span>                                          | <span data-ttu-id="b925d-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b925d-119">Description</span></span>                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b925d-120">parentReference</span><span class="sxs-lookup"><span data-stu-id="b925d-120">parentReference</span></span> | [<span data-ttu-id="b925d-121">ItemReference</span><span class="sxs-lookup"><span data-stu-id="b925d-121">ItemReference</span></span>](../resources/itemreference.md) | <span data-ttu-id="b925d-p102">Optional.  Verweis auf das übergeordnete Element, in dem die Kopie erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="b925d-p102">Optional. Reference to the parent item the copy will be created in.</span></span>                                         |
| <span data-ttu-id="b925d-124">name</span><span class="sxs-lookup"><span data-stu-id="b925d-124">name</span></span>            | <span data-ttu-id="b925d-125">string</span><span class="sxs-lookup"><span data-stu-id="b925d-125">string</span></span>                                         | <span data-ttu-id="b925d-p103">Optional.  Der neue Name der Kopie. Wenn dieser nicht angegeben wird, wird der gleiche Namen wie für das Original verwendet.</span><span class="sxs-lookup"><span data-stu-id="b925d-p103">Optional. The new name for the copy. If this isn't provided, the same name will be used as the original.</span></span>    |

<span data-ttu-id="b925d-p104">**Hinweis:** Das _parentReference_-Element sollte entweder ein `id`- oder `path`-Element enthalten, jedoch nicht beides. Wenn beide enthalten sind, müssen sie auf das gleiche Element verweisen, andernfalls tritt ein Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="b925d-p104">**Note:** The _parentReference_ should include either an `id` or `path` but not both. If both are included, they need to reference the same item or an error will occur.</span></span>

## <a name="example"></a><span data-ttu-id="b925d-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b925d-131">Example</span></span>

<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "path": "/drive/root:/Documents"
  },
  "name": "contoso plan.docx"
}
```

## <a name="response"></a><span data-ttu-id="b925d-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="b925d-132">Response</span></span>

<span data-ttu-id="b925d-133">Gibt detaillierte Informationen zum Überwachen des Status der Kopie,bis die Anforderung akzeptiert wird.</span><span class="sxs-lookup"><span data-stu-id="b925d-133">Returns details about how to monitor the progress of the copy, upon accepting the request.</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 202 Accepted
```

## <a name="remarks"></a><span data-ttu-id="b925d-134">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="b925d-134">Remarks</span></span>

<span data-ttu-id="b925d-p105">In vielen Fällen wird die Aktion zum Kopieren asynchron durchgeführt. Die Antwort der API gibt nur an, dass der Kopiervorgang akzeptiert oder abgelehnt wurde, wenn der Zieldateiname zum Beispiel bereits verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="b925d-p105">In many cases the copy action is performed asynchronously. The response from the API will only indicate that the copy operation was accepted or rejected, say due to the destination filename already being in use.</span></span>

<span data-ttu-id="b925d-137">**Hinweis:** Die API stellt keine Methode zum Abrufen von Informationen dazu bereit, ob die Kopie erfolgreich war.</span><span class="sxs-lookup"><span data-stu-id="b925d-137">**Note:** The API does not provide a method to know if the copy was successful.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Copy"
} -->
