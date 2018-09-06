# <a name="get-photo"></a><span data-ttu-id="9b371-101">Foto abrufen</span><span class="sxs-lookup"><span data-stu-id="9b371-101">Get photo</span></span>

<span data-ttu-id="9b371-102">Rufen Sie das angegebene [profilePhoto](../resources/profilephoto.md) oder die Metadaten (profilePhoto-Eigenschaften) ab.</span><span class="sxs-lookup"><span data-stu-id="9b371-102">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (profilePhoto properties).</span></span>

> <span data-ttu-id="9b371-103">**Hinweis:** Dieser Vorgang in Version 1.0 unterstützt ausschließlich Postfächer in Geschäfts-, Schul- oder Unikonten des Benutzers. Persönliche Postfächer werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9b371-103">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

<span data-ttu-id="9b371-104">Die unterstützten Größen der HD-Fotos in Office 365 sind wie folgt: „48x48“, „64x64“, „96x96“, „120x120“, „240x240“, „360x360“,“432x432“, „504x504“ und „648x648“.</span><span class="sxs-lookup"><span data-stu-id="9b371-104">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="9b371-105">Fotos können eine beliebige Größe aufweisen, wenn sie in Azure Active Directory gespeichert sind.</span><span class="sxs-lookup"><span data-stu-id="9b371-105">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="9b371-106">Sie können die Metadaten des größten verfügbaren Fotos abrufen oder eine Größe angeben, um die Metadaten für diese Fotogröße abzurufen.</span><span class="sxs-lookup"><span data-stu-id="9b371-106">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="9b371-107">Wenn die angeforderte Größe nicht verfügbar ist, können Sie immer noch eine kleinere Größe abrufen, die der Benutzer hochgeladen und zur Verfügung gestellt hat.</span><span class="sxs-lookup"><span data-stu-id="9b371-107">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="9b371-108">Wenn der Benutzer beispielsweise ein Foto mit 504x504 Pixeln hochlädt, sind alle Fotogrößen bis auf 648x648 zum Download verfügbar.</span><span class="sxs-lookup"><span data-stu-id="9b371-108">For example, if the user uploads a photo that is 504x504 pixels, then all but the 648x648 size of photo will be available for download.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b371-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9b371-109">Permissions</span></span>

<span data-ttu-id="9b371-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9b371-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9b371-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9b371-112">Permission type</span></span>      | <span data-ttu-id="9b371-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9b371-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b371-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9b371-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9b371-115">Für **user**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="9b371-115">For **user** resource:</span></span><br/><span data-ttu-id="9b371-116">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b371-116">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="9b371-117">Für **group**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="9b371-117">For **group** resource:</span></span><br /><span data-ttu-id="9b371-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b371-118">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="9b371-119">Für **contact**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="9b371-119">For **contact** resource:</span></span><br /><span data-ttu-id="9b371-120">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b371-120">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="9b371-121">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9b371-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b371-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9b371-122">Not supported</span></span> |
|<span data-ttu-id="9b371-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9b371-123">Application</span></span>                        | <span data-ttu-id="9b371-124">Für **user**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="9b371-124">For **user** resource:</span></span><br/><span data-ttu-id="9b371-125">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b371-125">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="9b371-126">Für **group**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="9b371-126">For **group** resource:</span></span><br /><span data-ttu-id="9b371-127">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b371-127">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="9b371-128">Für **contact**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="9b371-128">For **contact** resource:</span></span><br /><span data-ttu-id="9b371-129">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b371-129">Contacts.Read, Contacts.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="9b371-130">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9b371-130">HTTP request</span></span> 

### <a name="get-the-photo"></a><span data-ttu-id="9b371-131">Foto abrufen</span><span class="sxs-lookup"><span data-stu-id="9b371-131">Get the user's photo.</span></span>
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
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="9b371-132">Metadaten des Fotos abrufen</span><span class="sxs-lookup"><span data-stu-id="9b371-132">Get the metadata for the largest available photo</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo
GET /me/photos
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /me/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contacts/{id}/photo
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo
```

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="9b371-133">Metadaten für eine bestimmte Fotogröße abrufen</span><span class="sxs-lookup"><span data-stu-id="9b371-133">HTTP request to get the metadata for a specific photo size</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photos/{size}
GET /users/{id | userPrincipalName}/photos/{size}
GET /groups/{id}/photos/{size}
GET /me/contacts/{id}/photos/{size}
GET /users/{id | userPrincipalName}/contacts/{id}/photos/{size}
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photos/{size}
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photos/{size}
```

## <a name="path-parameters"></a><span data-ttu-id="9b371-134">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="9b371-134">Path parameters</span></span>

|<span data-ttu-id="9b371-135">Parameter</span><span class="sxs-lookup"><span data-stu-id="9b371-135">Parameter</span></span>|<span data-ttu-id="9b371-136">Typ</span><span class="sxs-lookup"><span data-stu-id="9b371-136">Type</span></span>|<span data-ttu-id="9b371-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9b371-137">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9b371-138">size</span><span class="sxs-lookup"><span data-stu-id="9b371-138">size</span></span>  |<span data-ttu-id="9b371-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9b371-139">String</span></span>  | <span data-ttu-id="9b371-140">Eine Fotogröße.</span><span class="sxs-lookup"><span data-stu-id="9b371-140">A photo size.</span></span> <span data-ttu-id="9b371-141">Die unterstützten Größen der HD-Fotos in Office 365 sind wie folgt: „48x48“, „64x64“, „96x96“, „120x120“, „240x240“, „360x360“,“432x432“, „504x504“ und „648x648“.</span><span class="sxs-lookup"><span data-stu-id="9b371-141">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="9b371-142">Fotos können eine beliebige Größe aufweisen, wenn sie in Azure Active Directory gespeichert sind.</span><span class="sxs-lookup"><span data-stu-id="9b371-142">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="9b371-143">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9b371-143">Optional query parameters</span></span>
<span data-ttu-id="9b371-144">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9b371-144">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9b371-145">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9b371-145">Request headers</span></span>
| <span data-ttu-id="9b371-146">Name</span><span class="sxs-lookup"><span data-stu-id="9b371-146">Name</span></span>       | <span data-ttu-id="9b371-147">Typ</span><span class="sxs-lookup"><span data-stu-id="9b371-147">Type</span></span> | <span data-ttu-id="9b371-148">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9b371-148">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9b371-149">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9b371-149">Authorization</span></span>  | <span data-ttu-id="9b371-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9b371-150">string</span></span>  | <span data-ttu-id="9b371-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9b371-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b371-153">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9b371-153">Request body</span></span>
<span data-ttu-id="9b371-154">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9b371-154">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b371-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="9b371-155">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="9b371-156">Antwort für Abrufen des Fotos</span><span class="sxs-lookup"><span data-stu-id="9b371-156">Response for getting the photo</span></span>
<span data-ttu-id="9b371-p106">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und binäre Daten des angeforderten Fotos zurückgegeben.  Wenn kein Foto vorhanden ist, gibt der Vorgang `404 Not Found` zurück.</span><span class="sxs-lookup"><span data-stu-id="9b371-p106">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="9b371-159">Antwort für Abrufen der Metadaten des Fotos</span><span class="sxs-lookup"><span data-stu-id="9b371-159">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="9b371-160">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [profilePhoto](../resources/profilePhoto.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9b371-160">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilePhoto.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9b371-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9b371-161">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="9b371-162">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="9b371-162">Request 1</span></span>
<span data-ttu-id="9b371-163">Diese Anforderung ruft das Foto des angemeldeten Benutzers mit der größten verfügbaren Größe ab.</span><span class="sxs-lookup"><span data-stu-id="9b371-163">This request gets the photo for the signed-in user, in the largest available size.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response-1"></a><span data-ttu-id="9b371-164">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="9b371-164">Response 1</span></span>
<span data-ttu-id="9b371-p107">Enthält die binären Daten des angeforderten Fotos. Der HTTP-Antwortcode ist 200.</span><span class="sxs-lookup"><span data-stu-id="9b371-p107">Contains the binary data of the requested photo. The HTTP response code is 200.</span></span>

##### <a name="request-2"></a><span data-ttu-id="9b371-167">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="9b371-167">Request 2</span></span>
<span data-ttu-id="9b371-168">Diese Anforderung ruft das 48x48-Foto für den angemeldeten Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="9b371-168">This request gets the 48x48 photo for the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response-2"></a><span data-ttu-id="9b371-169">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="9b371-169">Response 2</span></span>
<span data-ttu-id="9b371-p108">Enthält die binären Daten des angeforderten 48x48-Fotos. Der HTTP-Antwortcode ist 200.</span><span class="sxs-lookup"><span data-stu-id="9b371-p108">Contains the binary data of the requested 48x48 photo. The HTTP response code is 200.</span></span>

##### <a name="request-3"></a><span data-ttu-id="9b371-172">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="9b371-172">Request 3</span></span>
<span data-ttu-id="9b371-173">Diese Anforderung ruft die Metadaten des Benutzerfotos des angemeldeten Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="9b371-173">This request gets the metadata of the user photo of the signed-in user.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response-3"></a><span data-ttu-id="9b371-174">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="9b371-174">Response 3</span></span>

<span data-ttu-id="9b371-p109">Die folgenden Antwortdaten zeigen die Metadaten des Fotos. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="9b371-p109">The following response data shows the photo metadata. Note: The response object shown here may be truncated for brevity.</span></span>
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

<span data-ttu-id="9b371-p110">Die folgenden Antwortdaten zeigen die Inhalte einer Antwort, wenn für den Benutzer noch kein Foto hochgeladen wurde. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="9b371-p110">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user. Note: The response object shown here may be truncated for brevity.</span></span>

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
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="9b371-179">Verwenden der Binärdaten des angeforderten Fotos</span><span class="sxs-lookup"><span data-stu-id="9b371-179">Using the binary data of the requested photo</span></span>

<span data-ttu-id="9b371-180">Wenn Sie den `/photo/$value`-Endpunkt zum Abrufen der Binärdaten für ein Profilfoto verwenden, müssen Sie die Daten in eine Base-64-Zeichenfolge konvertieren, damit sie als E-Mail-Anlage hinzugefügt werden können.</span><span class="sxs-lookup"><span data-stu-id="9b371-180">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="9b371-181">Das folgende Beispiel in JavaScript zeigt das Erstellen eines Arrays, das Sie als Wert des `Attachments`-Parameters einer [Outlook-Nachricht](user_post_messages.md) übergeben können.</span><span class="sxs-lookup"><span data-stu-id="9b371-181">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user_post_messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="9b371-182">Unter [Microsoft Graph Connect-Beispiel für Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) finden Sie eine Implementierung dieses Beispiels.</span><span class="sxs-lookup"><span data-stu-id="9b371-182">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="9b371-183">Wenn Sie das Bild auf einer Webseite anzeigen möchten, erstellen Sie ein Objekt im Arbeitsspeicher aus dem Bild, und verwenden Sie das Objekt als Quelle eines Bildelements.</span><span class="sxs-lookup"><span data-stu-id="9b371-183">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="9b371-184">Hier ist ein Beispiel in JavaScript für diesen Vorgang.</span><span class="sxs-lookup"><span data-stu-id="9b371-184">Here is an example in JavaScript of this operation.</span></span>

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
