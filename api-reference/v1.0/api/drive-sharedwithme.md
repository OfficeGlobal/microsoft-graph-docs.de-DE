---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Mit mir geteilte Dateien auflisten
localization_priority: Priority
ms.openlocfilehash: 89ad3a5fc8aa12dd6865a629fd80b5a72623302c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889425"
---
# <a name="list-items-shared-with-the-signed-in-user"></a><span data-ttu-id="1211b-102">Elemente auflisten, die für den angemeldeten Benutzer freigegeben sind</span><span class="sxs-lookup"><span data-stu-id="1211b-102">List items shared with the signed-in user</span></span>

<span data-ttu-id="1211b-103">Mit dieser API können Sie eine Sammlung von Ressourcen des Typs [DriveItem](../resources/driveitem.md) abrufen, die für den Besitzer der Ressource des Typs [Drive](../resources/drive.md) freigegeben wurden.</span><span class="sxs-lookup"><span data-stu-id="1211b-103">Retrieve a collection of [DriveItem](../resources/driveitem.md) resources that have been shared with the owner of the [Drive](../resources/drive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1211b-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1211b-104">Permissions</span></span>

<span data-ttu-id="1211b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1211b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1211b-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1211b-107">Permission type</span></span>      | <span data-ttu-id="1211b-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1211b-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1211b-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1211b-109">Delegated (work or school account)</span></span> | <span data-ttu-id="1211b-110">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1211b-110">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1211b-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1211b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1211b-112">Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1211b-112">Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="1211b-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1211b-113">Application</span></span> | <span data-ttu-id="1211b-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1211b-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

<span data-ttu-id="1211b-115">**Hinweis:** Die /sharedWithMe-Anforderung funktioniert zwar mit Files.Read- oder Files.ReadWrite-Berechtigungen, es kann jedoch sein, dass einige Eigenschaften fehlen.</span><span class="sxs-lookup"><span data-stu-id="1211b-115">**Note:** while the /sharedWithMe request will succeed with Files.Read or Files.ReadWrite permissions, some properties may be missing.</span></span>
<span data-ttu-id="1211b-116">Zusätzlich gilt: Ohne eine der Berechtigungen des Typs **All** ist kein Zugriff auf die von dieser API zurückgegebenen freigegebenen Elemente möglich.</span><span class="sxs-lookup"><span data-stu-id="1211b-116">Additionally, without one of the  **All** permissions, shared items returned from this API will not be accessible.</span></span>

## <a name="http-request"></a><span data-ttu-id="1211b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1211b-117">HTTP request</span></span>

<!-- { "blockType": "request", "name": "shared-with-me", "scopes": "files.read", "tags": "service.graph", "target": "action" } -->

```http
GET /me/drive/sharedWithMe
```

## <a name="response"></a><span data-ttu-id="1211b-118">Antwort</span><span class="sxs-lookup"><span data-stu-id="1211b-118">Response</span></span>

<span data-ttu-id="1211b-p103">Dadurch wird eine Sammlung von [DriveItem](../resources/driveitem.md)-Ressourcen, zurückgegeben, die die DriveItem-Ressourcen enthalten, die für den Besitzer des Laufwerks freigegeben wurden. Da es sich bei dem Laufwerk um das Standardlaufwerk des Benutzers handelt, werden in diesem Beispiel Elemente zurückgegeben, die für den angemeldeten Benutzer freigegeben sind.</span><span class="sxs-lookup"><span data-stu-id="1211b-p103">This returns a collection of [DriveItem](../resources/driveitem.md) resources which contain the DriveItem resources shared with the owner of the drive. In this example, since the drive is the user's default drive, this returns items shared with the signed in user.</span></span>

<!-- {"blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc",
      "remoteItem": {
        "id": "1991210caf!192",
        "name": "March Proposal.docx",
        "file": { },
        "size": 19121,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    },
    {
      "id": "1312def",
      "remoteItem": {
        "id": "1991210caf!1991",
        "name": "Team Roster.xlsx",
        "file": { },
        "size": 37619,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="1211b-121">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="1211b-121">Remarks</span></span>

<span data-ttu-id="1211b-p104">DriveItems, die von der **SharedWithMe**-Aktion zurückgegeben werden, enthalten immer das [**remoteItem**](../resources/remoteitem.md)-Facet, das angibt, dass es sich um Elemente von einem anderen Laufwerk handelt. Um auf die freigegebenen DriveItem Ressourcen zuzugreifen, müssen Sie eine Anforderung anhand der Angaben in **remoteItem** im folgenden Format stellen:</span><span class="sxs-lookup"><span data-stu-id="1211b-p104">DriveItems returned from the **sharedWithMe** action will always include the [**remoteItem**](../resources/remoteitem.md) facet which indicates they are items from a different drive. To access the shared DriveItem resource, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```

<!-- {
  "type": "#page.annotation",
  "description": "List the items shared with the owner of a drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Sharing/Shared with me"
} -->
