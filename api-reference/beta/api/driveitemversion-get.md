---
title: DriveItemVersion-Ressource erhalten (Vorschau)
description: Rufen Sie die Metadaten für eine bestimmte Version eines DriveItem ab.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 4292f511ffde5da4b287fcb090f2102575adcb2f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984682"
---
# <a name="get-a-driveitemversion-resource-preview"></a><span data-ttu-id="d606a-103">DriveItemVersion-Ressource erhalten (Vorschau)</span><span class="sxs-lookup"><span data-stu-id="d606a-103">Get a DriveItemVersion resource (preview)</span></span>

> <span data-ttu-id="d606a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d606a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d606a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d606a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d606a-106">Rufen Sie die Metadaten für eine bestimmte Version eines [DriveItem](../resources/driveitem.md) ab.</span><span class="sxs-lookup"><span data-stu-id="d606a-106">Retrieve the metadata for a specific version of a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d606a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d606a-107">Permissions</span></span>

<span data-ttu-id="d606a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d606a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d606a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d606a-110">Permission type</span></span>      | <span data-ttu-id="d606a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d606a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d606a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d606a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d606a-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d606a-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d606a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d606a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d606a-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d606a-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d606a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d606a-116">Application</span></span> | <span data-ttu-id="d606a-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d606a-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="d606a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d606a-118">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions/{version-id}
GET /groups/{group-id}/drive/{item-id}/versions/{version-id}
GET /me/drive/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/drive/items/{item-id}/versions/{version-id}
GET /users/{user-id}/drive/items/{item-id}/versions/{version-id}
```

## <a name="response"></a><span data-ttu-id="d606a-119">Antwort</span><span class="sxs-lookup"><span data-stu-id="d606a-119">Response</span></span>

<span data-ttu-id="d606a-120">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [DriveItemVersion](../resources/driveitemversion.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d606a-120">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/driveitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="d606a-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d606a-121">Example</span></span>

<span data-ttu-id="d606a-122">In diesem Beispiel wird die Version einer Datei auf dem Laufwerk des aktuellen Benutzers abgerufen.</span><span class="sxs-lookup"><span data-stu-id="d606a-122">This example retrieves a version of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="d606a-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d606a-123">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/versions/{version-id}
```

### <a name="response"></a><span data-ttu-id="d606a-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="d606a-124">Response</span></span>

<span data-ttu-id="d606a-125">Dadurch wird eine Sammlung von Versionen zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="d606a-125">This returns a collection of versions:</span></span>

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

## <a name="remarks"></a><span data-ttu-id="d606a-126">Hinweise</span><span class="sxs-lookup"><span data-stu-id="d606a-126">Remarks</span></span>

<span data-ttu-id="d606a-127">OneDrive behält nicht die kompletten Metadaten für vorherige Versionen einer Datei bei.</span><span class="sxs-lookup"><span data-stu-id="d606a-127">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="d606a-128">Wenn Ihre App die Liste verfügbarer Versionen für eine Datei abruft, wird eine [DriveItemVersion](../resources/driveitemversion.md)-Ressource zurückgegeben, welche die verfügbaren Informationen zu der jeweiligen Version bereitstellt.</span><span class="sxs-lookup"><span data-stu-id="d606a-128">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
