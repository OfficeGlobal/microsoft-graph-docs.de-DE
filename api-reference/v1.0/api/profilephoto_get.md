# <a name="get-photo"></a><span data-ttu-id="de18e-101">Foto abrufen</span><span class="sxs-lookup"><span data-stu-id="de18e-101">Get photo</span></span>

<span data-ttu-id="de18e-102">Rufen Sie das angegebene [profilePhoto](../resources/profilephoto.md) oder die Metadaten (profilePhoto-Eigenschaften) ab.</span><span class="sxs-lookup"><span data-stu-id="de18e-102">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (profilePhoto properties).</span></span>

<span data-ttu-id="de18e-103">Ein GET-Vorgang sucht nach dem angegebenen Foto im Postfach des Benutzers in Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="de18e-103">A GET operation looks for the specified photo in the user's mailbox on Exchange Online.</span></span>

> <span data-ttu-id="de18e-104">**Hinweis:** Dieser Vorgang in Version 1.0 unterstützt ausschließlich Postfächer in Geschäfts-, Schul- oder Unikonten des Benutzers. Persönliche Postfächer werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="de18e-104">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="de18e-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="de18e-105">Permissions</span></span>
<span data-ttu-id="de18e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="de18e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

*   <span data-ttu-id="de18e-108">Profilfotos aller Benutzer im Mandanten, einschließlich des angemeldeten Benutzers: User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de18e-108">Profile photo of any user in the tenant including the signed-in user - User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>
*   <span data-ttu-id="de18e-109">Profilfoto des angemeldeten Benutzers: User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de18e-109">Profile photo of specifically the signed-in user - User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>
* <span data-ttu-id="de18e-110">Profilfoto einer **Gruppe**: Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de18e-110">Profile photo of a **group** - Group.Read.All, Group.ReadWrite.All</span></span>
* <span data-ttu-id="de18e-111">Foto eines **Kontakts**: Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de18e-111">Photo of a **contact** - Contacts.Read, Contacts.ReadWrite</span></span>

## <a name="http-request-to-get-the-photo"></a><span data-ttu-id="de18e-112">HTTP-Anforderung zum Abrufen des Fotos</span><span class="sxs-lookup"><span data-stu-id="de18e-112">HTTP request to get the photo</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo/$value
GET /users/{id | userPrincipalName}/photo/$value
GET /groups/{id}/photo/$value
GET /me/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contacts/{id}/photo/$value
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
## <a name="http-request-to-get-the-metadata-of-the-photo"></a><span data-ttu-id="de18e-113">HTTP-Anforderung zum Abrufen von Metadaten des Fotos</span><span class="sxs-lookup"><span data-stu-id="de18e-113">HTTP request to get the metadata of the photo</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /me/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contacts/{id}/photo
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="de18e-114">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="de18e-114">Optional query parameters</span></span>
<span data-ttu-id="de18e-115">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="de18e-115">This method supports the [OData Query Parameters](http://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="de18e-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="de18e-116">Request headers</span></span>
| <span data-ttu-id="de18e-117">Name</span><span class="sxs-lookup"><span data-stu-id="de18e-117">Name</span></span>       | <span data-ttu-id="de18e-118">Typ</span><span class="sxs-lookup"><span data-stu-id="de18e-118">Type</span></span> | <span data-ttu-id="de18e-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de18e-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="de18e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="de18e-120">Authorization</span></span>  | <span data-ttu-id="de18e-121">string</span><span class="sxs-lookup"><span data-stu-id="de18e-121">string</span></span>  | <span data-ttu-id="de18e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="de18e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de18e-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="de18e-124">Request body</span></span>
<span data-ttu-id="de18e-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="de18e-125">Do not supply a request body for this method.</span></span>
## <a name="response-for-getting-the-photo"></a><span data-ttu-id="de18e-126">Antwort für Abrufen des Fotos</span><span class="sxs-lookup"><span data-stu-id="de18e-126">Response for getting the photo</span></span>
<span data-ttu-id="de18e-p103">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und binäre Daten des angeforderten Fotos zurückgegeben.  Wenn kein Foto vorhanden ist, gibt der Vorgang `404 Not Found` zurück.</span><span class="sxs-lookup"><span data-stu-id="de18e-p103">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
## <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="de18e-129">Antwort für Abrufen der Metadaten des Fotos</span><span class="sxs-lookup"><span data-stu-id="de18e-129">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="de18e-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [profilePhoto](../resources/profilePhoto.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="de18e-130">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilePhoto.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="de18e-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="de18e-131">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="de18e-132">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="de18e-132">Request 1</span></span>
<span data-ttu-id="de18e-133">Diese Anforderung ruft das Foto des angemeldeten Benutzers mit der größten verfügbaren Größe ab.</span><span class="sxs-lookup"><span data-stu-id="de18e-133">This request gets the photo for the signed-in user, in the largest available size.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response-1"></a><span data-ttu-id="de18e-134">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="de18e-134">Response 1</span></span>
<span data-ttu-id="de18e-p104">Enthält die binären Daten des angeforderten Fotos. Der HTTP-Antwortcode ist 200.</span><span class="sxs-lookup"><span data-stu-id="de18e-p104">Contains the binary data of the requested photo. The HTTP response code is 200.</span></span>

##### <a name="request-2"></a><span data-ttu-id="de18e-137">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="de18e-137">Request 2</span></span>
<span data-ttu-id="de18e-138">Diese Anforderung ruft die Metadaten des Benutzerfotos des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="de18e-138">This request gets the metadata of the user photo of the signed-in user.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response-2"></a><span data-ttu-id="de18e-139">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="de18e-139">Response 2</span></span>

<span data-ttu-id="de18e-p105">Die folgenden Antwortdaten zeigen die Metadaten des Fotos. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="de18e-p105">The following response data shows the photo metadata. Note: The response object shown here may be truncated for brevity.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

<span data-ttu-id="de18e-p106">Die folgenden Antwortdaten zeigen die Inhalte einer Antwort, wenn für den Benutzer noch kein Foto hochgeladen wurde. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="de18e-p106">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user. Note: The response object shown here may be truncated for brevity.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/gif",
    "@odata.mediaEtag": "",
    "id": "1X1",
    "width": 1,
    "height": 1
}
```
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="de18e-144">Verwenden der Binärdaten des angeforderten Fotos</span><span class="sxs-lookup"><span data-stu-id="de18e-144">Using the binary data of the requested photo</span></span>

<span data-ttu-id="de18e-145">Wenn Sie den `/photo/$value`-Endpunkt zum Abrufen der Binärdaten für ein Profilfoto verwenden, müssen Sie die Daten in eine Base-64-Zeichenfolge konvertieren, damit sie als E-Mail-Anlage hinzugefügt werden können.</span><span class="sxs-lookup"><span data-stu-id="de18e-145">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="de18e-146">Das folgende Beispiel in JavaScript zeigt das Erstellen eines Arrays, das Sie als Wert des `Attachments`-Parameters einer [Outlook-Nachricht](user_post_messages.md) übergeben können.</span><span class="sxs-lookup"><span data-stu-id="de18e-146">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user_post_messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="de18e-147">Unter [Microsoft Graph Connect-Beispiel für Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) finden Sie eine Implementierung dieses Beispiels.</span><span class="sxs-lookup"><span data-stu-id="de18e-147">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="de18e-148">Wenn Sie das Bild auf einer Webseite anzeigen möchten, erstellen Sie ein Objekt im Arbeitsspeicher aus dem Bild, und verwenden Sie das Objekt als Quelle eines Bildelements.</span><span class="sxs-lookup"><span data-stu-id="de18e-148">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="de18e-149">Hier ist ein Beispiel in JavaScript für diesen Vorgang.</span><span class="sxs-lookup"><span data-stu-id="de18e-149">Here is an example in JavaScript of this operation.</span></span>

    const url = window.URL || window.webkitURL;
    const blobUrl = url.createObjectURL(image.data);
    document.getElementById(imageElement).setAttribute("src", blobUrl);

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
