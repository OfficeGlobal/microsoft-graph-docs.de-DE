---
title: Abrufen einer Ressource DriveItemVersion
description: Rufen Sie die Metadaten für eine bestimmte Version eines DriveItem ab.
localization_priority: Normal
ms.openlocfilehash: d16e6bf6a9fa797f952109a773cfd4227696e032
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868341"
---
# <a name="get-a-driveitemversion-resource"></a><span data-ttu-id="4930d-103">Abrufen einer Ressource DriveItemVersion</span><span class="sxs-lookup"><span data-stu-id="4930d-103">Get a DriveItemVersion resource</span></span>

<span data-ttu-id="4930d-104">Rufen Sie die Metadaten für eine bestimmte Version eines [DriveItem](../resources/driveitem.md) ab.</span><span class="sxs-lookup"><span data-stu-id="4930d-104">Retrieve the metadata for a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4930d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4930d-105">Permissions</span></span>

<span data-ttu-id="4930d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4930d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4930d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4930d-108">Permission type</span></span>      | <span data-ttu-id="4930d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4930d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4930d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4930d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4930d-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4930d-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4930d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4930d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4930d-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4930d-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="4930d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4930d-114">Application</span></span> | <span data-ttu-id="4930d-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4930d-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="4930d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4930d-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}
GET /me/drive/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}
```

## <a name="response"></a><span data-ttu-id="4930d-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="4930d-117">Response</span></span>

<span data-ttu-id="4930d-118">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [DriveItemVersion](../resources/driveitemversion.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4930d-118">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/driveitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="4930d-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4930d-119">Example</span></span>

<span data-ttu-id="4930d-120">In diesem Beispiel wird die Version einer Datei auf dem Laufwerk des aktuellen Benutzers abgerufen.</span><span class="sxs-lookup"><span data-stu-id="4930d-120">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="4930d-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4930d-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}
```

### <a name="response"></a><span data-ttu-id="4930d-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="4930d-122">Response</span></span>

<span data-ttu-id="4930d-123">Dadurch wird eine Sammlung von Versionen zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="4930d-123">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "D4990684-58CE-4FAB-9B87-D6C49E74F298",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "size": 123
}
```

## <a name="remarks"></a><span data-ttu-id="4930d-124">Hinweise</span><span class="sxs-lookup"><span data-stu-id="4930d-124">Remarks</span></span>

<span data-ttu-id="4930d-125">OneDrive behält nicht die kompletten Metadaten für vorherige Versionen einer Datei bei.</span><span class="sxs-lookup"><span data-stu-id="4930d-125">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="4930d-126">Wenn Ihre App die Liste verfügbarer Versionen für eine Datei abruft, wird eine [DriveItemVersion](../resources/driveitemversion.md)-Ressource zurückgegeben, welche die verfügbaren Informationen zu der jeweiligen Version bereitstellt.</span><span class="sxs-lookup"><span data-stu-id="4930d-126">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
