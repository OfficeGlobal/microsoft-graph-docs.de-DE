---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Kleine Dateien hochladen
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 59036213350b3efa5c22fd277328176999bbbc11
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481510"
---
# <a name="upload-or-replace-the-contents-of-a-driveitem"></a><span data-ttu-id="46cbf-102">Inhalte eines DriveItem hochladen oder ersetzen</span><span class="sxs-lookup"><span data-stu-id="46cbf-102">Upload or replace the contents of a DriveItem</span></span>

<span data-ttu-id="46cbf-p101">Mit der einfachen Upload-API können Sie den Inhalt einer neuen Datei bereitstellen oder den Inhalt einer vorhandenen Datei in einem einzigen API-Aufruf aktualisieren . Diese Methode unterstützt nur Dateien, die bis zu 4MB groß sind.</span><span class="sxs-lookup"><span data-stu-id="46cbf-p101">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

<span data-ttu-id="46cbf-105">Informationen zum Hochladen großer Dateien finden Sie unter [Große Dateien mit einer Uploadsitzung hochladen](driveitem-createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="46cbf-105">To upload large files see [Upload large files with an upload session](driveitem-createuploadsession.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="46cbf-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="46cbf-106">Permissions</span></span>

<span data-ttu-id="46cbf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46cbf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46cbf-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="46cbf-109">Permission type</span></span>      | <span data-ttu-id="46cbf-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="46cbf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46cbf-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="46cbf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="46cbf-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46cbf-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="46cbf-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="46cbf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46cbf-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46cbf-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="46cbf-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="46cbf-115">Application</span></span> | <span data-ttu-id="46cbf-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46cbf-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request-to-replace-an-existing-item"></a><span data-ttu-id="46cbf-117">HTTP-Anforderung (um ein vorhandenes Element zu ersetzen)</span><span class="sxs-lookup"><span data-stu-id="46cbf-117">HTTP request (to replace an existing item)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{item-id}/content
PUT /groups/{group-id}/drive/items/{item-id}/content
PUT /me/drive/items/{item-id}/content
PUT /sites/{site-id}/drive/items/{item-id}/content
PUT /users/{user-id}/drive/items/{item-id}/content
```

## <a name="http-request-to-upload-a-new-file"></a><span data-ttu-id="46cbf-118">HTTP-Anforderung (um eine neue Datei hochzuladen)</span><span class="sxs-lookup"><span data-stu-id="46cbf-118">HTTP request (to upload a new file)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{parent-id}:/{filename}:/content
PUT /groups/{group-id}/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /sites/{site-id}/drive/items/{parent-id}:/{filename}:/content
PUT /users/{user-id}/drive/items/{parent-id}:/{filename}:/content
```

## <a name="request-body"></a><span data-ttu-id="46cbf-119">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="46cbf-119">Request body</span></span>

<span data-ttu-id="46cbf-120">Der Inhalt des Anforderungstexts sollte den binären Stream der hochzuladenden Datei sein.</span><span class="sxs-lookup"><span data-stu-id="46cbf-120">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <a name="response"></a><span data-ttu-id="46cbf-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="46cbf-121">Response</span></span>

<span data-ttu-id="46cbf-122">Wenn die Methode erfolgreich verläuft, wird ein [driveItem](../resources/driveitem.md)-Objekt im Antworttext der neu erstellten oder aktualisierten Datei zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="46cbf-122">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created or updated file.</span></span>

## <a name="example-upload-a-new-file"></a><span data-ttu-id="46cbf-123">Beispiel (Hochladen einer neuen Datei)</span><span class="sxs-lookup"><span data-stu-id="46cbf-123">Example (upload a new file)</span></span>

<span data-ttu-id="46cbf-124">In diesem Beispiel wird die Zeichenfolge "Die Inhalte der Datei hier einfügen"</span><span class="sxs-lookup"><span data-stu-id="46cbf-124">This example uploads the string "The contents of the file goes here."</span></span> <span data-ttu-id="46cbf-125">auf dem angemeldeten Benutzerlaufwerk in einer Datei mit dem Namen FileB.txt in den Ordner FolderA hochgeladen.</span><span class="sxs-lookup"><span data-stu-id="46cbf-125">to a file in the signed-in user's drive under FolderA named FileB.txt.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/root:/FolderA/FileB.txt:/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="46cbf-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="46cbf-126">Response</span></span>

<span data-ttu-id="46cbf-127">Wenn die Methode erfolgreich verläuft, wird eine [driveItem][item-resource]-Ressource im Antworttext der neu erstellten Datei zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="46cbf-127">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

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

## <a name="example-updating-an-existing-file"></a><span data-ttu-id="46cbf-128">Beispiel (Aktualisieren einer vorhandenen Datei)</span><span class="sxs-lookup"><span data-stu-id="46cbf-128">Example (updating an existing file)</span></span>

<span data-ttu-id="46cbf-129">In diesem Beispiel wird der Inhalt einer Datei durch eine bekannte ID ersetzt.</span><span class="sxs-lookup"><span data-stu-id="46cbf-129">This example replaces the contents of a file with a known ID.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put-id", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/items/{item-id}/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="46cbf-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="46cbf-130">Response</span></span>

<span data-ttu-id="46cbf-131">Wenn die Methode erfolgreich verläuft, wird eine [driveItem][item-resource]-Ressource im Antworttext der neu erstellten Datei zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="46cbf-131">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="46cbf-132">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="46cbf-132">Error responses</span></span>

<span data-ttu-id="46cbf-133">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie unter [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="46cbf-133">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new file with content or update a file's content.",
  "keywords": "insert,upsert,update,upload",
  "section": "documentation"
} -->
