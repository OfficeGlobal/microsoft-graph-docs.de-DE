# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="aa758-101">Directory-Objekte aus einer Liste von IDs abrufen</span><span class="sxs-lookup"><span data-stu-id="aa758-101">Get directory objects from a list of ids</span></span>

<span data-ttu-id="aa758-p101">Gibt die in einer Liste von IDs angegebenen Directory-Objekte zurück.  HINWEIS: Die zurückgegebenen Directory-Objekte sind die vollständigen Objekte mit **allen** Eigenschaften. Die Abfrageoption `$select` ist für diesen Vorgang nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="aa758-p101">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="aa758-105">Nachfolgend sind einige gängige Verwendungsmöglichkeiten für diese Funktion aufgeführt:</span><span class="sxs-lookup"><span data-stu-id="aa758-105">Some common uses for this function are to:</span></span>

* <span data-ttu-id="aa758-106">Auflösen von IDs, die von Funktionen zurückgegeben werden (die Sammlungen von IDs zurückgeben), z. B. [getMemberObjects](directoryobject_getmemberobjects.md) oder [getMemberGroups](directoryobject_getmembergroups.md) in ihre zugrunde liegenden Directory-Objekte.</span><span class="sxs-lookup"><span data-stu-id="aa758-106">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](directoryobject_getmemberobjects.md) or [getMemberGroups](directoryobject_getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="aa758-107">Auflösen von durch die Anwendung permanent in einem externen Speicher gespeicherten IDs in ihre zugrunde liegenden Verzeichnisobjekte</span><span class="sxs-lookup"><span data-stu-id="aa758-107">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa758-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="aa758-108">Permissions</span></span>

<span data-ttu-id="aa758-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aa758-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="aa758-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aa758-111">Permission type</span></span>      | <span data-ttu-id="aa758-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aa758-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa758-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aa758-113">Delegated (work or school account)</span></span> | <span data-ttu-id="aa758-114">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aa758-114">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aa758-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aa758-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa758-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aa758-116">Not supported.</span></span>    |
|<span data-ttu-id="aa758-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aa758-117">Application</span></span> | <span data-ttu-id="aa758-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa758-118">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa758-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa758-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getById
```

## <a name="request-headers"></a><span data-ttu-id="aa758-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aa758-120">Request headers</span></span>

| <span data-ttu-id="aa758-121">Name</span><span class="sxs-lookup"><span data-stu-id="aa758-121">Name</span></span>       | <span data-ttu-id="aa758-122">Typ</span><span class="sxs-lookup"><span data-stu-id="aa758-122">Type</span></span> | <span data-ttu-id="aa758-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa758-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aa758-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa758-124">Authorization</span></span>  | <span data-ttu-id="aa758-125">string</span><span class="sxs-lookup"><span data-stu-id="aa758-125">string</span></span>  | <span data-ttu-id="aa758-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aa758-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aa758-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aa758-128">Content-Type</span></span>  | <span data-ttu-id="aa758-129">application/json</span><span class="sxs-lookup"><span data-stu-id="aa758-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aa758-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aa758-130">Request body</span></span>

<span data-ttu-id="aa758-131">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="aa758-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="aa758-132">Parameter</span><span class="sxs-lookup"><span data-stu-id="aa758-132">Parameter</span></span>   | <span data-ttu-id="aa758-133">Typ</span><span class="sxs-lookup"><span data-stu-id="aa758-133">Type</span></span> |<span data-ttu-id="aa758-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa758-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa758-135">ids</span><span class="sxs-lookup"><span data-stu-id="aa758-135">ids</span></span>|<span data-ttu-id="aa758-136">String collection</span><span class="sxs-lookup"><span data-stu-id="aa758-136">String collection</span></span>| <span data-ttu-id="aa758-p104">Eine Sammlung von IDs, für die Objekte zurückgegeben werden sollen. Sie können bis zu 1000 IDs angeben.</span><span class="sxs-lookup"><span data-stu-id="aa758-p104">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="aa758-139">types</span><span class="sxs-lookup"><span data-stu-id="aa758-139">types</span></span>|<span data-ttu-id="aa758-140">String collection</span><span class="sxs-lookup"><span data-stu-id="aa758-140">String collection</span></span>| <span data-ttu-id="aa758-p105">Eine Sammlung von Ressourcentypen, die den Satz von zu durchsuchenden Ressourcensammlungen angibt. Wenn keine Angabe erfolgt, wird [directoryObject](../resources/directoryobject.md) als Standardwert verwendet; dieser enthält alle im Verzeichnis definierten Ressourcentypen. Jedes Objekt, das von `directoryObject` abgeleitet wird, kann in der Sammlung angegeben werden; Beispiel: [user](../resources/user.md), [group](../resources/group.md), [device](../resources/device.md) usw. Bei den Werten wird nicht zwischen Groß- und Kleinschreibung unterschieden.</span><span class="sxs-lookup"><span data-stu-id="aa758-p105">A collection of resource types that specifies the set of resource collections to search. If not specified, the default is [directoryObject](../resources/directoryobject.md), which contains all of the resource types defined in the directory. Any object that derives from `directoryObject` may be specified in the collection; for example: [user](../resources/user.md), [group](../resources/group.md), [device](../resources/device.md), and so on. The values are not case sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="aa758-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa758-145">Response</span></span>

<span data-ttu-id="aa758-146">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200, OK` und das String-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa758-146">If successful, this method returns `200, OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa758-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aa758-147">Example</span></span>

##### <a name="request"></a><span data-ttu-id="aa758-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa758-148">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getById"
}-->

```http
POST https://graph.microsoft.com/v1.0/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893-8749-40a3-97b7-68513b600544","5d6059b6-368d-45f8-91e1-8e07d485f1d0"],
    "types":["user"]
}
```

##### <a name="response"></a><span data-ttu-id="aa758-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa758-149">Response</span></span>

<span data-ttu-id="aa758-p106">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa758-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
    "value": [
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Trevor Jones"
      },
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Billy Smith"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
