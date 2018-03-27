# <a name="get-photo"></a><span data-ttu-id="853a3-101">Foto abrufen</span><span class="sxs-lookup"><span data-stu-id="853a3-101">Get photo</span></span>

<span data-ttu-id="853a3-102">Rufen Sie das angegebene [profilePhoto](../resources/profilephoto.md) oder die Metadaten (profilePhoto-Eigenschaften) ab.</span><span class="sxs-lookup"><span data-stu-id="853a3-102">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (profilePhoto properties).</span></span>

> <span data-ttu-id="853a3-103">**Hinweis:** Dieser Vorgang in Version 1.0 unterstützt ausschließlich Postfächer in Geschäfts-, Schul- oder Unikonten des Benutzers. Persönliche Postfächer werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="853a3-103">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

<span data-ttu-id="853a3-104">Die unterstützten Größen der HD-Fotos in Office 365 sind wie folgt: „48x48“, „64x64“, „96x96“, „120x120“, „240x240“, „360x360“,“432x432“, „504x504“ und „648x648“.</span><span class="sxs-lookup"><span data-stu-id="853a3-104">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="853a3-105">Fotos können eine beliebige Größe aufweisen, wenn sie in Azure Active Directory gespeichert sind.</span><span class="sxs-lookup"><span data-stu-id="853a3-105">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="853a3-106">Sie können die Metadaten des größten verfügbaren Fotos abrufen oder eine Größe angeben, um die Metadaten für diese Fotogröße abzurufen.</span><span class="sxs-lookup"><span data-stu-id="853a3-106">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="853a3-107">Wenn die angeforderte Größe nicht verfügbar ist, können Sie immer noch eine kleinere Größe abrufen, die der Benutzer hochgeladen und zur Verfügung gestellt hat.</span><span class="sxs-lookup"><span data-stu-id="853a3-107">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="853a3-108">Wenn der Benutzer beispielsweise ein Foto mit 504x504 Pixeln hochlädt, sind alle Fotogrößen bis auf 648x648 zum Download verfügbar.</span><span class="sxs-lookup"><span data-stu-id="853a3-108">For example, if the user uploads a photo that is 504x504 pixels, then all but the 648x648 size of photo will be available for download.</span></span>
<span data-ttu-id="853a3-109">Wenn die angegebene Größe nicht im Postfach des Benutzers oder in Azure Active Directory verfügbar ist, wird die Größe „1x1“ mit den restlichen Metadaten zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="853a3-109">If the specified size is not available in the user's mailbox or in Azure Active Directory, the size of '1x1' is returned with the rest of metadata.</span></span>

## <a name="permissions"></a><span data-ttu-id="853a3-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="853a3-110">Permissions</span></span>

<span data-ttu-id="853a3-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="853a3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="853a3-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="853a3-113">Permission type</span></span>      | <span data-ttu-id="853a3-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="853a3-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="853a3-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="853a3-115">Delegated (work or school account)</span></span> | <span data-ttu-id="853a3-116">Für **user**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="853a3-116">For **user** resource:</span></span><br/><span data-ttu-id="853a3-117">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="853a3-117">Profile photo of specifically the signed-in user - User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="853a3-118">Für **group**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="853a3-118">For **group** resource:</span></span><br /><span data-ttu-id="853a3-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="853a3-119">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="853a3-120">Für **contact**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="853a3-120">For **contact** resource:</span></span><br /><span data-ttu-id="853a3-121">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="853a3-121">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="853a3-122">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="853a3-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="853a3-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="853a3-123">Not supported</span></span> |
|<span data-ttu-id="853a3-124">Anwendung</span><span class="sxs-lookup"><span data-stu-id="853a3-124">Application</span></span>                        | <span data-ttu-id="853a3-125">Für **user**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="853a3-125">For **user** resource:</span></span><br/><span data-ttu-id="853a3-126">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="853a3-126">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span><br /><br /><span data-ttu-id="853a3-127">Für **group**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="853a3-127">For **group** resource:</span></span><br /><span data-ttu-id="853a3-128">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="853a3-128">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="853a3-129">Für **contact**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="853a3-129">For **contact** resource:</span></span><br /><span data-ttu-id="853a3-130">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="853a3-130">Contacts.Read, Contacts.ReadWrite</span></span> |


## <a name="http-request-to-get-the-photo"></a><span data-ttu-id="853a3-131">HTTP-Anforderung zum Abrufen des Fotos</span><span class="sxs-lookup"><span data-stu-id="853a3-131">HTTP request to get the photo</span></span>
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
## <a name="http-request-to-get-the-metadata-of-the-photo"></a><span data-ttu-id="853a3-132">HTTP-Anforderung zum Abrufen von Metadaten des Fotos</span><span class="sxs-lookup"><span data-stu-id="853a3-132">HTTP request to get the metadata of the photo</span></span>
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

## <a name="parameters"></a><span data-ttu-id="853a3-133">Parameter</span><span class="sxs-lookup"><span data-stu-id="853a3-133">Parameters</span></span>

|<span data-ttu-id="853a3-134">**Parameter**</span><span class="sxs-lookup"><span data-stu-id="853a3-134">**Parameter**</span></span>|<span data-ttu-id="853a3-135">**Typ**</span><span class="sxs-lookup"><span data-stu-id="853a3-135">**Type**</span></span>|<span data-ttu-id="853a3-136">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="853a3-136">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="853a3-137">_URL-Parameter_</span><span class="sxs-lookup"><span data-stu-id="853a3-137">_URL parameters_</span></span>|
|<span data-ttu-id="853a3-138">size</span><span class="sxs-lookup"><span data-stu-id="853a3-138">size</span></span>  |<span data-ttu-id="853a3-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="853a3-139">String</span></span>  | <span data-ttu-id="853a3-140">Eine Fotogröße.</span><span class="sxs-lookup"><span data-stu-id="853a3-140">A photo size.</span></span> <span data-ttu-id="853a3-141">Die unterstützten Größen der HD-Fotos in Office 365 sind wie folgt: „48x48“, „64x64“, „96x96“, „120x120“, „240x240“,</span><span class="sxs-lookup"><span data-stu-id="853a3-141">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> 
<span data-ttu-id="853a3-142">„360x360“, „432x432“, „504x504“ und „648x648“.</span><span class="sxs-lookup"><span data-stu-id="853a3-142">'360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="853a3-143">Fotos können eine beliebige Größe aufweisen, wenn sie in Azure Active Directory gespeichert sind.</span><span class="sxs-lookup"><span data-stu-id="853a3-143">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="853a3-144">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="853a3-144">Optional query parameters</span></span>
<span data-ttu-id="853a3-145">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="853a3-145">This method supports the [OData Query Parameters](http://developer.microsoft.com/de-DE/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="853a3-146">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="853a3-146">Request headers</span></span>
| <span data-ttu-id="853a3-147">Name</span><span class="sxs-lookup"><span data-stu-id="853a3-147">Name</span></span>       | <span data-ttu-id="853a3-148">Typ</span><span class="sxs-lookup"><span data-stu-id="853a3-148">Type</span></span> | <span data-ttu-id="853a3-149">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="853a3-149">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="853a3-150">Authorization</span><span class="sxs-lookup"><span data-stu-id="853a3-150">Authorization</span></span>  | <span data-ttu-id="853a3-151">string</span><span class="sxs-lookup"><span data-stu-id="853a3-151">string</span></span>  | <span data-ttu-id="853a3-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="853a3-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="853a3-154">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="853a3-154">Request body</span></span>
<span data-ttu-id="853a3-155">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="853a3-155">Do not supply a request body for this method.</span></span>
## <a name="response-for-getting-the-photo"></a><span data-ttu-id="853a3-156">Antwort für Abrufen des Fotos</span><span class="sxs-lookup"><span data-stu-id="853a3-156">Response for getting the photo</span></span>
<span data-ttu-id="853a3-p107">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und binäre Daten des angeforderten Fotos zurückgegeben.  Wenn kein Foto vorhanden ist, gibt der Vorgang `404 Not Found` zurück.</span><span class="sxs-lookup"><span data-stu-id="853a3-p107">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
## <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="853a3-159">Antwort für Abrufen der Metadaten des Fotos</span><span class="sxs-lookup"><span data-stu-id="853a3-159">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="853a3-160">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [profilePhoto](../resources/profilePhoto.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="853a3-160">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilePhoto.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="853a3-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="853a3-161">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="853a3-162">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="853a3-162">Request 1</span></span>
<span data-ttu-id="853a3-163">Diese Anforderung ruft das Foto des angemeldeten Benutzers mit der größten verfügbaren Größe ab.</span><span class="sxs-lookup"><span data-stu-id="853a3-163">This request gets the photo for the signed-in user, in the largest available size.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response-1"></a><span data-ttu-id="853a3-164">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="853a3-164">Response 1</span></span>
<span data-ttu-id="853a3-p108">Enthält die binären Daten des angeforderten Fotos. Der HTTP-Antwortcode ist 200.</span><span class="sxs-lookup"><span data-stu-id="853a3-p108">Contains the binary data of the requested photo. The HTTP response code is 200.</span></span>

##### <a name="request-2"></a><span data-ttu-id="853a3-167">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="853a3-167">Request 2</span></span>
<span data-ttu-id="853a3-168">Diese Anforderung ruft das 48x48-Foto für den angemeldeten Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="853a3-168">This request gets the 48x48 photo for the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response-2"></a><span data-ttu-id="853a3-169">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="853a3-169">Response 2</span></span>
<span data-ttu-id="853a3-p109">Enthält die binären Daten des angeforderten 48x48-Fotos. Der HTTP-Antwortcode ist 200.</span><span class="sxs-lookup"><span data-stu-id="853a3-p109">Contains the binary data of the requested 48x48 photo. The HTTP response code is 200.</span></span>

##### <a name="request-3"></a><span data-ttu-id="853a3-172">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="853a3-172">Request 3</span></span>
<span data-ttu-id="853a3-173">Diese Anforderung ruft die Metadaten des Benutzerfotos des angemeldeten Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="853a3-173">This request gets the metadata of the user photo of the signed-in user.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response-3"></a><span data-ttu-id="853a3-174">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="853a3-174">Response 3</span></span>

<span data-ttu-id="853a3-p110">Die folgenden Antwortdaten zeigen die Metadaten des Fotos. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="853a3-p110">The following response data shows the photo metadata. Note: The response object shown here may be truncated for brevity.</span></span>
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

<span data-ttu-id="853a3-p111">Die folgenden Antwortdaten zeigen die Inhalte einer Antwort, wenn für den Benutzer noch kein Foto hochgeladen wurde. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="853a3-p111">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user. Note: The response object shown here may be truncated for brevity.</span></span>

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
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="853a3-179">Verwenden der Binärdaten des angeforderten Fotos</span><span class="sxs-lookup"><span data-stu-id="853a3-179">Using the binary data of the requested photo</span></span>

<span data-ttu-id="853a3-180">Wenn Sie den `/photo/$value`-Endpunkt zum Abrufen der Binärdaten für ein Profilfoto verwenden, müssen Sie die Daten in eine Base-64-Zeichenfolge konvertieren, damit sie als E-Mail-Anlage hinzugefügt werden können.</span><span class="sxs-lookup"><span data-stu-id="853a3-180">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="853a3-181">Das folgende Beispiel in JavaScript zeigt das Erstellen eines Arrays, das Sie als Wert des `Attachments`-Parameters einer [Outlook-Nachricht](user_post_messages.md) übergeben können.</span><span class="sxs-lookup"><span data-stu-id="853a3-181">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user_post_messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="853a3-182">Unter [Microsoft Graph Connect-Beispiel für Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) finden Sie eine Implementierung dieses Beispiels.</span><span class="sxs-lookup"><span data-stu-id="853a3-182">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="853a3-183">Wenn Sie das Bild auf einer Webseite anzeigen möchten, erstellen Sie ein Objekt im Arbeitsspeicher aus dem Bild, und verwenden Sie das Objekt als Quelle eines Bildelements.</span><span class="sxs-lookup"><span data-stu-id="853a3-183">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="853a3-184">Hier ist ein Beispiel in JavaScript für diesen Vorgang.</span><span class="sxs-lookup"><span data-stu-id="853a3-184">Here is an example in JavaScript of this operation.</span></span>

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
