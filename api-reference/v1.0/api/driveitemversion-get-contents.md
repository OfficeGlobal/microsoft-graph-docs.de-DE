---
title: Herunterladen von Inhalt einer Ressource DriveItemVersion
description: Rufen Sie die Inhalte einer bestimmten DriveItem-Version ab.
ms.openlocfilehash: 3f8f7ca6202be0ac8882cc513aac178dc1ac632f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016980"
---
# <a name="download-contents-of-a-driveitemversion-resource"></a><span data-ttu-id="5de5d-103">Herunterladen von Inhalt einer Ressource DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="5de5d-103">Download contents of a DriveItemVersion resource</span></span>

<span data-ttu-id="5de5d-104">Rufen Sie die Inhalte einer bestimmten [DriveItem](../resources/driveitem.md)-Version ab.</span><span class="sxs-lookup"><span data-stu-id="5de5d-104">Retrieve the contents of a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5de5d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5de5d-105">Permissions</span></span>

<span data-ttu-id="5de5d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5de5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5de5d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5de5d-108">Permission type</span></span>      | <span data-ttu-id="5de5d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5de5d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5de5d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5de5d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5de5d-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5de5d-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="5de5d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5de5d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5de5d-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5de5d-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="5de5d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5de5d-114">Application</span></span> | <span data-ttu-id="5de5d-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5de5d-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="5de5d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5de5d-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}/content
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}/content
GET /me/drive/items/{item-id}/versions/{version-id}/content
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}/content
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}/content
```

## <a name="response"></a><span data-ttu-id="5de5d-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="5de5d-117">Response</span></span>

<span data-ttu-id="5de5d-118">Die Methode gibt eine Antwort `302 Found` zurück, die auf eine vorab authentifizierte URL zum Download der Bytes der Datei umleitet.</span><span class="sxs-lookup"><span data-stu-id="5de5d-118">Returns a `302 Found` response redirecting to a pre-authenticated download URL for the bytes of the file.</span></span>

<span data-ttu-id="5de5d-p102">Zum Herunterladen der Inhalte der Datei muss die Anwendung dem `Location`-Header in der Antwort folgen. Viele HTTP-Clientbibliotheken folgen automatisch der 302-Umleitung und beginnen sofort mit dem Download der Datei.</span><span class="sxs-lookup"><span data-stu-id="5de5d-p102">To download the contents of the file your application will need to follow the `Location` header in the response. Many HTTP client libraries will automatically follow the 302 redirection and start downloading the file immedately.</span></span>

<span data-ttu-id="5de5d-121">Zuvor authentifizierte Download-URLs sind nur für einen kurzen Zeitraum (einige Minuten) gültig und erfordern keinen `Authorization`-Header für den Download.</span><span class="sxs-lookup"><span data-stu-id="5de5d-121">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

## <a name="example"></a><span data-ttu-id="5de5d-122">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5de5d-122">Example</span></span>

<span data-ttu-id="5de5d-123">In diesem Beispiel wird die Version einer Datei auf dem Laufwerk des aktuellen Benutzers abgerufen.</span><span class="sxs-lookup"><span data-stu-id="5de5d-123">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="5de5d-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5de5d-124">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-version-contents", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}/content
```

### <a name="response"></a><span data-ttu-id="5de5d-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="5de5d-125">Response</span></span>

<span data-ttu-id="5de5d-126">Diese Methode gibt eine Umleitung zurück, über die der Inhalt der Version heruntergeladen werden kann.</span><span class="sxs-lookup"><span data-stu-id="5de5d-126">This returns a redirect to where the contents of the version can be downloaded.</span></span>

<!-- { "blockType": "response", "isEmpty": true  } -->

```http
HTTP/1.1 302 Found
Location: https://onedrive.com/34FF49D6...
```


## <a name="remarks"></a><span data-ttu-id="5de5d-127">Hinweise</span><span class="sxs-lookup"><span data-stu-id="5de5d-127">Remarks</span></span>

<span data-ttu-id="5de5d-128">OneDrive behält nicht die kompletten Metadaten für vorherige Versionen einer Datei bei.</span><span class="sxs-lookup"><span data-stu-id="5de5d-128">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="5de5d-129">Wenn Ihre App die Liste verfügbarer Versionen für eine Datei abruft, wird eine [DriveItemVersion](../resources/driveitemversion.md)-Ressource zurückgegeben, welche die verfügbaren Informationen zu der jeweiligen Version bereitstellt.</span><span class="sxs-lookup"><span data-stu-id="5de5d-129">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
