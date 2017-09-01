# <a name="get-a-special-folder-by-name"></a><span data-ttu-id="d030c-101">Speziellen Ordner nach Name abrufen</span><span class="sxs-lookup"><span data-stu-id="d030c-101">Get a special folder by name</span></span>

<span data-ttu-id="d030c-102">Verwenden Sie spezielle Auflistung, um auf einen speziellen Ordner basierend auf dem Namen zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="d030c-102">Use the special collection to access a special folder by name.</span></span>

<span data-ttu-id="d030c-p101">Spezielle Ordner bieten einfache Aliase für den Zugriff auf bekannte Ordner in OneDrive, ohne dass der Ordner anhand des Pfads nachgeschlagen werden muss (wofür eine Lokalisierung erforderlich wäre) oder anhand einer ID auf den Ordner verwiesen werden muss. Wenn ein spezieller Ordner umbenannt oder an eine andere Position innerhalb des Laufwerks verschoben wird, kann mit dieser Syntax weiterhin nach diesem Ordner gesucht werden.</span><span class="sxs-lookup"><span data-stu-id="d030c-p101">Special folders provide simple aliases to access well-known folders in OneDrive without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to find that folder.</span></span>

<span data-ttu-id="d030c-p102">Spezielle Ordner werden automatisch erstellt, wenn eine Anwendung das erste Mal versucht, einen Ordner zu schreiben, wenn noch keiner vorhanden ist. Wenn ein Benutzer einen speziellen Ordner löscht, wird dieser neu erstellt, wenn erneut in den Ordner geschrieben wird.</span><span class="sxs-lookup"><span data-stu-id="d030c-p102">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

><span data-ttu-id="d030c-107">**Hinweis:**  Wenn Sie nur über Leseberechtigungen verfügen und einen speziellen Ordner anfordern, der nicht vorhanden ist, wird ein `403 Forbidden`-Fehler angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d030c-107">**Note:**  If you have read-only permissions and request a special folder that doesn't exist, you'll receive a `403 Forbidden` error.</span></span>

## <a name="permissions"></a><span data-ttu-id="d030c-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d030c-108">Permissions</span></span>

<span data-ttu-id="d030c-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d030c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d030c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d030c-111">Permission type</span></span>                        | <span data-ttu-id="d030c-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d030c-112">Permissions (from least to most privileged)</span></span>                                                           |
|:--------------------------------------|:------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="d030c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d030c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d030c-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d030c-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |
|<span data-ttu-id="d030c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d030c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d030c-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Files.ReadWrite.AppFolder</span><span class="sxs-lookup"><span data-stu-id="d030c-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Files.ReadWrite.AppFolder</span></span>           |
|<span data-ttu-id="d030c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d030c-117">Application</span></span>                            | <span data-ttu-id="d030c-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d030c-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="d030c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d030c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/special/{name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d030c-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d030c-120">Optional query parameters</span></span>

<span data-ttu-id="d030c-121">Diese Methode unterstützt die [OData-Abfrageparameter](../../../concepts/query_parameters.md) von  `$expand` und `$select` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d030c-121">This method supports the `$expand` and `$select` [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d030c-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d030c-122">Request headers</span></span>

| <span data-ttu-id="d030c-123">Name</span><span class="sxs-lookup"><span data-stu-id="d030c-123">Name</span></span>          | <span data-ttu-id="d030c-124">Typ</span><span class="sxs-lookup"><span data-stu-id="d030c-124">Type</span></span>   | <span data-ttu-id="d030c-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d030c-125">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="d030c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d030c-126">Authorization</span></span> | <span data-ttu-id="d030c-127">string</span><span class="sxs-lookup"><span data-stu-id="d030c-127">string</span></span> | <span data-ttu-id="d030c-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d030c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d030c-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d030c-130">Request body</span></span>

<span data-ttu-id="d030c-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d030c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d030c-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="d030c-132">Response</span></span>

<span data-ttu-id="d030c-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [driveItem](../resources/driveitem.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d030c-133">If successful, this method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d030c-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d030c-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d030c-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d030c-135">Request</span></span>

<span data-ttu-id="d030c-136">Hier ist ein Beispiel für die Anforderung der Laufwerke des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="d030c-136">Here is an example of the request for the user's drives.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drive_special"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/special/{name}
```

##### <a name="response"></a><span data-ttu-id="d030c-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="d030c-137">Response</span></span>
<span data-ttu-id="d030c-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d030c-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "folder": { },
  "id": "s!lkjqwlkj124912049an",
  "name": "Photos",
  "specialFolder": { "name": "photos" },
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents/Photos",
}
```

## <a name="remarks"></a><span data-ttu-id="d030c-139">Hinweise</span><span class="sxs-lookup"><span data-stu-id="d030c-139">Remarks</span></span>

<span data-ttu-id="d030c-140">Um die untergeordneten Elemente eines speziellen Ordners anzufordern, können Sie die `children`-Sammlung anfordern oder die Option [$expand](../../../concepts/query_parameters.md) verwenden, um die Sammlung untergeordneter Elemente zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="d030c-140">To request the children of a special folder, you can request the `children` collection or use the [expand](../../../concepts/query_parameters.md) option to expand the children collection.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List drives",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Get special folder"
}-->
