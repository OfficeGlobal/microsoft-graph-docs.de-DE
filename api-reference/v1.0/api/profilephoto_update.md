# <a name="update-profilephoto"></a><span data-ttu-id="662e3-101">profilephoto aktualisieren</span><span class="sxs-lookup"><span data-stu-id="662e3-101">Update profilephoto</span></span>

<span data-ttu-id="662e3-p101">Aktualisieren Sie das Foto für den angemeldeten **Benutzer**, die angegebene **Gruppe** oder den angegebenen **Kontakt**. Da es derzeit eine Beschränkung von 4 MB für die Gesamtgröße jeder REST-Anforderung gibt, wird hierdurch die Größe des Fotos, das Sie hinzufügen können, auf unter 4 MB beschränkt.</span><span class="sxs-lookup"><span data-stu-id="662e3-p101">Update the photo for the signed-in **user**, or the specified **group** or **contact**. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="662e3-104">In Version 1.0 können Sie PATCH oder PUT für diesen Vorgang verwenden.</span><span class="sxs-lookup"><span data-stu-id="662e3-104">You can use either PATCH or PUT for this operation in version 1.0.</span></span>

> <span data-ttu-id="662e3-105">**Hinweis:** Dieser Vorgang in Version 1.0 unterstützt ausschließlich Postfächer in Geschäfts-, Schul- oder Unikonten des Benutzers. Persönliche Postfächer werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="662e3-105">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="662e3-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="662e3-106">Permissions</span></span>
<span data-ttu-id="662e3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="662e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="662e3-109">Profilfoto des angemeldeten **Benutzers**: User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="662e3-109">Profile photo of specifically the signed-in user - User.ReadWrite, User.ReadWrite.All</span></span>
- <span data-ttu-id="662e3-110">Profilfoto einer **Gruppe**: Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="662e3-110">Profile photo of a **group** - Group.ReadWrite.All</span></span>
- <span data-ttu-id="662e3-111">Foto eines **Kontakts**: Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="662e3-111">Photo of a **contact** - Contacts.ReadWrite</span></span>

> <span data-ttu-id="662e3-p103">**Hinweis** Um das Foto eines Benutzers in der Organisation zu aktualisieren, muss Ihre App über die User.ReadWrite.All-Anwendungsberechtigung verfügen und diese API unter ihrer eigenen Identität und nicht im Auftrag eines Benutzers aufrufen. Weitere Informationen hierzu finden Sie unter [Zugriff ohne einen angemeldeten Benutzer erlangen](../../../concepts/auth_v2_service.md).</span><span class="sxs-lookup"><span data-stu-id="662e3-p103">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user. To learn more, see [get access without a signed-in user](../../../concepts/auth_v2_service.md).</span></span>

## <a name="http-request-to-update-the-photo"></a><span data-ttu-id="662e3-114">HTTP-Anforderung zum Aktualisieren des Fotos</span><span class="sxs-lookup"><span data-stu-id="662e3-114">HTTP request to update the photo</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/photo/$value
PATCH /users/{id | userPrincipalName}/photo/$value
PATCH /groups/{id}/photo/$value
PATCH /me/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PATCH /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value

PUT /me/photo/$value
PUT /users/{id | userPrincipalName}/photo/$value
PUT /groups/{id}/photo/$value
PUT /me/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
## <a name="request-headers"></a><span data-ttu-id="662e3-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="662e3-115">Request headers</span></span>
| <span data-ttu-id="662e3-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="662e3-116">Header</span></span>       | <span data-ttu-id="662e3-117">Wert</span><span class="sxs-lookup"><span data-stu-id="662e3-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="662e3-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="662e3-118">Authorization</span></span>  | <span data-ttu-id="662e3-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="662e3-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="662e3-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="662e3-121">Content-Type</span></span>  | <span data-ttu-id="662e3-p105">image/jpeg. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="662e3-p105">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="662e3-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="662e3-124">Request body</span></span>
<span data-ttu-id="662e3-125">Fügen Sie in den Anforderungstext die Binärdaten des Fotos ein.</span><span class="sxs-lookup"><span data-stu-id="662e3-125">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="662e3-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="662e3-126">Response</span></span>

<span data-ttu-id="662e3-127">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="662e3-127">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="662e3-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="662e3-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="662e3-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="662e3-129">Request</span></span>
<span data-ttu-id="662e3-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="662e3-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/v1.0/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
##### <a name="response"></a><span data-ttu-id="662e3-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="662e3-131">Response</span></span>
<span data-ttu-id="662e3-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="662e3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update profilephoto",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
