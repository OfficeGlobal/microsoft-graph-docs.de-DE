---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Kleine Dateien hochladen
ms.openlocfilehash: 44d3d3033014067af968720d24e87ec5047416ae
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="upload-or-replace-the-contents-of-a-driveitem"></a><span data-ttu-id="aebbe-102">Inhalte eines DriveItem hochladen oder ersetzen</span><span class="sxs-lookup"><span data-stu-id="aebbe-102">Upload or replace the contents of a driveItem</span></span>

<span data-ttu-id="aebbe-p101">Mit der einfachen Upload-API können Sie den Inhalt einer neuen Datei bereitstellen oder den Inhalt einer vorhandenen Datei in einem einzigen API-Aufruf aktualisieren . Diese Methode unterstützt nur Dateien, die bis zu 4MB groß sind.</span><span class="sxs-lookup"><span data-stu-id="aebbe-p101">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

<span data-ttu-id="aebbe-105">Informationen zum Hochladen großer Dateien finden Sie unter [Große Dateien mit einer Uploadsitzung hochladen](driveitem_createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="aebbe-105">To upload large files see [Upload large files with an upload session](driveitem_createuploadsession.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="aebbe-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="aebbe-106">Permissions</span></span>

<span data-ttu-id="aebbe-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aebbe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aebbe-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aebbe-109">Permission type</span></span>      | <span data-ttu-id="aebbe-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aebbe-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aebbe-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aebbe-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aebbe-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aebbe-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="aebbe-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aebbe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aebbe-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aebbe-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="aebbe-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aebbe-115">Application</span></span> | <span data-ttu-id="aebbe-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aebbe-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request-to-replace-an-existing-item"></a><span data-ttu-id="aebbe-117">HTTP-Anforderung (um ein vorhandenes Element zu ersetzen)</span><span class="sxs-lookup"><span data-stu-id="aebbe-117">HTTP request (to replace an existing item)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{item-id}/content
PUT /groups/{group-id}/drive/items/{item-id}/content
PUT /me/drive/items/{item-id}/content
PUT /sites/{site-id}/drive/items/{item-id}/content
PUT /users/{user-id}/drive/items/{item-id}/content
```

## <a name="http-request-to-upload-a-new-file"></a><span data-ttu-id="aebbe-118">HTTP-Anforderung (um eine neue Datei hochzuladen)</span><span class="sxs-lookup"><span data-stu-id="aebbe-118">HTTP request (to upload a new file)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{parent-id}:/{filename}:/content
PUT /groups/{group-id}/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /sites/{site-id}/drive/items/{parent-id}:/{filename}:/content
PUT /users/{user-id}/drive/items/{parent-id}:/{filename}:/content
```

## <a name="request-body"></a><span data-ttu-id="aebbe-119">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aebbe-119">Request body</span></span>

<span data-ttu-id="aebbe-120">Der Inhalt des Anforderungstexts sollte den binären Stream der hochzuladenden Datei sein.</span><span class="sxs-lookup"><span data-stu-id="aebbe-120">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <a name="response"></a><span data-ttu-id="aebbe-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="aebbe-121">Response</span></span>

<span data-ttu-id="aebbe-122">Wenn die Methode erfolgreich verläuft, wird ein [driveItem](../resources/driveitem.md)-Objekt im Antworttext der neu erstellten oder aktualisierten Datei zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aebbe-122">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created file.</span></span>

## <a name="example-upload-a-new-file"></a><span data-ttu-id="aebbe-123">Beispiel (Hochladen einer neuen Datei)</span><span class="sxs-lookup"><span data-stu-id="aebbe-123">Example (upload a new file)</span></span>

<span data-ttu-id="aebbe-124">In diesem Beispiel wird die Zeichenfolge "Die Inhalte der Datei hier einfügen"</span><span class="sxs-lookup"><span data-stu-id="aebbe-124">This example uploads the string "The contents of the file goes here."</span></span> <span data-ttu-id="aebbe-125">auf dem angemeldeten Benutzerlaufwerk in einer Datei mit dem Namen FileB.txt in den Ordner FolderA hochgeladen.</span><span class="sxs-lookup"><span data-stu-id="aebbe-125">to a file in the signed-in user's drive under FolderA named FileB.txt.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/root:/FolderA/FileB.txt:/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="aebbe-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="aebbe-126">Response</span></span>

<span data-ttu-id="aebbe-127">Wenn die Methode erfolgreich verläuft, wird eine [driveItem][item-resource]-Ressource im Antworttext der neu erstellten Datei zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aebbe-127">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "FileB.txt",
  "size": 35,
  "file": { }
}
```

## <a name="example-updating-an-existing-file"></a><span data-ttu-id="aebbe-128">Beispiel (Aktualisieren einer vorhandenen Datei)</span><span class="sxs-lookup"><span data-stu-id="aebbe-128">Example (updating an existing file)</span></span>

<span data-ttu-id="aebbe-129">In diesem Beispiel wird der Inhalt einer Datei durch eine bekannte ID ersetzt.</span><span class="sxs-lookup"><span data-stu-id="aebbe-129">This example replaces the contents of a file with a known ID.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put-id", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/items/{item-id}/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="aebbe-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="aebbe-130">Response</span></span>

<span data-ttu-id="aebbe-131">Wenn die Methode erfolgreich verläuft, wird eine [driveItem][item-resource]-Ressource im Antworttext der neu erstellten Datei zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aebbe-131">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "FileB.txt",
  "size": 35,
  "file": { }
}
```

## <a name="error-responses"></a><span data-ttu-id="aebbe-132">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="aebbe-132">Error responses</span></span>

<span data-ttu-id="aebbe-133">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie unter [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="aebbe-133">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: ../../../concepts/errors.md
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new file with content or update a file's content.",
  "keywords": "insert,upsert,update,upload",
  "section": "documentation"
} -->
