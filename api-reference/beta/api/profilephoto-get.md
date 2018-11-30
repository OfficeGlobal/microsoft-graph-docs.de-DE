---
title: Foto abrufen
description: Rufen Sie die angegebenen ProfilePhoto oder der Metadaten (**ProfilePhoto** Eigenschaften).
ms.openlocfilehash: 6374680e37d409a89b61d3e2244b45ccb29869e7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066116"
---
# <a name="get-photo"></a><span data-ttu-id="be2bc-103">Foto abrufen</span><span class="sxs-lookup"><span data-stu-id="be2bc-103">Get photo</span></span>

> <span data-ttu-id="be2bc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="be2bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be2bc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="be2bc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="be2bc-106">Rufen Sie die angegebenen [ProfilePhoto](../resources/profilephoto.md) oder der Metadaten (**ProfilePhoto** Eigenschaften).</span><span class="sxs-lookup"><span data-stu-id="be2bc-106">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (**profilePhoto** properties).</span></span>

<span data-ttu-id="be2bc-107">Ein GET Foto Vorgang ersten Versuch zum Abrufen des angegebenen Fotos aus Office 365.</span><span class="sxs-lookup"><span data-stu-id="be2bc-107">A GET photo operation first attempt to retrieve the specified photo from Office 365.</span></span> <span data-ttu-id="be2bc-108">Wenn das Foto nicht in Office 365 verfügbar ist, versucht die API das Foto von Azure Active Directory abzurufen.</span><span class="sxs-lookup"><span data-stu-id="be2bc-108">If the photo is not available in Office 365, the API attempts to retrieve the photo from Azure Active Directory.</span></span>

<span data-ttu-id="be2bc-109">Die unterstützten Größen der HD-Fotos in Office 365 sind wie folgt: „48x48“, „64x64“, „96x96“, „120x120“, „240x240“, „360x360“,“432x432“, „504x504“ und „648x648“.</span><span class="sxs-lookup"><span data-stu-id="be2bc-109">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="be2bc-110">Fotos können eine beliebige Größe aufweisen, wenn sie in Azure Active Directory gespeichert sind.</span><span class="sxs-lookup"><span data-stu-id="be2bc-110">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="be2bc-111">Sie können die Metadaten des größten verfügbaren Fotos abrufen oder eine Größe angeben, um die Metadaten für diese Fotogröße abzurufen.</span><span class="sxs-lookup"><span data-stu-id="be2bc-111">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="be2bc-112">Wenn die angeforderte Größe nicht verfügbar ist, können Sie immer noch eine kleinere Größe abrufen, die der Benutzer hochgeladen und zur Verfügung gestellt hat.</span><span class="sxs-lookup"><span data-stu-id="be2bc-112">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="be2bc-113">Wenn der Benutzer beispielsweise ein Foto mit 504x504 Pixeln hochlädt, sind alle Fotogrößen bis auf 648x648 zum Download verfügbar.</span><span class="sxs-lookup"><span data-stu-id="be2bc-113">For example, if the user uploads a photo that is 504x504 pixels, then all but the 648x648 size of photo will be available for download.</span></span>
<span data-ttu-id="be2bc-114">Wenn die angegebene Größe nicht im Postfach des Benutzers oder in Azure Active Directory verfügbar ist, wird die Größe „1x1“ mit den restlichen Metadaten zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="be2bc-114">If the specified size is not available in the user's mailbox or in Azure Active Directory, the size of '1x1' is returned with the rest of metadata.</span></span>

## <a name="permissions"></a><span data-ttu-id="be2bc-115">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="be2bc-115">Permissions</span></span>
<span data-ttu-id="be2bc-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be2bc-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> <span data-ttu-id="be2bc-118">**Hinweis:** GET-Operation Foto in Beta unterstützt Arbeit, Schule oder persönliche Konten eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="be2bc-118">**Note:** The GET photo operation in beta supports a user's work, school, or personal accounts.</span></span> <span data-ttu-id="be2bc-119">Der GET-Foto Metadatenvorgang unterstützt jedoch nur der Benutzer Arbeit oder Schule Konten und keine persönlichen Konten.</span><span class="sxs-lookup"><span data-stu-id="be2bc-119">The GET photo metadata operation, however, supports only the user's work or school accounts and not personal accounts.</span></span>

|<span data-ttu-id="be2bc-120">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="be2bc-120">Permission type</span></span>      | <span data-ttu-id="be2bc-121">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="be2bc-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be2bc-122">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="be2bc-122">Delegated (work or school account)</span></span> | <span data-ttu-id="be2bc-123">Für **user**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="be2bc-123">For **user** resource:</span></span><br/><span data-ttu-id="be2bc-124">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be2bc-124">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="be2bc-125">Für **group**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="be2bc-125">For **group** resource:</span></span><br /><span data-ttu-id="be2bc-126">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be2bc-126">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="be2bc-127">Für **contact**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="be2bc-127">For **contact** resource:</span></span><br /><span data-ttu-id="be2bc-128">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be2bc-128">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="be2bc-129">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="be2bc-129">Delegated (personal Microsoft account)</span></span>  <br /> <span data-ttu-id="be2bc-130">**Hinweis**: Metadaten-Vorgang wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="be2bc-130">**Note**: Metadata operation is not supported.</span></span> | <span data-ttu-id="be2bc-131">Für **user**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="be2bc-131">For **user** resource:</span></span><br/><span data-ttu-id="be2bc-132">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be2bc-132">User.Read, User.ReadWrite</span></span><br /><br /><span data-ttu-id="be2bc-133">Für **contact**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="be2bc-133">For **contact** resource:</span></span><br /><span data-ttu-id="be2bc-134">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be2bc-134">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="be2bc-135">Anwendung</span><span class="sxs-lookup"><span data-stu-id="be2bc-135">Application</span></span>                        | <span data-ttu-id="be2bc-136">Für **user**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="be2bc-136">For **user** resource:</span></span><br/><span data-ttu-id="be2bc-137">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be2bc-137">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="be2bc-138">Für **group**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="be2bc-138">For **group** resource:</span></span><br /><span data-ttu-id="be2bc-139">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be2bc-139">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="be2bc-140">Für **contact**-Ressource:</span><span class="sxs-lookup"><span data-stu-id="be2bc-140">For **contact** resource:</span></span><br /><span data-ttu-id="be2bc-141">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be2bc-141">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="be2bc-142">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="be2bc-142">HTTP request</span></span> 

### <a name="get-the-photo"></a><span data-ttu-id="be2bc-143">Möchten Sie das Foto</span><span class="sxs-lookup"><span data-stu-id="be2bc-143">Get the photo</span></span>
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
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="be2bc-144">Abrufen der Metadaten des Fotos</span><span class="sxs-lookup"><span data-stu-id="be2bc-144">Get the metadata of the photo</span></span>
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

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="be2bc-145">Abrufen der Metadaten für eine bestimmte Fotogröße</span><span class="sxs-lookup"><span data-stu-id="be2bc-145">Get the metadata for a specific photo size</span></span>
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

## <a name="path-parameters"></a><span data-ttu-id="be2bc-146">Pfadparameter</span><span class="sxs-lookup"><span data-stu-id="be2bc-146">Path parameters</span></span>

|<span data-ttu-id="be2bc-147">**Parameter**</span><span class="sxs-lookup"><span data-stu-id="be2bc-147">**Parameter**</span></span>|<span data-ttu-id="be2bc-148">**Typ**</span><span class="sxs-lookup"><span data-stu-id="be2bc-148">**Type**</span></span>|<span data-ttu-id="be2bc-149">**Beschreibung**</span><span class="sxs-lookup"><span data-stu-id="be2bc-149">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="be2bc-150">size</span><span class="sxs-lookup"><span data-stu-id="be2bc-150">size</span></span>  |<span data-ttu-id="be2bc-151">String</span><span class="sxs-lookup"><span data-stu-id="be2bc-151">String</span></span>  | <span data-ttu-id="be2bc-152">Eine Fotogröße.</span><span class="sxs-lookup"><span data-stu-id="be2bc-152">A photo size.</span></span> <span data-ttu-id="be2bc-153">Die unterstützten Größen der HD-Fotos in Office 365 sind wie folgt: „48x48“, „64x64“, „96x96“, „120x120“, „240x240“, „360x360“,“432x432“, „504x504“ und „648x648“.</span><span class="sxs-lookup"><span data-stu-id="be2bc-153">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="be2bc-154">Fotos können eine beliebige Größe aufweisen, wenn sie in Azure Active Directory gespeichert sind.</span><span class="sxs-lookup"><span data-stu-id="be2bc-154">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="be2bc-155">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="be2bc-155">Optional query parameters</span></span>
<span data-ttu-id="be2bc-156">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="be2bc-156">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be2bc-157">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="be2bc-157">Request headers</span></span>
| <span data-ttu-id="be2bc-158">Name</span><span class="sxs-lookup"><span data-stu-id="be2bc-158">Name</span></span>       | <span data-ttu-id="be2bc-159">Typ</span><span class="sxs-lookup"><span data-stu-id="be2bc-159">Type</span></span> | <span data-ttu-id="be2bc-160">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="be2bc-160">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="be2bc-161">Authorization</span><span class="sxs-lookup"><span data-stu-id="be2bc-161">Authorization</span></span>  | <span data-ttu-id="be2bc-162">string</span><span class="sxs-lookup"><span data-stu-id="be2bc-162">string</span></span>  | <span data-ttu-id="be2bc-p108">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="be2bc-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be2bc-165">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="be2bc-165">Request body</span></span>
<span data-ttu-id="be2bc-166">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="be2bc-166">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be2bc-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="be2bc-167">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="be2bc-168">Antwort für Abrufen des Fotos</span><span class="sxs-lookup"><span data-stu-id="be2bc-168">Response for getting the photo</span></span>
<span data-ttu-id="be2bc-p109">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und binäre Daten des angeforderten Fotos zurückgegeben.  Wenn kein Foto vorhanden ist, gibt der Vorgang `404 Not Found` zurück.</span><span class="sxs-lookup"><span data-stu-id="be2bc-p109">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="be2bc-171">Antwort für Abrufen der Metadaten des Fotos</span><span class="sxs-lookup"><span data-stu-id="be2bc-171">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="be2bc-172">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [profilePhoto](../resources/profilephoto.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="be2bc-172">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilephoto.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be2bc-173">Beispiel</span><span class="sxs-lookup"><span data-stu-id="be2bc-173">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="be2bc-174">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="be2bc-174">Request 1</span></span>
<span data-ttu-id="be2bc-175">Diese Anforderung ruft das Foto des angemeldeten Benutzers mit der größten verfügbaren Größe ab.</span><span class="sxs-lookup"><span data-stu-id="be2bc-175">This request gets the photo for the signed-in user, in the largest available size.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo/$value
Content-Type: image/jpg
```

##### <a name="response-1"></a><span data-ttu-id="be2bc-176">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="be2bc-176">Response 1</span></span>
<span data-ttu-id="be2bc-p110">Enthält die binären Daten des angeforderten Fotos. Der HTTP-Antwortcode ist 200.</span><span class="sxs-lookup"><span data-stu-id="be2bc-p110">Contains the binary data of the requested photo. The HTTP response code is 200.</span></span>

##### <a name="request-2"></a><span data-ttu-id="be2bc-179">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="be2bc-179">Request 2</span></span>
<span data-ttu-id="be2bc-180">Diese Anforderung ruft das 48x48-Foto für den angemeldeten Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="be2bc-180">This request gets the 48x48 photo for the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response-2"></a><span data-ttu-id="be2bc-181">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="be2bc-181">Response 2</span></span>
<span data-ttu-id="be2bc-p111">Enthält die binären Daten des angeforderten 48x48-Fotos. Der HTTP-Antwortcode ist 200.</span><span class="sxs-lookup"><span data-stu-id="be2bc-p111">Contains the binary data of the requested 48x48 photo. The HTTP response code is 200.</span></span>

##### <a name="request-3"></a><span data-ttu-id="be2bc-184">Anforderung 3</span><span class="sxs-lookup"><span data-stu-id="be2bc-184">Request 3</span></span>
<span data-ttu-id="be2bc-185">Diese Anforderung ruft die Metadaten des Benutzerfotos des angemeldeten Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="be2bc-185">This request gets the metadata of the user photo of the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo
```

##### <a name="response-3"></a><span data-ttu-id="be2bc-186">Antwort 3</span><span class="sxs-lookup"><span data-stu-id="be2bc-186">Response 3</span></span>
<span data-ttu-id="be2bc-p112">Die folgenden Antwortdaten zeigen die Metadaten des Fotos. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="be2bc-p112">The following response data shows the photo metadata. Note: The response object shown here may be truncated for brevity.</span></span>

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

<span data-ttu-id="be2bc-p113">Die folgenden Antwortdaten zeigen die Inhalte einer Antwort, wenn für den Benutzer noch kein Foto hochgeladen wurde. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="be2bc-p113">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user. Note: The response object shown here may be truncated for brevity.</span></span>

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
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="be2bc-191">Verwenden der Binärdaten des angeforderten Fotos</span><span class="sxs-lookup"><span data-stu-id="be2bc-191">Using the binary data of the requested photo</span></span>

<span data-ttu-id="be2bc-192">Wenn Sie den `/photo/$value`-Endpunkt zum Abrufen der Binärdaten für ein Profilfoto verwenden, müssen Sie die Daten in eine Base-64-Zeichenfolge konvertieren, damit sie als E-Mail-Anlage hinzugefügt werden können.</span><span class="sxs-lookup"><span data-stu-id="be2bc-192">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="be2bc-193">Das folgende Beispiel in JavaScript zeigt das Erstellen eines Arrays, das Sie als Wert des `Attachments`-Parameters einer [Outlook-Nachricht](user-post-messages.md) übergeben können.</span><span class="sxs-lookup"><span data-stu-id="be2bc-193">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user-post-messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="be2bc-194">Unter [Microsoft Graph Connect-Beispiel für Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) finden Sie eine Implementierung dieses Beispiels.</span><span class="sxs-lookup"><span data-stu-id="be2bc-194">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="be2bc-195">Wenn Sie das Bild auf einer Webseite anzeigen möchten, erstellen Sie ein Objekt im Arbeitsspeicher aus dem Bild, und verwenden Sie das Objekt als Quelle eines Bildelements.</span><span class="sxs-lookup"><span data-stu-id="be2bc-195">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="be2bc-196">Hier ist ein Beispiel in JavaScript für diesen Vorgang.</span><span class="sxs-lookup"><span data-stu-id="be2bc-196">Here is an example in JavaScript of this operation.</span></span>

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
