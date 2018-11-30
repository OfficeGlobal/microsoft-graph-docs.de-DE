---
title: Foto abrufen
description: Rufen Sie das angegebene profilePhoto oder die Metadaten (profilePhoto-Eigenschaften) ab.
ms.openlocfilehash: 11411f3439cf0e85991bbac7d3ccf30ac535651c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016758"
---
# <a name="get-photo"></a><span data-ttu-id="ed901-103">Foto abrufen</span><span class="sxs-lookup"><span data-stu-id="ed901-103">Get photo</span></span>

<span data-ttu-id="ed901-104">Rufen Sie das angegebene [profilePhoto](../resources/profilephoto.md) oder die Metadaten (profilePhoto-Eigenschaften) ab.</span><span class="sxs-lookup"><span data-stu-id="ed901-104">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (profilePhoto properties).</span></span>

> <span data-ttu-id="ed901-105">**Hinweis:** Dieser Vorgang in Version 1.0 unterstützt ausschließlich Postfächer in Geschäfts-, Schul- oder Unikonten des Benutzers. Persönliche Postfächer werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ed901-105">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

<span data-ttu-id="ed901-106">Die unterstützten Größen der HD-Fotos in Office 365 sind wie folgt: „48x48“, „64x64“, „96x96“, „120x120“, „240x240“, „360x360“,“432x432“, „504x504“ und „648x648“.</span><span class="sxs-lookup"><span data-stu-id="ed901-106">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="ed901-107">Fotos können eine beliebige Größe aufweisen, wenn sie in Azure Active Directory gespeichert sind.</span><span class="sxs-lookup"><span data-stu-id="ed901-107">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="ed901-108">Sie können die Metadaten des größten verfügbaren Fotos abrufen oder eine Größe angeben, um die Metadaten für diese Fotogröße abzurufen.</span><span class="sxs-lookup"><span data-stu-id="ed901-108">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="ed901-109">Wenn die angeforderte Größe nicht verfügbar ist, können Sie immer noch eine kleinere Größe abrufen, die der Benutzer hochgeladen und zur Verfügung gestellt hat.</span><span class="sxs-lookup"><span data-stu-id="ed901-109">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="ed901-110">Wenn der Benutzer beispielsweise ein Foto mit 504x504 Pixeln hochlädt, sind alle Fotogrößen bis auf 648x648 zum Download verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ed901-110">For example, if the user uploads a photo that is 504x504 pixels, then all but the 648x648 size of photo will be available for download.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed901-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ed901-111">Permissions</span></span>

<span data-ttu-id="ed901-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed901-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed901-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ed901-114">Permission type</span></span>      | <span data-ttu-id="ed901-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ed901-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed901-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ed901-116">Delegated (work or school account)</span></span> | <span data-ttu-id="ed901-117">Für **user**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="ed901-117">For **user** resource:</span></span><br/><span data-ttu-id="ed901-118">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed901-118">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="ed901-119">Für **group**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="ed901-119">For **group** resource:</span></span><br /><span data-ttu-id="ed901-120">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed901-120">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="ed901-121">Für **contact**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="ed901-121">For **contact** resource:</span></span><br /><span data-ttu-id="ed901-122">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed901-122">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="ed901-123">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ed901-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed901-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed901-124">Not supported</span></span> |
|<span data-ttu-id="ed901-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ed901-125">Application</span></span>                        | <span data-ttu-id="ed901-126">Für **user**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="ed901-126">For **user** resource:</span></span><br/><span data-ttu-id="ed901-127">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed901-127">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="ed901-128">Für **group**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="ed901-128">For **group** resource:</span></span><br /><span data-ttu-id="ed901-129">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed901-129">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="ed901-130">Für **contact**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="ed901-130">For **contact** resource:</span></span><br /><span data-ttu-id="ed901-131">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed901-131">Contacts.Read, Contacts.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="ed901-132">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed901-132">HTTP request</span></span> 

### <a name="get-the-photo"></a><span data-ttu-id="ed901-133">Möchten Sie das Foto</span><span class="sxs-lookup"><span data-stu-id="ed901-133">Get the photo</span></span>
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
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="ed901-134">Abrufen der Metadaten des Fotos</span><span class="sxs-lookup"><span data-stu-id="ed901-134">Get the metadata of the photo</span></span>
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

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="ed901-135">Abrufen der Metadaten für eine bestimmte Fotogröße</span><span class="sxs-lookup"><span data-stu-id="ed901-135">Get the metadata for a specific photo size</span></span>
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

## <a name="path-parameters"></a><span data-ttu-id="ed901-136">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="ed901-136">Path parameters</span></span>

|<span data-ttu-id="ed901-137">Parameter</span><span class="sxs-lookup"><span data-stu-id="ed901-137">Parameter</span></span>|<span data-ttu-id="ed901-138">Typ</span><span class="sxs-lookup"><span data-stu-id="ed901-138">Type</span></span>|<span data-ttu-id="ed901-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ed901-139">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ed901-140">size</span><span class="sxs-lookup"><span data-stu-id="ed901-140">size</span></span>  |<span data-ttu-id="ed901-141">String</span><span class="sxs-lookup"><span data-stu-id="ed901-141">String</span></span>  | <span data-ttu-id="ed901-142">Eine Fotogröße.</span><span class="sxs-lookup"><span data-stu-id="ed901-142">A photo size.</span></span> <span data-ttu-id="ed901-143">Die unterstützten Größen der HD-Fotos in Office 365 sind wie folgt: „48x48“, „64x64“, „96x96“, „120x120“, „240x240“, „360x360“,“432x432“, „504x504“ und „648x648“.</span><span class="sxs-lookup"><span data-stu-id="ed901-143">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="ed901-144">Fotos können eine beliebige Größe aufweisen, wenn sie in Azure Active Directory gespeichert sind.</span><span class="sxs-lookup"><span data-stu-id="ed901-144">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="ed901-145">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ed901-145">Optional query parameters</span></span>
<span data-ttu-id="ed901-146">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ed901-146">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed901-147">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ed901-147">Request headers</span></span>
| <span data-ttu-id="ed901-148">Name</span><span class="sxs-lookup"><span data-stu-id="ed901-148">Name</span></span>       | <span data-ttu-id="ed901-149">Typ</span><span class="sxs-lookup"><span data-stu-id="ed901-149">Type</span></span> | <span data-ttu-id="ed901-150">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ed901-150">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ed901-151">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed901-151">Authorization</span></span>  | <span data-ttu-id="ed901-152">string</span><span class="sxs-lookup"><span data-stu-id="ed901-152">string</span></span>  | <span data-ttu-id="ed901-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ed901-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed901-155">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ed901-155">Request body</span></span>
<span data-ttu-id="ed901-156">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ed901-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed901-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed901-157">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="ed901-158">Antwort für Abrufen des Fotos</span><span class="sxs-lookup"><span data-stu-id="ed901-158">Response for getting the photo</span></span>
<span data-ttu-id="ed901-p106">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und binäre Daten des angeforderten Fotos zurückgegeben.  Wenn kein Foto vorhanden ist, gibt der Vorgang `404 Not Found` zurück.</span><span class="sxs-lookup"><span data-stu-id="ed901-p106">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="ed901-161">Antwort für Abrufen der Metadaten des Fotos</span><span class="sxs-lookup"><span data-stu-id="ed901-161">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="ed901-162">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [profilePhoto](../resources/profilephoto.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ed901-162">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilephoto.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ed901-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ed901-163">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="ed901-164">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="ed901-164">Request 1</span></span>
<span data-ttu-id="ed901-165">Diese Anforderung ruft das Foto des angemeldeten Benutzers mit der größten verfügbaren Größe ab.</span><span class="sxs-lookup"><span data-stu-id="ed901-165">This request gets the photo for the signed-in user, in the largest available size.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response-1"></a><span data-ttu-id="ed901-166">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="ed901-166">Response 1</span></span>
<span data-ttu-id="ed901-p107">Enthält die binären Daten des angeforderten Fotos. Der HTTP-Antwortcode ist 200.</span><span class="sxs-lookup"><span data-stu-id="ed901-p107">Contains the binary data of the requested photo. The HTTP response code is 200.</span></span>

##### <a name="request-2"></a><span data-ttu-id="ed901-169">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="ed901-169">Request 2</span></span>
<span data-ttu-id="ed901-170">Diese Anforderung ruft das 48x48-Foto für den angemeldeten Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="ed901-170">This request gets the 48x48 photo for the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response-2"></a><span data-ttu-id="ed901-171">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="ed901-171">Response 2</span></span>
<span data-ttu-id="ed901-p108">Enthält die binären Daten des angeforderten 48x48-Fotos. Der HTTP-Antwortcode ist 200.</span><span class="sxs-lookup"><span data-stu-id="ed901-p108">Contains the binary data of the requested 48x48 photo. The HTTP response code is 200.</span></span>

##### <a name="request-3"></a><span data-ttu-id="ed901-174">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="ed901-174">Request 3</span></span>
<span data-ttu-id="ed901-175">Diese Anforderung ruft die Metadaten des Benutzerfotos des angemeldeten Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="ed901-175">This request gets the metadata of the user photo of the signed-in user.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response-3"></a><span data-ttu-id="ed901-176">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="ed901-176">Response 3</span></span>

<span data-ttu-id="ed901-p109">Die folgenden Antwortdaten zeigen die Metadaten des Fotos. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="ed901-p109">The following response data shows the photo metadata. Note: The response object shown here may be truncated for brevity.</span></span>
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

<span data-ttu-id="ed901-p110">Die folgenden Antwortdaten zeigen die Inhalte einer Antwort, wenn für den Benutzer noch kein Foto hochgeladen wurde. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="ed901-p110">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user. Note: The response object shown here may be truncated for brevity.</span></span>

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
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="ed901-181">Verwenden der Binärdaten des angeforderten Fotos</span><span class="sxs-lookup"><span data-stu-id="ed901-181">Using the binary data of the requested photo</span></span>

<span data-ttu-id="ed901-182">Wenn Sie den `/photo/$value`-Endpunkt zum Abrufen der Binärdaten für ein Profilfoto verwenden, müssen Sie die Daten in eine Base-64-Zeichenfolge konvertieren, damit sie als E-Mail-Anlage hinzugefügt werden können.</span><span class="sxs-lookup"><span data-stu-id="ed901-182">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="ed901-183">Das folgende Beispiel in JavaScript zeigt das Erstellen eines Arrays, das Sie als Wert des `Attachments`-Parameters einer [Outlook-Nachricht](user-post-messages.md) übergeben können.</span><span class="sxs-lookup"><span data-stu-id="ed901-183">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user-post-messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="ed901-184">Unter [Microsoft Graph Connect-Beispiel für Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) finden Sie eine Implementierung dieses Beispiels.</span><span class="sxs-lookup"><span data-stu-id="ed901-184">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="ed901-185">Wenn Sie das Bild auf einer Webseite anzeigen möchten, erstellen Sie ein Objekt im Arbeitsspeicher aus dem Bild, und verwenden Sie das Objekt als Quelle eines Bildelements.</span><span class="sxs-lookup"><span data-stu-id="ed901-185">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="ed901-186">Hier ist ein Beispiel in JavaScript für diesen Vorgang.</span><span class="sxs-lookup"><span data-stu-id="ed901-186">Here is an example in JavaScript of this operation.</span></span>

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
