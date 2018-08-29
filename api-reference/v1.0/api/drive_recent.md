---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Zuletzt verwendete Dateien auflisten
ms.openlocfilehash: 9713803cb639f3eb27e46d087b0e8fec41abb5a7
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23267654"
---
# <a name="list-recent-files"></a><span data-ttu-id="d5d3a-102">Zuletzt verwendete Dateien auflisten</span><span class="sxs-lookup"><span data-stu-id="d5d3a-102">List recent files</span></span>

<span data-ttu-id="d5d3a-p101">Dient zum Auflisten eines Satzes von Elementen, die zuletzt von dem angemeldeten Benutzer verwendet wurden. Diese Sammlung enthält Elemente, die sich in dem Laufwerk des Benutzers befinden sowie Elemente in anderen Laufwerken, auf die dieser Zugriff hat.</span><span class="sxs-lookup"><span data-stu-id="d5d3a-p101">List a set of items that have been recently used by the signed in user. This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5d3a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d5d3a-105">Permissions</span></span>

<span data-ttu-id="d5d3a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d5d3a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d5d3a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d5d3a-108">Permission type</span></span>      | <span data-ttu-id="d5d3a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d5d3a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5d3a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d5d3a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d5d3a-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5d3a-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d5d3a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d5d3a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5d3a-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5d3a-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d5d3a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d5d3a-114">Application</span></span> | <span data-ttu-id="d5d3a-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5d3a-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5d3a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d5d3a-116">HTTP request</span></span>

<!-- { "blockType": "request",
       "name": "view-recent-files", 
       "scopes": "files.read",
       "tags": "service.graph",
       "target": "action" } -->

```http
GET /me/drive/recent
```

## <a name="response"></a><span data-ttu-id="d5d3a-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="d5d3a-117">Response</span></span>

<span data-ttu-id="d5d3a-118">Mit dieser Methode wird eine Sammlung von [DriveItem](../resources/driveitem.md)-Ressourcen für Elemente zurückgegeben, auf die der Besitzer des Laufwerks vor kurzem zugegriffen hat.</span><span class="sxs-lookup"><span data-stu-id="d5d3a-118">This method returns a collection of [DriveItem](../resources/driveitem.md) resources for items which the owner of the drive has recently accessed.</span></span>

<!-- { "blockType": "response",
       "@odata.type": "Collection(microsoft.graph.driveItem)",
       "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc!1231",
      "remoteItem":
      {
        "id": "1991210caf!192",
        "name": "March Proposal.docx",
        "file": { },
        "size": 19121,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      },
      "fileSystemInfo": {
        "lastAccessedDateTime": "2017-02-20T19:13:00Z"
      }
    },
    {
      "id": "1312def!9943",
      "name": "Vacation.jpg",
      "file": { },
      "size": 37810,
      "parentReference": {
        "driveId": "1312def",
        "id": "1312def!123"
      },
      "fileSystemInfo": {
        "lastAccessedDateTime": "2017-02-20T16:43:21Z"
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="d5d3a-119">Hinweise</span><span class="sxs-lookup"><span data-stu-id="d5d3a-119">Remarks</span></span>

<span data-ttu-id="d5d3a-p103">Einige driveItems, die von der **recent**-Aktion zurückgegeben werden, enthalten immer das **remoteItem**-Facet, das angibt, dass es sich um Elemente von einem anderen Laufwerk handelt. Um auf das ursprüngliche DriveItem-Objekt zuzugreifen, müssen Sie eine Anforderung anhand der Angaben in **remoteItem** im folgenden Format stellen:</span><span class="sxs-lookup"><span data-stu-id="d5d3a-p103">Some driveItems returned from the **recent** action will include the **remoteItem** facet which indicates they are items from another drive. To access the original driveItem object, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve a list of recently used files for the owner of the drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Drives/Recent files"
} -->
