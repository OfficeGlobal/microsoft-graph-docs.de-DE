---
title: Foto abrufen
description: Rufen Sie das angegebene profilePhoto oder die Metadaten (**profilePhoto**-Eigenschaften) ab.
localization_priority: Priority
ms.openlocfilehash: 759c0ff3ac2585f43ea38963e10b001250702c56
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509630"
---
# <a name="get-photo"></a><span data-ttu-id="181a2-103">Foto abrufen</span><span class="sxs-lookup"><span data-stu-id="181a2-103">Get photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="181a2-104">Rufen Sie das angegebene [profilePhoto](../resources/profilephoto.md) oder die Metadaten (**profilePhoto**-Eigenschaften) ab.</span><span class="sxs-lookup"><span data-stu-id="181a2-104">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (**profilePhoto** properties).</span></span>

<span data-ttu-id="181a2-105">Ein erster Versuch des Vorgangs „GET photo“ zum Abrufen des angegebenen Fotos aus Office 365.</span><span class="sxs-lookup"><span data-stu-id="181a2-105">A GET photo operation first attempt to retrieve the specified photo from Office 365.</span></span> <span data-ttu-id="181a2-106">Wenn das Foto nicht in Office 365 verfügbar ist, versucht die API, das Foto aus Azure Active Directory abzurufen.</span><span class="sxs-lookup"><span data-stu-id="181a2-106">If the photo is not available in Office 365, the API attempts to retrieve the photo from Azure Active Directory.</span></span>

<span data-ttu-id="181a2-107">Die unterstützten Größen der HD-Fotos in Office 365 sind wie folgt: „48x48“, „64x64“, „96x96“, „120x120“, „240x240“, „360x360“,“432x432“, „504x504“ und „648x648“.</span><span class="sxs-lookup"><span data-stu-id="181a2-107">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="181a2-108">Fotos können eine beliebige Größe aufweisen, wenn sie in Azure Active Directory gespeichert sind.</span><span class="sxs-lookup"><span data-stu-id="181a2-108">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="181a2-109">Sie können die Metadaten des größten verfügbaren Fotos abrufen oder eine Größe angeben, um die Metadaten für diese Fotogröße abzurufen.</span><span class="sxs-lookup"><span data-stu-id="181a2-109">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="181a2-110">Wenn die angeforderte Größe nicht verfügbar ist, können Sie immer noch eine kleinere Größe abrufen, die der Benutzer hochgeladen und zur Verfügung gestellt hat.</span><span class="sxs-lookup"><span data-stu-id="181a2-110">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="181a2-111">Wenn der Benutzer beispielsweise ein Foto mit 504x504 Pixeln hochlädt, sind alle Fotogrößen bis auf 648x648 zum Download verfügbar.</span><span class="sxs-lookup"><span data-stu-id="181a2-111">For example, if the user uploads a photo that is 504x504 pixels, then all but the 648x648 size of photo will be available for download.</span></span>
<span data-ttu-id="181a2-112">Wenn die angegebene Größe nicht im Postfach des Benutzers oder in Azure Active Directory verfügbar ist, wird die Größe „1x1“ mit den restlichen Metadaten zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="181a2-112">If the specified size is not available in the user's mailbox or in Azure Active Directory, the size of '1x1' is returned with the rest of metadata.</span></span>

## <a name="permissions"></a><span data-ttu-id="181a2-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="181a2-113">Permissions</span></span>
<span data-ttu-id="181a2-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="181a2-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> <span data-ttu-id="181a2-116">**Hinweis** Der Vorgang „GET photo“ in der Betaversion unterstützt das private Konto sowie das Geschäfts- und Schulkonto eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="181a2-116">**Note:** The GET photo operation in beta supports a user's work, school, or personal accounts.</span></span> <span data-ttu-id="181a2-117">Der Vorgang „GET photo metadata“ unterstützt jedoch nur Geschäfts- oder Schulkonten eines Benutzers, keine persönlichen Konten.</span><span class="sxs-lookup"><span data-stu-id="181a2-117">The GET photo metadata operation, however, supports only the user's work or school accounts and not personal accounts.</span></span>

|<span data-ttu-id="181a2-118">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="181a2-118">Permission type</span></span>      | <span data-ttu-id="181a2-119">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="181a2-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="181a2-120">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="181a2-120">Delegated (work or school account)</span></span> | <span data-ttu-id="181a2-121">Für **user**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="181a2-121">For **user** resource:</span></span><br/><span data-ttu-id="181a2-122">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="181a2-122">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="181a2-123">Für **group**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="181a2-123">For **group** resource:</span></span><br /><span data-ttu-id="181a2-124">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="181a2-124">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="181a2-125">Für **contact**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="181a2-125">For **contact** resource:</span></span><br /><span data-ttu-id="181a2-126">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="181a2-126">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="181a2-127">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="181a2-127">Delegated (personal Microsoft account)</span></span>  <br /> <span data-ttu-id="181a2-128">**Hinweis**:Der Vorgang wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="181a2-128">**Note**: Metadata operation is not supported.</span></span> | <span data-ttu-id="181a2-129">Für **user**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="181a2-129">For **user** resource:</span></span><br/><span data-ttu-id="181a2-130">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="181a2-130">User.Read, User.ReadWrite</span></span><br /><br /><span data-ttu-id="181a2-131">Für **contact**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="181a2-131">For **contact** resource:</span></span><br /><span data-ttu-id="181a2-132">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="181a2-132">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="181a2-133">Application</span><span class="sxs-lookup"><span data-stu-id="181a2-133">Application</span></span>                        | <span data-ttu-id="181a2-134">Für **user**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="181a2-134">For **user** resource:</span></span><br/><span data-ttu-id="181a2-135">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="181a2-135">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="181a2-136">Für **group**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="181a2-136">For **group** resource:</span></span><br /><span data-ttu-id="181a2-137">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="181a2-137">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="181a2-138">Für **contact**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="181a2-138">For **contact** resource:</span></span><br /><span data-ttu-id="181a2-139">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="181a2-139">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="181a2-140">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="181a2-140">HTTP request</span></span> 

### <a name="get-the-photo"></a><span data-ttu-id="181a2-141">Abrufen des Fotos</span><span class="sxs-lookup"><span data-stu-id="181a2-141">Get the photo</span></span>
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
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="181a2-142">Abrufen von Metadaten des Fotos</span><span class="sxs-lookup"><span data-stu-id="181a2-142">Get the metadata of the photo</span></span>
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

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="181a2-143">Abrufen der Metadaten für eine bestimmte Fotogröße</span><span class="sxs-lookup"><span data-stu-id="181a2-143">Get the metadata for a specific photo size</span></span>
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

## <a name="path-parameters"></a><span data-ttu-id="181a2-144">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="181a2-144">Path parameters</span></span>

|<span data-ttu-id="181a2-145">**Parameter**</span><span class="sxs-lookup"><span data-stu-id="181a2-145">**Parameter**</span></span>|<span data-ttu-id="181a2-146">**Typ**</span><span class="sxs-lookup"><span data-stu-id="181a2-146">**Type**</span></span>|<span data-ttu-id="181a2-147">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="181a2-147">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="181a2-148">size</span><span class="sxs-lookup"><span data-stu-id="181a2-148">size</span></span>  |<span data-ttu-id="181a2-149">String</span><span class="sxs-lookup"><span data-stu-id="181a2-149">String</span></span>  | <span data-ttu-id="181a2-150">Eine Fotogröße.</span><span class="sxs-lookup"><span data-stu-id="181a2-150">A photo size.</span></span> <span data-ttu-id="181a2-151">Die unterstützten Größen der HD-Fotos in Office 365 sind wie folgt: „48x48“, „64x64“, „96x96“, „120x120“, „240x240“, „360x360“,“432x432“, „504x504“ und „648x648“.</span><span class="sxs-lookup"><span data-stu-id="181a2-151">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="181a2-152">Fotos können eine beliebige Größe aufweisen, wenn sie in Azure Active Directory gespeichert sind.</span><span class="sxs-lookup"><span data-stu-id="181a2-152">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="181a2-153">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="181a2-153">Optional query parameters</span></span>
<span data-ttu-id="181a2-154">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="181a2-154">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="181a2-155">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="181a2-155">Request headers</span></span>
| <span data-ttu-id="181a2-156">Name</span><span class="sxs-lookup"><span data-stu-id="181a2-156">Name</span></span>       | <span data-ttu-id="181a2-157">Typ</span><span class="sxs-lookup"><span data-stu-id="181a2-157">Type</span></span> | <span data-ttu-id="181a2-158">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="181a2-158">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="181a2-159">Authorization</span><span class="sxs-lookup"><span data-stu-id="181a2-159">Authorization</span></span>  | <span data-ttu-id="181a2-160">string</span><span class="sxs-lookup"><span data-stu-id="181a2-160">string</span></span>  | <span data-ttu-id="181a2-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="181a2-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="181a2-163">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="181a2-163">Request body</span></span>
<span data-ttu-id="181a2-164">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="181a2-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="181a2-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="181a2-165">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="181a2-166">Antwort für Abrufen des Fotos</span><span class="sxs-lookup"><span data-stu-id="181a2-166">Response for getting the photo</span></span>
<span data-ttu-id="181a2-p108">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und binäre Daten des angeforderten Fotos zurückgegeben.  Wenn kein Foto vorhanden ist, gibt der Vorgang `404 Not Found` zurück.</span><span class="sxs-lookup"><span data-stu-id="181a2-p108">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="181a2-169">Antwort für Abrufen der Metadaten des Fotos</span><span class="sxs-lookup"><span data-stu-id="181a2-169">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="181a2-170">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [profilePhoto](../resources/profilephoto.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="181a2-170">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilephoto.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="181a2-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="181a2-171">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="181a2-172">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="181a2-172">Request 1</span></span>
<span data-ttu-id="181a2-173">Diese Anforderung ruft das Foto des angemeldeten Benutzers mit der größten verfügbaren Größe ab.</span><span class="sxs-lookup"><span data-stu-id="181a2-173">This request gets the photo for the signed-in user, in the largest available size.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo/$value
Content-Type: image/jpg
```

##### <a name="response-1"></a><span data-ttu-id="181a2-174">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="181a2-174">Response 1</span></span>
<span data-ttu-id="181a2-p109">Enthält die binären Daten des angeforderten Fotos. Der HTTP-Antwortcode ist 200.</span><span class="sxs-lookup"><span data-stu-id="181a2-p109">Contains the binary data of the requested photo. The HTTP response code is 200.</span></span>

##### <a name="request-2"></a><span data-ttu-id="181a2-177">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="181a2-177">Request 2</span></span>
<span data-ttu-id="181a2-178">Diese Anforderung ruft das 48x48-Foto für den angemeldeten Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="181a2-178">This request gets the 48x48 photo for the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response-2"></a><span data-ttu-id="181a2-179">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="181a2-179">Response 2</span></span>
<span data-ttu-id="181a2-p110">Enthält die binären Daten des angeforderten 48x48-Fotos. Der HTTP-Antwortcode ist 200.</span><span class="sxs-lookup"><span data-stu-id="181a2-p110">Contains the binary data of the requested 48x48 photo. The HTTP response code is 200.</span></span>

##### <a name="request-3"></a><span data-ttu-id="181a2-182">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="181a2-182">Request 3</span></span>
<span data-ttu-id="181a2-183">Diese Anforderung ruft die Metadaten des Benutzerfotos des angemeldeten Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="181a2-183">This request gets the metadata of the user photo of the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo
```

##### <a name="response-3"></a><span data-ttu-id="181a2-184">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="181a2-184">Response 3</span></span>
<span data-ttu-id="181a2-p111">Die folgenden Antwortdaten zeigen die Metadaten des Fotos. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="181a2-p111">The following response data shows the photo metadata. Note: The response object shown here may be truncated for brevity.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

<span data-ttu-id="181a2-p112">Die folgenden Antwortdaten zeigen die Inhalte einer Antwort, wenn für den Benutzer noch kein Foto hochgeladen wurde. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="181a2-p112">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user. Note: The response object shown here may be truncated for brevity.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/gif",
    "@odata.mediaEtag": "",
    "id": "1X1",
    "width": 1,
    "height": 1
}
```
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="181a2-189">Verwenden der Binärdaten des angeforderten Fotos</span><span class="sxs-lookup"><span data-stu-id="181a2-189">Using the binary data of the requested photo</span></span>

<span data-ttu-id="181a2-190">Wenn Sie den `/photo/$value`-Endpunkt zum Abrufen der Binärdaten für ein Profilfoto verwenden, müssen Sie die Daten in eine Base-64-Zeichenfolge konvertieren, damit sie als E-Mail-Anlage hinzugefügt werden können.</span><span class="sxs-lookup"><span data-stu-id="181a2-190">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="181a2-191">Das folgende Beispiel in JavaScript zeigt das Erstellen eines Arrays, das Sie als Wert des `Attachments`-Parameters einer [Outlook-Nachricht](user-post-messages.md) übergeben können.</span><span class="sxs-lookup"><span data-stu-id="181a2-191">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user-post-messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="181a2-192">Unter [Microsoft Graph Connect-Beispiel für Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) finden Sie eine Implementierung dieses Beispiels.</span><span class="sxs-lookup"><span data-stu-id="181a2-192">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="181a2-193">Wenn Sie das Bild auf einer Webseite anzeigen möchten, erstellen Sie ein Objekt im Arbeitsspeicher aus dem Bild, und verwenden Sie das Objekt als Quelle eines Bildelements.</span><span class="sxs-lookup"><span data-stu-id="181a2-193">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="181a2-194">Hier ist ein Beispiel in JavaScript für diesen Vorgang.</span><span class="sxs-lookup"><span data-stu-id="181a2-194">Here is an example in JavaScript of this operation.</span></span>

    const url = window.URL || window.webkitURL;
    const blobUrl = url.createObjectURL(image.data);
    document.getElementById(imageElement).setAttribute("src", blobUrl);

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/profilephoto-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
