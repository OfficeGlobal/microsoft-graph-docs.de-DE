# <a name="accessing-shared-driveitems"></a><span data-ttu-id="ef0dc-101">Zugriff auf freigegebene DriveItems</span><span class="sxs-lookup"><span data-stu-id="ef0dc-101">Accessing shared DriveItems</span></span>

<span data-ttu-id="ef0dc-102">Verwenden Sie für den Zugriff auf ein freigegebenes [DriveItem](../resources/driveitem.md)-Element oder eine Sammlung freigegebener Elemente eine **shareId** oder Freigabe-URL.</span><span class="sxs-lookup"><span data-stu-id="ef0dc-102">Access a shared [DriveItem](../resources/driveitem.md) or a collection of shared items by using a **shareId** or sharing URL.</span></span>

<span data-ttu-id="ef0dc-103">Um eine Freigabe-URL mit dieser API verwenden zu können, muss die App [die URL in ein Freigabetoken konvertieren](#transform-a-sharing-url).</span><span class="sxs-lookup"><span data-stu-id="ef0dc-103">To use a sharing URL with this API, your app needs to [transform the URL into a sharing token](#transform-a-sharing-url).</span></span>

## <a name="permissions"></a><span data-ttu-id="ef0dc-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ef0dc-104">Permissions</span></span>

<span data-ttu-id="ef0dc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ef0dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ef0dc-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ef0dc-107">Permission type</span></span>      | <span data-ttu-id="ef0dc-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ef0dc-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef0dc-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ef0dc-109">Delegated (work or school account)</span></span> | <span data-ttu-id="ef0dc-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef0dc-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ef0dc-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ef0dc-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef0dc-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef0dc-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ef0dc-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ef0dc-113">Application</span></span> | <span data-ttu-id="ef0dc-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef0dc-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef0dc-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef0dc-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /shares/{sharingIdOrUrl}
```

## <a name="request-body"></a><span data-ttu-id="ef0dc-116">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ef0dc-116">Request body</span></span>
<span data-ttu-id="ef0dc-117">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ef0dc-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef0dc-118">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef0dc-118">Response</span></span>

<span data-ttu-id="ef0dc-119">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine [sharedDriveItem](../resources/shareddriveitem.md)-Ressource im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ef0dc-119">If successful, this method returns a `200 OK` response code and a [sharedDriveItem](../resources/shareddriveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef0dc-120">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ef0dc-120">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ef0dc-121">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef0dc-121">Request</span></span>

<span data-ttu-id="ef0dc-122">Im Folgenden finden Sie ein Beispiel für die Anforderung zum Abrufen eines freigegebenen Elements:</span><span class="sxs-lookup"><span data-stu-id="ef0dc-122">Here is an example of the request to retrieve a shared item:</span></span>

<!-- {
  "blockType": "request",
  "name": "get_shares_by_url"
}-->
```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}
```
##### <a name="response"></a><span data-ttu-id="ef0dc-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef0dc-123">Response</span></span>

<span data-ttu-id="ef0dc-124">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ef0dc-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharedDriveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "B64397C8-07AE-43E4-920E-32BFB4331A5B",
  "name": "contoso project.docx",
  "owner": {
    "user": {
      "id": "98E88F1C-F8DC-47CC-A406-C090248B30E5",
      "displayName": "Ryan Gregg"
    }
  }
}
```

## <a name="access-the-shared-item-directly"></a><span data-ttu-id="ef0dc-125">Direkter Zugriff auf das freigegebene Element</span><span class="sxs-lookup"><span data-stu-id="ef0dc-125">Access the shared item directly</span></span>

<span data-ttu-id="ef0dc-p102">Obwohl das [**SharedDriveItem**](../resources/shareddriveitem.md)-Element nützliche Informationen enthält, möchten die meisten Apps direkt auf das freigegebene [DriveItem](../resources/driveitem.md)-Element zugreifen. Die **SharedDriveItem**-Ressource umfasst **root**- und **items**-Beziehungen, die innerhalb des Bereichs des freigegebenen Elements auf die Inhalte zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="ef0dc-p102">While the [**SharedDriveItem**](../resources/shareddriveitem.md) contains some useful information, most apps will want to directly access the shared [DriveItem](../resources/driveitem.md). The **SharedDriveItem** resource includes a **root** and **items** relationships which can access content within the scope of the shared item.</span></span>

## <a name="example-single-file"></a><span data-ttu-id="ef0dc-128">Beispiel (einzelne Datei)</span><span class="sxs-lookup"><span data-stu-id="ef0dc-128">Example (single file)</span></span>

##### <a name="request"></a><span data-ttu-id="ef0dc-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef0dc-129">Request</span></span>

<span data-ttu-id="ef0dc-130">Durch das Anfordern der **root**-Beziehung wird das **DriveItem**-Element zurückgegeben, das freigegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="ef0dc-130">By requesting the **root** relationship, the **DriveItem** that was shared will be returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}/root
```

##### <a name="response"></a><span data-ttu-id="ef0dc-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef0dc-131">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "contoso project.docx",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "file": {},
  "size": 109112
}
```

## <a name="example-shared-folder"></a><span data-ttu-id="ef0dc-132">Beispiel (freigegebener Ordner)</span><span class="sxs-lookup"><span data-stu-id="ef0dc-132">Example (shared folder)</span></span>

##### <a name="request"></a><span data-ttu-id="ef0dc-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef0dc-133">Request</span></span>

<span data-ttu-id="ef0dc-134">Durch das Anfordern der **root**-Beziehung und das Erweitern der **children**-Sammlung wird das freigegebene **DriveItem**-Element mit Dateien im freigegebenen Ordner zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ef0dc-134">By requesting the **root** relationship and expanding the **children** collection, the **DriveItem** that was shared will be returned along with the files within the shared folder.</span></span>

```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}/root?$expand=children
```

##### <a name="response"></a><span data-ttu-id="ef0dc-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef0dc-135">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "Contoso Project",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "folder": {}
  "size": 10911212,
  "children": [
    {
      "id": "AFBBDD79-868E-452D-AD4D-24697D4A4044",
      "name": "Propsoal.docx",
      "file": {},
      "size": 19001
    },
    {
      "id": "A91FE90A-2F2C-4EE6-B412-C4FFBA3F71A6",
      "name": "Update to Proposal.docx",
      "file": {},
      "size": 91001
    }
  ]
}
```

## <a name="transform-a-sharing-url"></a><span data-ttu-id="ef0dc-136">Konvertieren einer Freigabe-URL</span><span class="sxs-lookup"><span data-stu-id="ef0dc-136">Transform a sharing URL</span></span>

<span data-ttu-id="ef0dc-137">Um auf eine Freigabe-URL unter Verwendung der **shares**-API zuzugreifen, muss die URL in ein Freigabetoken umgewandelt werden.</span><span class="sxs-lookup"><span data-stu-id="ef0dc-137">To access a sharing URL using the **shares** API, the URL needs to be transformed into a sharing token.</span></span>

<span data-ttu-id="ef0dc-138">So wandeln Sie eine URL in ein Freigabetoken um:</span><span class="sxs-lookup"><span data-stu-id="ef0dc-138">To transform a URL into a sharing token:</span></span>

1. <span data-ttu-id="ef0dc-139">Codieren Sie die URL-Freigabe mithilfe von Base64.</span><span class="sxs-lookup"><span data-stu-id="ef0dc-139">Base64 encode the sharing URL.</span></span>
2. <span data-ttu-id="ef0dc-140">Konvertieren Sie die Base64-codierten Daten in das [base64url-Format ohne Füllzeichen](https://en.wikipedia.org/wiki/Base64), indem Sie folgende Aktionen durchführen:</span><span class="sxs-lookup"><span data-stu-id="ef0dc-140">Convert the base64 encoded data to [unpadded base64url format](https://en.wikipedia.org/wiki/Base64) by:</span></span>
  1. <span data-ttu-id="ef0dc-141">Kürzen Sie nachgestellte `=`-Zeichen in der Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ef0dc-141">Trim trailing `=` characters from the string</span></span>
  2. <span data-ttu-id="ef0dc-142">Ersetzen Sie unsichere URL-Zeichen mit einem entsprechenden Zeichen; ersetzen Sie `/` mit `_` und `+` mit `-`.</span><span class="sxs-lookup"><span data-stu-id="ef0dc-142">Replace unsafe URL characters with an equivalent character; replace `/` with `_` and `+` with `-`.</span></span>
3. <span data-ttu-id="ef0dc-143">Fügen Sie `u!` an den Anfang der Zeichenfolge an.</span><span class="sxs-lookup"><span data-stu-id="ef0dc-143">Append `u!` to the beginning of the string.</span></span>

<span data-ttu-id="ef0dc-144">Mit der folgenden C#-Methode wird beispielsweise eine Eingabezeichenfolge in eine Freigabetoken konvertiert:</span><span class="sxs-lookup"><span data-stu-id="ef0dc-144">For example, the following C# method transforms an input string into a sharing token:</span></span>

```csharp
string UrlToSharingToken(string inputUrl) {
  var base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(inputUrl));
  return "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->
