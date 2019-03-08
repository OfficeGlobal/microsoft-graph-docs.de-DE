---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Berechtigungen abrufen
localization_priority: Normal
ms.openlocfilehash: 3c0d8c9a00a098e83ec0ff7bd4282546fe7d94c1
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481349"
---
# <a name="get-sharing-permission-for-a-file-or-folder"></a><span data-ttu-id="47e3f-102">Abrufen einer Freigabeberechtigung für eine Datei oder einen Ordner</span><span class="sxs-lookup"><span data-stu-id="47e3f-102">Get sharing permission for a file or folder</span></span>

<span data-ttu-id="47e3f-103">Geben Sie die geltende Freigabeberechtigung für eine bestimmte Berechtigungsressource zurück.</span><span class="sxs-lookup"><span data-stu-id="47e3f-103">Return the effective sharing permission for a particular permission resource.</span></span>

<span data-ttu-id="47e3f-104">Geltende Berechtigungen eines Elements können aus zwei Quellen stammen: Berechtigungen, die direkt für das Element selbst festgelegt werden, oder Berechtigungen, die von den Vorgängern des Elements geerbt werden.</span><span class="sxs-lookup"><span data-stu-id="47e3f-104">Effective permissions of an item can come from two sources: permissions set directly on the item itself or permissions that are inherited from the item's ancestors.</span></span>

<span data-ttu-id="47e3f-p101">Aufrufer können prüfen, ob die Berechtigung geerbt wurde, indem sie die `inheritedFrom`-Eigenschaft prüfen. Diese Eigenschaft ist eine [ItemReference](../resources/itemreference.md)-Ressource, die auf das Vorgängerelement verweist, von dem die Berechtigung vererbt wurde.</span><span class="sxs-lookup"><span data-stu-id="47e3f-p101">Callers can differentiate if the permission is inherited or not by checking the `inheritedFrom` property. This property is an [ItemReference](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

<span data-ttu-id="47e3f-p102">SharePoint-Berechtigungsstufen, die für ein Element festgelegt wurden, werden mit der Präfix „SP“ zurückgegeben. Zum Beispiel SP.Nur anzeigen, SP.Beschränkter Zugriff, SP.Web Analytics-Daten anzeigen. Weitere Informationen finden Sie unter [Vollständige Liste der SharePoint-Rollen](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).</span><span class="sxs-lookup"><span data-stu-id="47e3f-p102">SharePoint permission levels set on an item are returned with an 'SP' prefix. For example, SP.View Only, SP.Limited Access, SP.View Web Analytics Data. See [Full list of SharePoint roles](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).</span></span>

## <a name="permissions"></a><span data-ttu-id="47e3f-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="47e3f-110">Permissions</span></span>

<span data-ttu-id="47e3f-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47e3f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47e3f-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="47e3f-113">Permission type</span></span>      | <span data-ttu-id="47e3f-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="47e3f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47e3f-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="47e3f-115">Delegated (work or school account)</span></span> | <span data-ttu-id="47e3f-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47e3f-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="47e3f-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="47e3f-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47e3f-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47e3f-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="47e3f-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="47e3f-119">Application</span></span> | <span data-ttu-id="47e3f-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47e3f-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="47e3f-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="47e3f-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
GET /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
GET /me/drive/items/{item-id}/permissions/{perm-id}
GET /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
GET /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47e3f-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="47e3f-122">Optional query parameters</span></span>

<span data-ttu-id="47e3f-123">Diese Methode unterstützt die [$select-Abfrageparameter](/graph/query-parameters) zum Modellieren der Antwort.</span><span class="sxs-lookup"><span data-stu-id="47e3f-123">This method support the [$select query parameter](/graph/query-parameters) to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="47e3f-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="47e3f-124">Response</span></span>

<span data-ttu-id="47e3f-125">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und die aktualisierte [Berechtigungs](../resources/permission.md)-Ressource im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="47e3f-125">If successful, this method returns a `200 OK` response code and [Permission](../resources/permission.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47e3f-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="47e3f-126">Example</span></span>

### <a name="request"></a><span data-ttu-id="47e3f-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="47e3f-127">Request</span></span>

<span data-ttu-id="47e3f-128">Nachfolgend finden Sie ein Beispiel der Anforderung für den Zugriff auf eine Berechtigung zu einem Ordner.</span><span class="sxs-lookup"><span data-stu-id="47e3f-128">Here is an example of the request to access a permission on a folder.</span></span>

<!-- { "blockType": "request", "name": "get-item-permission", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/permissions/{perm-id}
```

### <a name="response"></a><span data-ttu-id="47e3f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="47e3f-129">Response</span></span>

<span data-ttu-id="47e3f-130">Bei Erfolg gibt diese Methode eine [Permission](../resources/permission.md)-Ressource für die angegebene ID zurück.</span><span class="sxs-lookup"><span data-stu-id="47e3f-130">If successful, this method returns a [Permission](../resources/permission.md) resource for the specified ID.</span></span> 

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.permission", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "write" ]
}
```

## <a name="remarks"></a><span data-ttu-id="47e3f-131">Hinweise</span><span class="sxs-lookup"><span data-stu-id="47e3f-131">Remarks</span></span>

<span data-ttu-id="47e3f-132">Die [Permission](../resources/permission.md)-Ressource verwendet _Facets_ zum Bereitstellen von Informationen über die Art der Berechtigung, die die Ressource dargestellt.</span><span class="sxs-lookup"><span data-stu-id="47e3f-132">The [Permission](../resources/permission.md) resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="47e3f-p104">Berechtigungen für ein [**link**](../resources/sharinglink.md)-Facet stellen Freigabe-Links dar, die für das Element erstellt wurden. Freigabelinks enthalten ein eindeutiges Token, mit dem alle Benutzer, die über den Link verfügen, Zugriff auf das Element haben.</span><span class="sxs-lookup"><span data-stu-id="47e3f-p104">Permissions with a [**link**](../resources/sharinglink.md) facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="47e3f-135">Berechtigungen mit einem [**invitation**](../resources/sharinginvitation.md)-Facet stellen Berechtigungen dar, die durch Einladung bestimmter Benutzer oder Gruppen für Zugriff auf die Datei hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="47e3f-135">Permissions with a [**invitation**](../resources/sharinginvitation.md) facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

### <a name="error-responses"></a><span data-ttu-id="47e3f-136">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="47e3f-136">Error responses</span></span>

<span data-ttu-id="47e3f-137">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie im Thema [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="47e3f-137">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Get a DriveItem's sharing permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "Sharing/Permissions"
} -->
