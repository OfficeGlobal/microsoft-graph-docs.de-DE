---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Liste der Benutzer, die Zugriff auf eine Datei haben
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1157aaafbcebe784acef9c08ff3987a0921ef833
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481916"
---
# <a name="list-sharing-permissions-on-a-driveitem"></a><span data-ttu-id="53603-102">Auflisten von Berechtigungen für ein DriveItem</span><span class="sxs-lookup"><span data-stu-id="53603-102">List sharing permissions on a DriveItem</span></span>

<span data-ttu-id="53603-103">Listen Sie geltende Freigabe-Berechtigungen für ein [DriveItem](../resources/driveitem.md) auf.</span><span class="sxs-lookup"><span data-stu-id="53603-103">List the effective sharing permissions of on a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="access-to-sharing-permissions"></a><span data-ttu-id="53603-104">Zugriff auf Freigabe-Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="53603-104">Access to sharing permissions</span></span>

<span data-ttu-id="53603-105">Die Berechtigungssammlung umfasst potenziell vertrauliche Informationen und ist möglicherweise nicht für alle Aufrufer verfügbar.</span><span class="sxs-lookup"><span data-stu-id="53603-105">The permissions collection includes potentially sensitive information and may not be available for every caller.</span></span>

* <span data-ttu-id="53603-106">Für den Besitzer des Elements werden alle Freigabe-Berechtigungen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53603-106">For the owner of the item, all sharing permissions will be returned.</span></span> <span data-ttu-id="53603-107">Dies umfasst Mitbesitzer.</span><span class="sxs-lookup"><span data-stu-id="53603-107">This includes co-owners.</span></span>
* <span data-ttu-id="53603-108">Für Aufrufer, die keine Besitzer sind, werden nur die Freigabe-Berechtigungen zurückgegeben, die für den Aufrufer gelten.</span><span class="sxs-lookup"><span data-stu-id="53603-108">For a non-owner caller, only the sharing permissions that apply to the caller are returned.</span></span>
* <span data-ttu-id="53603-109">Freigabe-Berechtigungseigenschaften, die Geheimnisse enthalten (z. B. `shareId` und `webUrl`), werden nur für Aufrufer zurückgegeben, die Freigabe-Berechtigungen erstellen können.</span><span class="sxs-lookup"><span data-stu-id="53603-109">Sharing permission properties that contain secrets (e.g. `shareId` and `webUrl`) are only returned for callers that are able to create the sharing permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="53603-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="53603-110">Permissions</span></span>

<span data-ttu-id="53603-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53603-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53603-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="53603-113">Permission type</span></span>      | <span data-ttu-id="53603-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="53603-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53603-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="53603-115">Delegated (work or school account)</span></span> | <span data-ttu-id="53603-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53603-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="53603-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="53603-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53603-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53603-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="53603-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="53603-119">Application</span></span> | <span data-ttu-id="53603-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53603-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53603-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="53603-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /sites/{siteId}/drive/items/{itemId}/permissions
GET /users/{userId}/drive/items/{itemId}/permissions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="53603-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="53603-122">Optional query parameters</span></span>

<span data-ttu-id="53603-123">Diese Methode unterstützt die `$select` [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="53603-123">This method supports the `$select` [OData Query Parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="53603-124">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="53603-124">Optional request headers</span></span>

| <span data-ttu-id="53603-125">Name</span><span class="sxs-lookup"><span data-stu-id="53603-125">Name</span></span>          | <span data-ttu-id="53603-126">Typ</span><span class="sxs-lookup"><span data-stu-id="53603-126">Type</span></span>   | <span data-ttu-id="53603-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53603-127">Description</span></span>                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="53603-128">if-none-match</span><span class="sxs-lookup"><span data-stu-id="53603-128">if-none-match</span></span> | <span data-ttu-id="53603-129">string</span><span class="sxs-lookup"><span data-stu-id="53603-129">string</span></span> | <span data-ttu-id="53603-130">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen eTag in dem Element übereinstimmt, wird die Antwort `HTTP 304 Not Modified` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53603-130">If this request header is included and the etag provided matches the current etag on the item, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="53603-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="53603-131">Response</span></span>

<span data-ttu-id="53603-132">Bei Erfolg gibt diese Methode den Antwortcode `200 OK` und eine Sammlung von [Permission](../resources/permission.md)-Ressourcen im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="53603-132">If successful, this method returns a `200 OK` response code and collection of [Permission](../resources/permission.md) resources in the response body.</span></span>

<span data-ttu-id="53603-133">Geltende Freigabe-Berechtigungen eines DriveItem können aus zwei Quellen stammen:</span><span class="sxs-lookup"><span data-stu-id="53603-133">Effective sharing permissions of a DriveItem can come from two sources:</span></span>

* <span data-ttu-id="53603-134">Freigabe-Berechtigungen, die direkt für das DriveItem selbst gelten</span><span class="sxs-lookup"><span data-stu-id="53603-134">Sharing permissions applied directly on the DriveItem itself</span></span>
* <span data-ttu-id="53603-135">Freigabe-Berechtigungen, die von Vorgänger-DriveItems geerbt werden</span><span class="sxs-lookup"><span data-stu-id="53603-135">Sharing permissions inherited from the DriveItem's ancestors</span></span>

<span data-ttu-id="53603-p103">Aufrufer können prüfen, ob die Berechtigung geerbt wurde, indem sie die **inheritedFrom**-Eigenschaft prüfen. Diese Eigenschaft ist eine [**itemReference**](../resources/itemreference.md)-Ressource, die auf das Vorgängerelement verweist, von dem die Berechtigung vererbt wurde.</span><span class="sxs-lookup"><span data-stu-id="53603-p103">Callers can differentiate if the permission is inherited or not by checking the **inheritedFrom** property. This property is an [**itemReference**](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

<span data-ttu-id="53603-p104">SharePoint-Berechtigungsstufen, die für ein Element festgelegt wurden, werden mit der Präfix „SP“ zurückgegeben. Zum Beispiel SP.Nur anzeigen, SP.Beschränkter Zugriff, SP.Web Analytics-Daten anzeigen. Weitere Informationen finden Sie unter [Vollständige Liste der SharePoint-Rollen](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).</span><span class="sxs-lookup"><span data-stu-id="53603-p104">SharePoint permission levels set on an item are returned with an 'SP' prefix. For example, SP.View Only, SP.Limited Access, SP.View Web Analytics Data. See [Full list of SharePoint roles](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).</span></span>

## <a name="example"></a><span data-ttu-id="53603-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="53603-141">Example</span></span>

<span data-ttu-id="53603-142">In diesem Beispiel wird die Sammlung von Berechtigungen für ein Element auf dem Laufwerk des angemeldeten Benutzers abgerufen.</span><span class="sxs-lookup"><span data-stu-id="53603-142">This example retrieves the collection of permissions on an item in the signed in user's drive.</span></span>

<!-- { "blockType": "request", "name": "get-item-permissions", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/permissions
```

### <a name="response"></a><span data-ttu-id="53603-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="53603-143">Response</span></span>

<span data-ttu-id="53603-144">Diese Beispielantwort umfasst drei Berechtigungen, bei der ersten handelt es sich um einen Freigabelink mit Bearbeitungsberechtigungen, bei der zweiten handelt es sich um eine ausdrückliche Berechtigung für einen Benutzer mit dem Namen John, die von einem übergeordneten Ordner vererbt wurde und bei der dritten handelt es sich um einen Freigabelink mit Lese-/Schreibberechtigung, der von einer Anwendung erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="53603-144">This example response includes three permissions, the first is a sharing link with edit permissions, the second is an explicit permission for a user named John, which was inherited from a parent folder, and the third is a read-write sharing link created by an application.</span></span>

<!-- {"blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit"
      }
    },
    {
      "id": "2",
      "roles": ["write"],
      "grantedTo": {
        "user": {
          "id": "5D33DD65C6932946",
          "displayName": "John Doe"
        }
      },
      "inheritedFrom": {
        "driveId": "1234567890ABD",
        "id": "1234567890ABC!123",
        "path": "/drive/root:/Documents" }
    },
    {
      "id": "3",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit",
        "application": {
          "id": "12345",
          "displayName": "Contoso Time Manager"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="53603-145">Hinweise</span><span class="sxs-lookup"><span data-stu-id="53603-145">Remarks</span></span>

<span data-ttu-id="53603-p105">Die **permissions**-Beziehungen eines DriveItem-Elements können nicht im Rahmen eines Aufrufs von [get DriveItem](driveitem-get.md) oder einer Sammlung von DriveItems erweitert werden. Sie müssen direkt auf die permissions-Eigenschaft zugreifen.</span><span class="sxs-lookup"><span data-stu-id="53603-p105">The **permissions** relationship of DriveItem cannot be expanded as part of a call to [get DriveItem](driveitem-get.md) or a collection of DriveItems. You must access the permissions property directly.</span></span>

## <a name="error-responses"></a><span data-ttu-id="53603-148">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="53603-148">Error responses</span></span>

<span data-ttu-id="53603-149">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie im Thema [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="53603-149">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "List an item's permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "Sharing/Permissions"
} -->
