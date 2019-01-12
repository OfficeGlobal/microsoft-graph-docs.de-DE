---
title: Auflisten von Versionen einer DriveItem
description: OneDrive und SharePoint können auch so konfiguriert werden, dass für Dateien ein Verlauf beibehalten wird.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: fa25734967aca0ad5c7022f147ca243530f1ac3f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932063"
---
# <a name="listing-versions-of-a-driveitem"></a><span data-ttu-id="c1e86-103">Auflisten von Versionen einer DriveItem</span><span class="sxs-lookup"><span data-stu-id="c1e86-103">Listing versions of a DriveItem</span></span>

<span data-ttu-id="c1e86-104">OneDrive und SharePoint können auch so konfiguriert werden, dass für Dateien ein Verlauf beibehalten wird.</span><span class="sxs-lookup"><span data-stu-id="c1e86-104">OneDrive and SharePoint can be configured to retain the history for files.</span></span>
<span data-ttu-id="c1e86-105">Je nach Dienst und Konfiguration kann für jede Änderung beim Speichern der Datei eine neue Version erstellt werden, manuell oder nie.</span><span class="sxs-lookup"><span data-stu-id="c1e86-105">Depending on the service and configuration, a new version can be created for each edit, each time the file is saved, manually, or never.</span></span>

<span data-ttu-id="c1e86-106">Vorherige Versionen eines Dokuments können je nach Administratoreinstellungen für einen begrenzten Zeitraum beibehalten werden, diese können pro Benutzer oder Speicherort eindeutig sein.</span><span class="sxs-lookup"><span data-stu-id="c1e86-106">Previous versions of a document may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1e86-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c1e86-107">Permissions</span></span>

<span data-ttu-id="c1e86-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1e86-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1e86-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c1e86-110">Permission type</span></span>      | <span data-ttu-id="c1e86-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c1e86-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1e86-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c1e86-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c1e86-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1e86-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c1e86-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c1e86-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1e86-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1e86-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c1e86-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c1e86-116">Application</span></span> | <span data-ttu-id="c1e86-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1e86-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="c1e86-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1e86-118">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /drives/{drive-id}/items/{item-id}/versions
GET /groups/{group-id}/drive/{item-id}/versions
GET /me/drive/items/{item-id}/versions
GET /sites/{site-id}/drive/items/{item-id}/versions
GET /users/{user-id}/drive/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="c1e86-119">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1e86-119">Response</span></span>

<span data-ttu-id="c1e86-120">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [DriveItemVersion](../resources/driveitemversion.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1e86-120">If successful, this method returns a `200 OK` response code and collection of [DriveItemVersion](../resources/driveitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="c1e86-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1e86-121">Example</span></span>

<span data-ttu-id="c1e86-122">In diesem Beispiel werden die Versionen einer Datei auf dem Laufwerk des aktuellen Benutzers abgerufen.</span><span class="sxs-lookup"><span data-stu-id="c1e86-122">This example retrieves the versions of a file in the current user's drive.</span></span>

### <a name="http-request"></a><span data-ttu-id="c1e86-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1e86-123">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="c1e86-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1e86-124">Response</span></span>

<span data-ttu-id="c1e86-125">Dadurch wird eine Sammlung von Versionen zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="c1e86-125">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItemVersion)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value":
  [
    {
      "id": "3.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
      "size": 123
    },
    {
      "id": "2.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-11T10:21:03.000Z",
      "size": 62
    },
    {
      "id": "1.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-10T15:20:01.125Z",
      "size": 16
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="c1e86-126">Hinweise</span><span class="sxs-lookup"><span data-stu-id="c1e86-126">Remarks</span></span>

<span data-ttu-id="c1e86-127">OneDrive behält nicht die kompletten Metadaten für vorherige Versionen einer Datei bei.</span><span class="sxs-lookup"><span data-stu-id="c1e86-127">OneDrive does not preserve the complete metadata for previous versions of a file.</span></span>

<span data-ttu-id="c1e86-128">Wenn Ihre App die Liste verfügbarer Versionen für eine Datei abruft, wird eine [DriveItemVersion](../resources/driveitemversion.md)-Ressource zurückgegeben, welche die verfügbaren Informationen zu der jeweiligen Version bereitstellt.</span><span class="sxs-lookup"><span data-stu-id="c1e86-128">When your app retrieves the list of available versions for a file, a [DriveItemVersion](../resources/driveitemversion.md) resource is returned that provides the available information about the specific version.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
