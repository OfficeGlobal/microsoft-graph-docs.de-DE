# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="ff37a-101">notebook: getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="ff37a-101">notebook: getRecentNotebooks</span></span>

<span data-ttu-id="ff37a-102">Rufen Sie eine Liste der [recentNotebook](../resources/recentnotebook.md)-Instanzen ab, auf die vom angemeldeten Benutzer zugegriffen wurde.</span><span class="sxs-lookup"><span data-stu-id="ff37a-102">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff37a-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ff37a-103">Permissions</span></span>
<span data-ttu-id="ff37a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ff37a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ff37a-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ff37a-106">Permission type</span></span>      | <span data-ttu-id="ff37a-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ff37a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff37a-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ff37a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ff37a-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span><span class="sxs-lookup"><span data-stu-id="ff37a-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span></span>|
|<span data-ttu-id="ff37a-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ff37a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff37a-111">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff37a-111">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="ff37a-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ff37a-112">Application</span></span> | <span data-ttu-id="ff37a-113">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff37a-113">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff37a-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff37a-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/{id | userPrincipalName}/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="ff37a-115">Der `<id | userPrincipalName>` für den Benutzer muss mit dem im Autorisierungstoken (zur Erstellung der Anforderung verwendet) codierten Benutzer übereinstimmen.</span><span class="sxs-lookup"><span data-stu-id="ff37a-115">The `<id | userPrincipalName>` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="ff37a-116">Funktionsparameter</span><span class="sxs-lookup"><span data-stu-id="ff37a-116">Function parameters</span></span>

| <span data-ttu-id="ff37a-117">Parameter</span><span class="sxs-lookup"><span data-stu-id="ff37a-117">Parameter</span></span>    | <span data-ttu-id="ff37a-118">Typ</span><span class="sxs-lookup"><span data-stu-id="ff37a-118">Type</span></span>   |<span data-ttu-id="ff37a-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff37a-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff37a-120">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="ff37a-120">includePersonalNotebooks</span></span>|<span data-ttu-id="ff37a-121">boolesch</span><span class="sxs-lookup"><span data-stu-id="ff37a-121">Boolean</span></span>|<span data-ttu-id="ff37a-122">Schließen Sie Notizbücher ein, die dem Benutzer gehören.</span><span class="sxs-lookup"><span data-stu-id="ff37a-122">Include notebooks owned by the user.</span></span> <span data-ttu-id="ff37a-123">Wählen Sie `true`, um Notizbücher einzuschließen, die dem Benutzer gehören; wählen Sie andernfalls `false`.</span><span class="sxs-lookup"><span data-stu-id="ff37a-123">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="ff37a-124">Wenn Sie den Parameter `includePersonalNotebooks` nicht einschließen, gibt Ihre Anforderung eine `400`-Fehlermeldung zurück.</span><span class="sxs-lookup"><span data-stu-id="ff37a-124">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="ff37a-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ff37a-125">Request headers</span></span>
| <span data-ttu-id="ff37a-126">Name</span><span class="sxs-lookup"><span data-stu-id="ff37a-126">Name</span></span>       | <span data-ttu-id="ff37a-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff37a-127">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ff37a-128">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ff37a-128">Authorization</span></span>  | <span data-ttu-id="ff37a-129">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ff37a-129">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff37a-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ff37a-130">Request body</span></span>
<span data-ttu-id="ff37a-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ff37a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff37a-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff37a-132">Response</span></span>
<span data-ttu-id="ff37a-133">Eine erfolgreiche Antwort gibt `200 OK` mit einer JSON-Sammlung von **recentNotebooks** zurück.</span><span class="sxs-lookup"><span data-stu-id="ff37a-133">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="ff37a-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ff37a-134">Example</span></span>
<span data-ttu-id="ff37a-135">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="ff37a-135">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="ff37a-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff37a-136">Request</span></span>
<span data-ttu-id="ff37a-137">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="ff37a-137">The following example shows the request.</span></span>
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=true)
```

#### <a name="response"></a><span data-ttu-id="ff37a-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff37a-138">Response</span></span>
<span data-ttu-id="ff37a-139">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="ff37a-139">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.recentNotebook)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 1110

{
  "value":[
    {
      "displayName":"Personal Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDrive"
    },{
      "displayName":"Team Shared Notebook","lastAccessedTime":"timestamp","links":{
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
