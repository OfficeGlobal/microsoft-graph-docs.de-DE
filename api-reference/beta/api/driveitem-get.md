---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Eine Datei oder einen Ordner abrufen
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f9b159e4686a22b759e2f2a42776df8dafb3a2b0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518107"
---
# <a name="get-a-driveitem-resource"></a><span data-ttu-id="ee99c-102">DriveItem-Ressource abrufen</span><span class="sxs-lookup"><span data-stu-id="ee99c-102">Get a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee99c-103">Mit dieser API können Sie die Metadaten einer Ressource des Typs [DriveItem](../resources/driveitem.md) in einer Ressource des Typs [Drive](../resources/drive.md) abrufen. Hierzu verwenden Sie den Dateisystempfad oder die ID der Ressource des Typs „DriveItem“.</span><span class="sxs-lookup"><span data-stu-id="ee99c-103">Retrieve the metadata for a [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) by file system path or ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee99c-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ee99c-104">Permissions</span></span>

<span data-ttu-id="ee99c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee99c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee99c-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ee99c-107">Permission type</span></span>      | <span data-ttu-id="ee99c-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ee99c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee99c-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ee99c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="ee99c-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee99c-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ee99c-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ee99c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee99c-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee99c-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ee99c-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ee99c-113">Application</span></span> | <span data-ttu-id="ee99c-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee99c-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee99c-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ee99c-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}
GET /drives/{drive-id}/root:/{item-path}
GET /groups/{group-id}/drive/items/{item-id}
GET /groups/{group-id}/drive/root:/{item-path}
GET /me/drive/items/{item-id}
GET /me/drive/root:/{item-path}
GET /sites/{siteId}/drive/items/{itemId}
GET /sites/{siteId}/drive/root:/{item-path}
GET /users/{userId}/drive/items/{itemId}
GET /users/{userId}/drive/root:/{item-path}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ee99c-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ee99c-116">Optional query parameters</span></span>

<span data-ttu-id="ee99c-117">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) von `$expand` und `$select` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ee99c-117">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

<span data-ttu-id="ee99c-118">Sie können den [`$expand`Parameter der Abfragezeichenfolge](/graph/query-parameters) verwenden, um die untergeordneten Elemente eines Elements im gleichen Aufruf wie beim Abrufen der Metadaten eines Elements verwenden, wenn das Element eine **untergeordnete** Beziehung aufweist.</span><span class="sxs-lookup"><span data-stu-id="ee99c-118">You can use the [`$expand` query string parameter](/graph/query-parameters) to include the children of an item in the same call as retrieving the metadata of an item if the item has a **children** relationship.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="ee99c-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ee99c-119">Optional request headers</span></span>

| <span data-ttu-id="ee99c-120">Name</span><span class="sxs-lookup"><span data-stu-id="ee99c-120">Name</span></span>          | <span data-ttu-id="ee99c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ee99c-121">Value</span></span>  | <span data-ttu-id="ee99c-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee99c-122">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ee99c-123">if-none-match</span><span class="sxs-lookup"><span data-stu-id="ee99c-123">if-none-match</span></span> | <span data-ttu-id="ee99c-124">String</span><span class="sxs-lookup"><span data-stu-id="ee99c-124">String</span></span> | <span data-ttu-id="ee99c-125">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) mit dem aktuellen Tag in der Datei übereinstimmt, wird die Antwort `HTTP 304 Not Modified` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ee99c-125">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="ee99c-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="ee99c-126">Response</span></span>

<span data-ttu-id="ee99c-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und die aktualisierte [DriveItem](../resources/driveitem.md)-Ressource im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ee99c-127">If successful, this method returns a `200 OK` response code and the [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee99c-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ee99c-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee99c-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ee99c-129">Request</span></span>

<span data-ttu-id="ee99c-130">Nachfolgend finden Sie ein Beispiel der Anforderung für den Stammordner des OneDrive-Elements des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="ee99c-130">Here is an example of the request to the root folder of the user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "get-item-metadata" }-->

```http
GET /me/drive/root
```

## <a name="response"></a><span data-ttu-id="ee99c-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="ee99c-131">Response</span></span>

<span data-ttu-id="ee99c-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ee99c-132">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "createdBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "createdDateTime": "2016-03-21T20:01:37Z",
  "cTag": "\"c:{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},0\"",
  "eTag": "\"{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},1\"",
  "folder": { "childCount": 120 },
  "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
  "lastModifiedBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "lastModifiedDateTime": "2016-03-21T20:01:37Z",
  "name": "OneDrive",
  "root": { },
  "size": 157286400,
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents"
}
```

## <a name="remarks"></a><span data-ttu-id="ee99c-133">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="ee99c-133">Remarks</span></span>

<span data-ttu-id="ee99c-134">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie unter [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="ee99c-134">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[odata-parameters]: /graph/query-parameters
[item-resource]: ../resources/driveitem.md
[special-folder]: ../api/drive-get-specialfolder.md

<!--
{
  "type": "#page.annotation",
  "description": "Retrieve metadata about an item and its children in OneDrive",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Items/Get item",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
