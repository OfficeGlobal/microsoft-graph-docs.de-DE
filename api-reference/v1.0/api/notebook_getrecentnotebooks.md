# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="eac3f-101">notebook: getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="eac3f-101">notebook: getRecentNotebooks</span></span>

<span data-ttu-id="eac3f-102">Rufen Sie eine Liste der [recentNotebook](../resources/recentnotebook.md)-Instanzen ab, auf die vom angemeldeten Benutzer zugegriffen wurde.</span><span class="sxs-lookup"><span data-stu-id="eac3f-102">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="eac3f-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="eac3f-103">Permissions</span></span>
<span data-ttu-id="eac3f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="eac3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eac3f-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eac3f-106">Permission type</span></span>      | <span data-ttu-id="eac3f-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eac3f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eac3f-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eac3f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="eac3f-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span><span class="sxs-lookup"><span data-stu-id="eac3f-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>|
|<span data-ttu-id="eac3f-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eac3f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eac3f-111">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eac3f-111">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="eac3f-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eac3f-112">Application</span></span> | <span data-ttu-id="eac3f-113">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eac3f-113">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eac3f-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eac3f-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/<id | userPrincipalName>/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="eac3f-115">Der `<id | userPrincipalName>` für den Benutzer muss mit dem im Autorisierungstoken (zur Erstellung der Anforderung verwendet) codierten Benutzer übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="eac3f-115">The `<id | userPrincipalName>` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eac3f-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eac3f-116">Request headers</span></span>
| <span data-ttu-id="eac3f-117">Name</span><span class="sxs-lookup"><span data-stu-id="eac3f-117">Name</span></span>       | <span data-ttu-id="eac3f-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eac3f-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="eac3f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="eac3f-119">Authorization</span></span>  | <span data-ttu-id="eac3f-120">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="eac3f-120">Bearer {code}</span></span>|

## <a name="request-parameters"></a><span data-ttu-id="eac3f-121">Anforderungsparameter</span><span class="sxs-lookup"><span data-stu-id="eac3f-121">Request parameters</span></span>
<span data-ttu-id="eac3f-122">Stellen Sie in der URL der Anforderung die folgenden Abfrageparameter mit Werten bereit.</span><span class="sxs-lookup"><span data-stu-id="eac3f-122">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="eac3f-123">Parameter</span><span class="sxs-lookup"><span data-stu-id="eac3f-123">Parameter</span></span>    | <span data-ttu-id="eac3f-124">Typ</span><span class="sxs-lookup"><span data-stu-id="eac3f-124">Type</span></span>   |<span data-ttu-id="eac3f-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eac3f-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eac3f-126">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="eac3f-126">includePersonalNotebooks</span></span>|<span data-ttu-id="eac3f-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="eac3f-127">Boolean</span></span>|<span data-ttu-id="eac3f-128">Schließen Sie Notizbücher ein, die dem Benutzer gehören.</span><span class="sxs-lookup"><span data-stu-id="eac3f-128">Include notebooks owned by the user.</span></span> <span data-ttu-id="eac3f-129">Wählen Sie `true`, um Notizbücher einzuschließen, die dem Benutzer gehören; wählen Sie andernfalls `false`.</span><span class="sxs-lookup"><span data-stu-id="eac3f-129">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="eac3f-130">Wenn Sie den Parameter `includePersonalNotebooks` nicht einschließen, gibt Ihre Anforderung eine `400`-Fehlermeldung zurück.</span><span class="sxs-lookup"><span data-stu-id="eac3f-130">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eac3f-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eac3f-131">Request body</span></span>
<span data-ttu-id="eac3f-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="eac3f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eac3f-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="eac3f-133">Response</span></span>
<span data-ttu-id="eac3f-134">Eine erfolgreiche Antwort gibt `200 OK` mit einer JSON-Sammlung von **recentNotebooks** zurück.</span><span class="sxs-lookup"><span data-stu-id="eac3f-134">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="eac3f-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eac3f-135">Example</span></span>
<span data-ttu-id="eac3f-136">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="eac3f-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="eac3f-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eac3f-137">Request</span></span>
<span data-ttu-id="eac3f-138">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="eac3f-138">The following example shows the request.</span></span>
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/onenote/notebooks/getrecentnotebooks(includePersonalNotebooks=true)
```

#### <a name="response"></a><span data-ttu-id="eac3f-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="eac3f-139">Response</span></span>
<span data-ttu-id="eac3f-140">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="eac3f-140">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 1110

{
  "value":[
    {
      "name":"Personal Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDrive"
    },{
      "name":"Team Shared Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDriveForBusiness"
    }
  ]
}
```
