---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Liste mit Zugriff auf eine Datei
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 224674d15f77794da798b3f5690c492089a932f1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956494"
---
# <a name="list-sharing-permissions-on-a-driveitem"></a><span data-ttu-id="be5ca-102">Auflisten von Berechtigungen für ein DriveItem</span><span class="sxs-lookup"><span data-stu-id="be5ca-102">List sharing permissions on a DriveItem</span></span>

> <span data-ttu-id="be5ca-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="be5ca-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be5ca-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="be5ca-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="be5ca-105">Listen Sie geltende Freigabe-Berechtigungen für ein [DriveItem](../resources/driveitem.md) auf.</span><span class="sxs-lookup"><span data-stu-id="be5ca-105">List the effective sharing permissions of on a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="access-to-sharing-permissions"></a><span data-ttu-id="be5ca-106">Zugriff auf Freigabe-Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="be5ca-106">Access to sharing permissions</span></span>

<span data-ttu-id="be5ca-107">Die Berechtigungssammlung umfasst potenziell vertrauliche Informationen und ist möglicherweise nicht für alle Aufrufer verfügbar.</span><span class="sxs-lookup"><span data-stu-id="be5ca-107">The permissions collection includes potentially sensitive information and may not be available for every caller.</span></span>

* <span data-ttu-id="be5ca-108">Für den Besitzer des Elements werden alle Freigabe-Berechtigungen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="be5ca-108">For the owner of the item, all sharing permissions will be returned.</span></span> <span data-ttu-id="be5ca-109">Dies umfasst Mitbesitzer.</span><span class="sxs-lookup"><span data-stu-id="be5ca-109">This includes co-owners.</span></span>
* <span data-ttu-id="be5ca-110">Für Aufrufer, die keine Besitzer sind, werden nur die Freigabe-Berechtigungen zurückgegeben, die für den Aufrufer gelten.</span><span class="sxs-lookup"><span data-stu-id="be5ca-110">For a non-owner caller, only the sharing permissions that apply to the caller are returned.</span></span>
* <span data-ttu-id="be5ca-111">Freigabe-Berechtigungseigenschaften, die Geheimnisse enthalten (z. B. `shareId` und `webUrl`), werden nur für Aufrufer zurückgegeben, die Freigabe-Berechtigungen erstellen können.</span><span class="sxs-lookup"><span data-stu-id="be5ca-111">Sharing permission properties that contain secrets (e.g. `shareId` and `webUrl`) are only returned for callers that are able to create the sharing permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="be5ca-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="be5ca-112">Permissions</span></span>

<span data-ttu-id="be5ca-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be5ca-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be5ca-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="be5ca-115">Permission type</span></span>      | <span data-ttu-id="be5ca-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="be5ca-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be5ca-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="be5ca-117">Delegated (work or school account)</span></span> | <span data-ttu-id="be5ca-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be5ca-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="be5ca-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="be5ca-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be5ca-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be5ca-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="be5ca-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="be5ca-121">Application</span></span> | <span data-ttu-id="be5ca-122">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be5ca-122">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="be5ca-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="be5ca-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /sites/{siteId}/drive/items/{itemId}/permissions
GET /users/{userId}/drive/items/{itemId}/permissions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="be5ca-124">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="be5ca-124">Optional query parameters</span></span>

<span data-ttu-id="be5ca-125">Diese Methode unterstützt die `$select` [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="be5ca-125">This method supports the `$select` [OData Query Parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="be5ca-126">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="be5ca-126">Optional request headers</span></span>

| <span data-ttu-id="be5ca-127">Name</span><span class="sxs-lookup"><span data-stu-id="be5ca-127">Name</span></span>          | <span data-ttu-id="be5ca-128">Typ</span><span class="sxs-lookup"><span data-stu-id="be5ca-128">Type</span></span>   | <span data-ttu-id="be5ca-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="be5ca-129">Description</span></span>                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="be5ca-130">if-none-match</span><span class="sxs-lookup"><span data-stu-id="be5ca-130">if-none-match</span></span> | <span data-ttu-id="be5ca-131">string</span><span class="sxs-lookup"><span data-stu-id="be5ca-131">string</span></span> | <span data-ttu-id="be5ca-132">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen eTag in dem Element übereinstimmt, wird die Antwort `HTTP 304 Not Modified` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="be5ca-132">If this request header is included and the etag provided matches the current etag on the item, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="be5ca-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="be5ca-133">Response</span></span>

<span data-ttu-id="be5ca-134">Bei Erfolg gibt diese Methode den Antwortcode `200 OK` und eine Sammlung von [Permission](../resources/permission.md)-Ressourcen im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="be5ca-134">If successful, this method returns a `200 OK` response code and collection of [Permission](../resources/permission.md) resources in the response body.</span></span>

<span data-ttu-id="be5ca-135">Geltende Freigabe-Berechtigungen eines DriveItem können aus zwei Quellen stammen:</span><span class="sxs-lookup"><span data-stu-id="be5ca-135">Effective sharing permissions of a DriveItem can come from two sources:</span></span>

* <span data-ttu-id="be5ca-136">Freigabe-Berechtigungen, die direkt für das DriveItem selbst gelten</span><span class="sxs-lookup"><span data-stu-id="be5ca-136">Sharing permissions applied directly on the DriveItem itself</span></span>
* <span data-ttu-id="be5ca-137">Freigabe-Berechtigungen, die von Vorgänger-DriveItems geerbt werden</span><span class="sxs-lookup"><span data-stu-id="be5ca-137">Sharing permissions inherited from the DriveItem's ancestors</span></span>

<span data-ttu-id="be5ca-p104">Aufrufer können prüfen, ob die Berechtigung geerbt wurde, indem sie die **inheritedFrom**-Eigenschaft prüfen. Diese Eigenschaft ist eine [**itemReference**](../resources/itemreference.md)-Ressource, die auf das Vorgängerelement verweist, von dem die Berechtigung vererbt wurde.</span><span class="sxs-lookup"><span data-stu-id="be5ca-p104">Callers can differentiate if the permission is inherited or not by checking the **inheritedFrom** property. This property is an [**itemReference**](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

<span data-ttu-id="be5ca-140">SharePoint-Berechtigungsstufen, die für ein Element festgelegt wurden, werden mit der Präfix „SP“ zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="be5ca-140">SharePoint permission levels set on an item are returned with an 'SP' prefix.</span></span> <span data-ttu-id="be5ca-141">Zum Beispiel SP.Nur anzeigen, SP.Beschränkter Zugriff, SP.Web Analytics-Daten anzeigen.</span><span class="sxs-lookup"><span data-stu-id="be5ca-141">For example, SP.View Only, SP.Limited Access, SP.View Web Analytics Data.</span></span> <span data-ttu-id="be5ca-142">Weitere Informationen finden Sie unter [Vollständige Liste der SharePoint-Rollen](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).</span><span class="sxs-lookup"><span data-stu-id="be5ca-142">See [Full list of SharePoint roles](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).</span></span>

## <a name="example"></a><span data-ttu-id="be5ca-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="be5ca-143">Example</span></span>

<span data-ttu-id="be5ca-144">In diesem Beispiel wird die Sammlung von Berechtigungen für ein Element auf dem Laufwerk des angemeldeten Benutzers abgerufen.</span><span class="sxs-lookup"><span data-stu-id="be5ca-144">This example retrieves the collection of permissions on an item in the signed in user's drive.</span></span>

<!-- { "blockType": "request", "name": "get-item-permissions", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/permissions
```

### <a name="response"></a><span data-ttu-id="be5ca-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="be5ca-145">Response</span></span>

<span data-ttu-id="be5ca-146">Diese Beispielantwort umfasst drei Berechtigungen, bei der ersten handelt es sich um einen Freigabelink mit Bearbeitungsberechtigungen, bei der zweiten handelt es sich um eine ausdrückliche Berechtigung für einen Benutzer mit dem Namen John, die von einem übergeordneten Ordner vererbt wurde und bei der dritten handelt es sich um einen Freigabelink mit Lese-/Schreibberechtigung, der von einer Anwendung erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="be5ca-146">This example response includes three permissions, the first is a sharing link with edit permissions, the second is an explicit permission for a user named John, which was inherited from a parent folder, and the third is a read-write sharing link created by an application.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="be5ca-147">Hinweise</span><span class="sxs-lookup"><span data-stu-id="be5ca-147">Remarks</span></span>

<span data-ttu-id="be5ca-p106">Die **permissions**-Beziehungen eines DriveItem-Elements können nicht im Rahmen eines Aufrufs von [get DriveItem](driveitem-get.md) oder einer Sammlung von DriveItems erweitert werden. Sie müssen direkt auf die permissions-Eigenschaft zugreifen.</span><span class="sxs-lookup"><span data-stu-id="be5ca-p106">The **permissions** relationship of DriveItem cannot be expanded as part of a call to [get DriveItem](driveitem-get.md) or a collection of DriveItems. You must access the permissions property directly.</span></span>

## <a name="error-responses"></a><span data-ttu-id="be5ca-150">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="be5ca-150">Error responses</span></span>

<span data-ttu-id="be5ca-151">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie im Thema [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="be5ca-151">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "List an item's permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "Sharing/Permissions"
} -->
