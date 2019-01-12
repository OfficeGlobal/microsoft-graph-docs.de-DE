---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Herunterladen von einer vorherigen version
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b0d8125f86459caa0fd9fd863a1a4f280e0ad89e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980111"
---
# <a name="download-contents-of-a-driveitemversion-resource-preview"></a><span data-ttu-id="e39a3-102">Inhalte einer DriveItemVersion-Ressource herunterladen (Vorschau)</span><span class="sxs-lookup"><span data-stu-id="e39a3-102">Download contents of a DriveItemVersion resource (preview)</span></span>

> <span data-ttu-id="e39a3-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e39a3-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e39a3-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e39a3-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e39a3-105">Rufen Sie den Inhalt einer bestimmten Version von einer [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e39a3-105">Retrieve the contents of a specific version of a [driveItem](../resources/driveitem.md).</span></span> 

><span data-ttu-id="e39a3-106">**Hinweis:** Abrufen des Inhalts der aktuellen Version wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e39a3-106">**Note:** Getting the content of the current version is not supported.</span></span> <span data-ttu-id="e39a3-107">Verwenden Sie stattdessen den [DriveItem Webinhalt-Endpunkt](driveitem-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="e39a3-107">Instead, use the [driveItem content endpoint](driveitem-get-content.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e39a3-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e39a3-108">Permissions</span></span>

<span data-ttu-id="e39a3-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e39a3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e39a3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e39a3-111">Permission type</span></span>      | <span data-ttu-id="e39a3-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e39a3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e39a3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e39a3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e39a3-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e39a3-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e39a3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e39a3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e39a3-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e39a3-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e39a3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e39a3-117">Application</span></span> | <span data-ttu-id="e39a3-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e39a3-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="e39a3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e39a3-119">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}/content
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}/content
GET /me/drive/items/{item-id}/versions/{version-id}/content
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}/content
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}/content
```

## <a name="response"></a><span data-ttu-id="e39a3-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="e39a3-120">Response</span></span>

<span data-ttu-id="e39a3-121">Die Methode gibt eine Antwort `302 Found` zurück, die auf eine vorab authentifizierte URL zum Download der Bytes der Datei umleitet.</span><span class="sxs-lookup"><span data-stu-id="e39a3-121">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the bytes of the file.</span></span>

<span data-ttu-id="e39a3-p104">Zum Herunterladen der Inhalte der Datei muss die Anwendung dem `Location`-Header in der Antwort folgen. Viele HTTP-Clientbibliotheken folgen automatisch der 302-Umleitung und beginnen sofort mit dem Download der Datei.</span><span class="sxs-lookup"><span data-stu-id="e39a3-p104">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="e39a3-124">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header für den Download.</span><span class="sxs-lookup"><span data-stu-id="e39a3-124">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

## <a name="example"></a><span data-ttu-id="e39a3-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e39a3-125">Example</span></span>

<span data-ttu-id="e39a3-126">In diesem Beispiel wird die Version einer Datei auf dem Laufwerk des aktuellen Benutzers abgerufen.</span><span class="sxs-lookup"><span data-stu-id="e39a3-126">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="request"></a><span data-ttu-id="e39a3-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e39a3-127">Request</span></span>

<!-- { "blockType": "request", "name": "get-version-contents", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}/content
```

### <a name="response"></a><span data-ttu-id="e39a3-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="e39a3-128">Response</span></span>

<span data-ttu-id="e39a3-129">Diese Methode gibt eine Umleitung zurück, über die der Inhalt der Version heruntergeladen werden kann.</span><span class="sxs-lookup"><span data-stu-id="e39a3-129">This returns a redirect to where the contents of the version can be downloaded.</span></span>

<!-- { "blockType": "response", "isEmpty": true  } -->

```http
HTTP/1.1 302 Redirect
Location: https://onedrive.com/34FF49D6...
```


## <a name="remarks"></a><span data-ttu-id="e39a3-130">Hinweise</span><span class="sxs-lookup"><span data-stu-id="e39a3-130">Remarks</span></span>

<span data-ttu-id="e39a3-131">OneDrive behält nicht die kompletten Metadaten für vorherige Versionen einer Datei bei.</span><span class="sxs-lookup"><span data-stu-id="e39a3-131">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="e39a3-132">Wenn Ihre app die Liste der verfügbaren Versionen für eine Datei abruft, wird eine [DriveItemVersion](../resources/driveitemversion.md) Ressource, die die verfügbare Informationen über die spezielle Version enthält zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e39a3-132">When your app retrieves the list of available versions for a file, a [driveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
