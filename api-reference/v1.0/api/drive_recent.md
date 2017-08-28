# <a name="list-recent-files"></a><span data-ttu-id="113a6-101">Zuletzt verwendete Dateien auflisten</span><span class="sxs-lookup"><span data-stu-id="113a6-101">List recent files</span></span>

<span data-ttu-id="113a6-p101">Dient zum Auflisten eines Satzes von Elementen, die zuletzt von dem angemeldeten Benutzer verwendet wurden. Diese Sammlung enthält Elemente, die sich in dem Laufwerk des Benutzers befinden sowie Elemente in anderen Laufwerken, auf die dieser Zugriff hat.</span><span class="sxs-lookup"><span data-stu-id="113a6-p101">List a set of items that have been recently used by the signed in user. This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="113a6-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="113a6-104">Permissions</span></span>
<span data-ttu-id="113a6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="113a6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="113a6-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="113a6-107">Permission type</span></span>      | <span data-ttu-id="113a6-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="113a6-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="113a6-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="113a6-109">Delegated (work or school account)</span></span> | <span data-ttu-id="113a6-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="113a6-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="113a6-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="113a6-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="113a6-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="113a6-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="113a6-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="113a6-113">Application</span></span> | <span data-ttu-id="113a6-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="113a6-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="113a6-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="113a6-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```
GET /me/drive/recent
```

## <a name="request-body"></a><span data-ttu-id="113a6-116">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="113a6-116">Request body</span></span>
<span data-ttu-id="113a6-117">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="113a6-117">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="113a6-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="113a6-118">Example</span></span>

<!-- { "blockType": "request", "name": "drive-recent", "scopes": "files.read" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/recent
```

## <a name="response"></a><span data-ttu-id="113a6-119">Antwort</span><span class="sxs-lookup"><span data-stu-id="113a6-119">Response</span></span>

<span data-ttu-id="113a6-p103">Dadurch wird eine Sammlung von [DriveItem](../resources/driveitem.md)-Ressourcen für Elemente zurückgegeben, auf die der Besitzer des Laufwerks vor kurzem zugegriffen hat. Elemente außerhalb des Laufwerks des Benutzers enthalten das [RemoteItem](../resources/remoteitem.md)-Facet, das Informationen zum Zugriff auf das freigegebene Element bereitstellt.</span><span class="sxs-lookup"><span data-stu-id="113a6-p103">This returns a collection of [DriveItem](../resources/driveitem.md) resources for items which the owner of the drive has recently accessed. Items outside of the user's drive will include the [RemoteItem](../resources/remoteitem.md) facet, which provides information to access the shared item.</span></span>


<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "isCollection": true, "truncated": true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc!1231",
      "remoteItem":
      {
        "id": "1991210caf!192",
        "name": "March Proposal.docx",
        "file": { },
        "size": 19121,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    },
    {
      "id": "1312def!9943",
      "name": "Vacation.jpg",
      "file": { },
      "size": 37810,
      "parentReference": {
        "driveId": "1312def",
        "id": "1312def!123"
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="113a6-122">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="113a6-122">Remarks</span></span>

<span data-ttu-id="113a6-p104">Einige driveItems, die von der **recent**-Aktion zurückgegeben werden, enthalten immer das **remoteItem**-Facet, das angibt, dass es sich um Elemente von einem anderen Laufwerk handelt. Um auf das ursprüngliche DriveItem-Objekt zuzugreifen, müssen Sie eine Anforderung anhand der Angaben in **remoteItem** im folgenden Format stellen:</span><span class="sxs-lookup"><span data-stu-id="113a6-p104">Some driveItems returned from the **recent** action will include the **remoteItem** facet which indicates they are items from another drive. To access the original driveItem object, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- {"blockType": "ignored"} -->
```http
GET https://graph.microsoft.com/v1.0/drives/{remoteItem.driveId}/items/{remoteItem.id}
```

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve a list of files shared with the signed-in user.",
  "keywords": "sharedWithMe onedrive shared files",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Shared with me"
} -->
