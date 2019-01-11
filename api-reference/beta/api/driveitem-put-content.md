---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Kleine Dateien hochladen
localization_priority: Normal
ms.openlocfilehash: 3549850f66c3a46eac49b4bac8040b876fc5509b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883230"
---
# <a name="upload-or-replace-the-contents-of-a-driveitem"></a><span data-ttu-id="b65bc-102">Inhalte eines DriveItem hochladen oder ersetzen</span><span class="sxs-lookup"><span data-stu-id="b65bc-102">Upload or replace the contents of a DriveItem</span></span>

> <span data-ttu-id="b65bc-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b65bc-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b65bc-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b65bc-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b65bc-p102">Mit der einfachen Upload-API können Sie den Inhalt einer neuen Datei bereitstellen oder den Inhalt einer vorhandenen Datei in einem einzigen API-Aufruf aktualisieren . Diese Methode unterstützt nur Dateien, die bis zu 4MB groß sind.</span><span class="sxs-lookup"><span data-stu-id="b65bc-p102">The simple upload API allows you to provide the contents of a new file or update the contents of an existing file in a single API call. This method only supports files up to 4MB in size.</span></span>

<span data-ttu-id="b65bc-107">Informationen zum Hochladen großer Dateien finden Sie unter [Große Dateien mit einer Uploadsitzung hochladen](driveitem-createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="b65bc-107">To upload large files see [Upload large files with an upload session](driveitem-createuploadsession.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b65bc-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b65bc-108">Permissions</span></span>

<span data-ttu-id="b65bc-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b65bc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b65bc-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b65bc-111">Permission type</span></span>      | <span data-ttu-id="b65bc-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b65bc-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b65bc-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b65bc-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b65bc-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b65bc-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b65bc-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b65bc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b65bc-116">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b65bc-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b65bc-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b65bc-117">Application</span></span> | <span data-ttu-id="b65bc-118">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b65bc-118">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request-to-replace-an-existing-item"></a><span data-ttu-id="b65bc-119">HTTP-Anforderung (um ein vorhandenes Element zu ersetzen)</span><span class="sxs-lookup"><span data-stu-id="b65bc-119">HTTP request (to replace an existing item)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{item-id}/content
PUT /groups/{group-id}/drive/items/{item-id}/content
PUT /me/drive/items/{item-id}/content
PUT /sites/{site-id}/drive/items/{item-id}/content
PUT /users/{user-id}/drive/items/{item-id}/content
```

## <a name="http-request-to-upload-a-new-file"></a><span data-ttu-id="b65bc-120">HTTP-Anforderung (um eine neue Datei hochzuladen)</span><span class="sxs-lookup"><span data-stu-id="b65bc-120">HTTP request (to upload a new file)</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /drives/{drive-id}/items/{parent-id}:/{filename}:/content
PUT /groups/{group-id}/drive/items/{parent-id}:/{filename}:/content
PUT /me/drive/items/{parent-id}:/{filename}:/content
PUT /sites/{site-id}/drive/items/{parent-id}:/{filename}:/content
PUT /users/{user-id}/drive/items/{parent-id}:/{filename}:/content
```

## <a name="request-body"></a><span data-ttu-id="b65bc-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b65bc-121">Request body</span></span>

<span data-ttu-id="b65bc-122">Der Inhalt des Anforderungstexts sollte den binären Stream der hochzuladenden Datei sein.</span><span class="sxs-lookup"><span data-stu-id="b65bc-122">The contents of the request body should be the binary stream of the file to be uploaded.</span></span>

## <a name="response"></a><span data-ttu-id="b65bc-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="b65bc-123">Response</span></span>

<span data-ttu-id="b65bc-124">Wenn die Methode erfolgreich verläuft, wird ein [driveItem](../resources/driveitem.md)-Objekt im Antworttext der neu erstellten oder aktualisierten Datei zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b65bc-124">If successful, this method returns a [driveItem](../resources/driveitem.md) object in the response body for the newly created or updated file.</span></span>

## <a name="example-upload-a-new-file"></a><span data-ttu-id="b65bc-125">Beispiel (Hochladen einer neuen Datei)</span><span class="sxs-lookup"><span data-stu-id="b65bc-125">Example (upload a new file)</span></span>

<span data-ttu-id="b65bc-126">In diesem Beispiel wird die Zeichenfolge "Die Inhalte der Datei hier einfügen"</span><span class="sxs-lookup"><span data-stu-id="b65bc-126">This example uploads the string "The contents of the file goes here."</span></span> <span data-ttu-id="b65bc-127">auf dem angemeldeten Benutzerlaufwerk in einer Datei mit dem Namen FileB.txt in den Ordner FolderA hochgeladen.</span><span class="sxs-lookup"><span data-stu-id="b65bc-127">to a file in the signed-in user's drive under FolderA named FileB.txt.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/root:/FolderA/FileB.txt:/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="b65bc-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="b65bc-128">Response</span></span>

<span data-ttu-id="b65bc-129">Wenn die Methode erfolgreich verläuft, wird eine [driveItem][item-resource]-Ressource im Antworttext der neu erstellten Datei zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b65bc-129">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

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

## <a name="example-updating-an-existing-file"></a><span data-ttu-id="b65bc-130">Beispiel (Aktualisieren einer vorhandenen Datei)</span><span class="sxs-lookup"><span data-stu-id="b65bc-130">Example (updating an existing file)</span></span>

<span data-ttu-id="b65bc-131">In diesem Beispiel wird der Inhalt einer Datei durch eine bekannte ID ersetzt.</span><span class="sxs-lookup"><span data-stu-id="b65bc-131">This example replaces the contents of a file with a known ID.</span></span>

<!-- { "blockType": "request", "name": "upload-via-put-id", "scopes": "files.readwrite" } -->

```http
PUT /me/drive/items/{item-id}/content
Content-Type: text/plain

The contents of the file goes here.
```

### <a name="response"></a><span data-ttu-id="b65bc-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="b65bc-132">Response</span></span>

<span data-ttu-id="b65bc-133">Wenn die Methode erfolgreich verläuft, wird eine [driveItem][item-resource]-Ressource im Antworttext der neu erstellten Datei zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b65bc-133">If successful, this method returns an [driveItem][item-resource] resource in the response body for the newly created file.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="b65bc-134">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="b65bc-134">Error responses</span></span>

<span data-ttu-id="b65bc-135">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie unter [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="b65bc-135">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new file with content or update a file's content.",
  "keywords": "insert,upsert,update,upload",
  "section": "documentation"
} -->
