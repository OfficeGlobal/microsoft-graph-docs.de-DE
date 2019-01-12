---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Freigeben einer Datei mit einem Link
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 75403c44a0d69269d7fe11b947da2f17b013dd3f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940407"
---
# <a name="create-a-sharing-link-for-a-driveitem"></a><span data-ttu-id="34ed7-102">Freigabelink für ein DriveItem erstellen</span><span class="sxs-lookup"><span data-stu-id="34ed7-102">Create a sharing link for a DriveItem</span></span>

> <span data-ttu-id="34ed7-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="34ed7-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34ed7-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34ed7-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34ed7-105">Sie können die Aktion **createLink** verwenden, um ein [DriveItem](../resources/driveitem.md) über einen Freigabelink freizugeben.</span><span class="sxs-lookup"><span data-stu-id="34ed7-105">You can use **createLink** action to share a [DriveItem](../resources/driveitem.md) via a sharing link.</span></span>

<span data-ttu-id="34ed7-p102">Die Aktion **createLink** erstellt einen neuen Freigabelink, falls der angegebene Linktyp für die aufrufende Anwendung noch nicht existiert. Existiert für die App bereits ein Freigabelink des angegebenen Typs, wird dieser bereits vorhandene Freigabelink zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="34ed7-p102">The **createLink** action will create a new sharing link if the specified link type doesn't already exist for the calling application. If a sharing link of the specified type already exists for the app, the existing sharing link will be returned.</span></span>

<span data-ttu-id="34ed7-108">DriveItem-Ressourcen erben Freigabe-Berechtigungen von ihren Vorgängern.</span><span class="sxs-lookup"><span data-stu-id="34ed7-108">DriveItem resources inherit sharing permissions from their ancestors.</span></span>

## <a name="permissions"></a><span data-ttu-id="34ed7-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="34ed7-109">Permissions</span></span>

<span data-ttu-id="34ed7-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34ed7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34ed7-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="34ed7-112">Permission type</span></span>      | <span data-ttu-id="34ed7-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="34ed7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34ed7-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="34ed7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="34ed7-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34ed7-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="34ed7-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="34ed7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34ed7-117">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34ed7-117">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="34ed7-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="34ed7-118">Application</span></span> | <span data-ttu-id="34ed7-119">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34ed7-119">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="34ed7-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="34ed7-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createLink
POST /groups/{groupId}/drive/items/{itemId}/createLink
POST /me/drive/items/{itemId}/createLink
POST /sites/{siteId}/drive/items/{itemId}/createLink
POST /users/{userId}/drive/items/{itemId}/createLink
```

### <a name="request-body"></a><span data-ttu-id="34ed7-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="34ed7-121">Request body</span></span>

<span data-ttu-id="34ed7-122">Der Anforderungstext definiert die Eigenschaften des Freigabelinks, den Ihre Anwendung anfordert.</span><span class="sxs-lookup"><span data-stu-id="34ed7-122">The body of the request defines properties of the sharing link your application is requesting.</span></span>
<span data-ttu-id="34ed7-123">Bei der Anforderung sollte es sich um ein JSON-Objekt mit folgenden Eigenschaften handeln:</span><span class="sxs-lookup"><span data-stu-id="34ed7-123">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="34ed7-124">Name</span><span class="sxs-lookup"><span data-stu-id="34ed7-124">Name</span></span>    |  <span data-ttu-id="34ed7-125">Typ</span><span class="sxs-lookup"><span data-stu-id="34ed7-125">Type</span></span>  |                                 <span data-ttu-id="34ed7-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34ed7-126">Description</span></span>                                  |
| :-------- | :----- | :--------------------------------------------------------------------------- |
| <span data-ttu-id="34ed7-127">**type**</span><span class="sxs-lookup"><span data-stu-id="34ed7-127">**type**</span></span>  | <span data-ttu-id="34ed7-128">string</span><span class="sxs-lookup"><span data-stu-id="34ed7-128">string</span></span> | <span data-ttu-id="34ed7-p105">Der Typ Freigabelink, der erstellt werden soll. Möglich sind `view`, `edit` oder `embed`.</span><span class="sxs-lookup"><span data-stu-id="34ed7-p105">The type of sharing link to create. Either `view`, `edit`, or `embed`.</span></span>       |
| <span data-ttu-id="34ed7-131">**scope**</span><span class="sxs-lookup"><span data-stu-id="34ed7-131">**scope**</span></span> | <span data-ttu-id="34ed7-132">string</span><span class="sxs-lookup"><span data-stu-id="34ed7-132">string</span></span> | <span data-ttu-id="34ed7-133">Optional.</span><span class="sxs-lookup"><span data-stu-id="34ed7-133">Optional.</span></span> <span data-ttu-id="34ed7-134">Der Bereich des zu erstellenden Links.</span><span class="sxs-lookup"><span data-stu-id="34ed7-134">The scope of link to create.</span></span> <span data-ttu-id="34ed7-135">Möglich sind `anonymous` oder `organization`.</span><span class="sxs-lookup"><span data-stu-id="34ed7-135">Either `anonymous` or `organization`.</span></span> |


### <a name="link-types"></a><span data-ttu-id="34ed7-136">Linktypen</span><span class="sxs-lookup"><span data-stu-id="34ed7-136">Link types</span></span>

<span data-ttu-id="34ed7-137">Für den Parameter **type** sind die folgenden Werte zulässig:</span><span class="sxs-lookup"><span data-stu-id="34ed7-137">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="34ed7-138">Typwert</span><span class="sxs-lookup"><span data-stu-id="34ed7-138">Type value</span></span> | <span data-ttu-id="34ed7-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34ed7-139">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | <span data-ttu-id="34ed7-140">Erstellt einen schreibgeschützten Link zum DriveItem.</span><span class="sxs-lookup"><span data-stu-id="34ed7-140">Creates a read-only link to the DriveItem.</span></span>                                                        |
| `edit`     | <span data-ttu-id="34ed7-141">Erstellt einen Link mit Lese-/Schreibzugriff zum DriveItem.</span><span class="sxs-lookup"><span data-stu-id="34ed7-141">Creates a read-write link to the DriveItem.</span></span>                                                       |
| `embed`    | <span data-ttu-id="34ed7-142">Erstellt einen einbettbaren Link zum DriveItem.</span><span class="sxs-lookup"><span data-stu-id="34ed7-142">Creates an embeddable link to the DriveItem.</span></span> <span data-ttu-id="34ed7-143">Diese Option ist nur für das persönliche OneDrive verfügbar.</span><span class="sxs-lookup"><span data-stu-id="34ed7-143">This option is only available for files in OneDrive personal.</span></span> |

### <a name="scope-types"></a><span data-ttu-id="34ed7-144">Bereichstypen</span><span class="sxs-lookup"><span data-stu-id="34ed7-144">Scope types</span></span>

<span data-ttu-id="34ed7-145">Für den Parameter **scope** sind die nachfolgend aufgeführten Werte zulässig.</span><span class="sxs-lookup"><span data-stu-id="34ed7-145">The following values are allowed for the **scope** parameter.</span></span>
<span data-ttu-id="34ed7-146">Wenn er **scope**-Parameter nicht angegeben ist, wird der Standardlinktyp für die Organisation erstellt.</span><span class="sxs-lookup"><span data-stu-id="34ed7-146">If the **scope** parameter is not specified, the default link type for the organization is created.</span></span>

| <span data-ttu-id="34ed7-147">Typwert</span><span class="sxs-lookup"><span data-stu-id="34ed7-147">Type value</span></span>     | <span data-ttu-id="34ed7-148">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34ed7-148">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="34ed7-149">Erstellt einen Link zum DriveItem, auf das alle über den Link zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="34ed7-149">Creates a link to the DriveItem accessible to anyone with the link.</span></span> <span data-ttu-id="34ed7-150">Anonyme Links können von einem Administrator deaktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="34ed7-150">Anonymous links may be disabled by an administrator.</span></span>                 |
| `organization` | <span data-ttu-id="34ed7-151">Erstellt einen Link zum DriveItem, auf das alle innerhalb der Organisation des Benutzers zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="34ed7-151">Creates a link to the DriveItem accessible to anyone within the user's organization.</span></span> <span data-ttu-id="34ed7-152">Der Linkbereich „organization“ ist nicht für das persönliche OneDrive verfügbar.</span><span class="sxs-lookup"><span data-stu-id="34ed7-152">Organization link scope is not available for OneDrive personal.</span></span> |

## <a name="response"></a><span data-ttu-id="34ed7-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="34ed7-153">Response</span></span>

<span data-ttu-id="34ed7-154">Bei Erfolg gibt diese Methode eine einzige Ressource des Typs [Permission](../resources/permission.md) im Antworttext zurück. Dabei handelt es sich um die angeforderten Freigabe-Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="34ed7-154">If successful, this method returns a single [Permission](../resources/permission.md) resource in the response body that represents the requested sharing permissions.</span></span>

<span data-ttu-id="34ed7-155">Wird ein neuer Freigabelink für das Element erstellt, lautet die Antwort `201 Created`. Wird ein bereits vorhandener Link zurückgegeben, lautet die Antwort `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="34ed7-155">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

## <a name="example"></a><span data-ttu-id="34ed7-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="34ed7-156">Example</span></span>

<span data-ttu-id="34ed7-157">Im folgende Beispiel wird das Erstellen eines Freigabelinks für das DriveItem angefordert, das durch {ItemId} im OneDrive des Benutzers angegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="34ed7-157">The following example requests a sharing link to be created for the DriveItem specified by {itemId} in the user's OneDrive.</span></span>
<span data-ttu-id="34ed7-158">Der Freigabelink ist schreibgeschützt konfiguriert und kann von allen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="34ed7-158">The sharing link is configured to be read-only and usable by anyone with the link.</span></span>

### <a name="request"></a><span data-ttu-id="34ed7-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="34ed7-159">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "item_createlink"
}-->

```http
POST /me/drive/items/{itemId}/createLink
Content-type: application/json

{
  "type": "view",
  "scope": "anonymous"
}
```

### <a name="response"></a><span data-ttu-id="34ed7-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="34ed7-160">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "anonymous",
    "webUrl": "https://1drv.ms/A6913278E564460AA616C71B28AD6EB6",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="creating-company-sharable-links"></a><span data-ttu-id="34ed7-161">Erstellen von nur innerhalb eines Unternehmens freigegebenen Links</span><span class="sxs-lookup"><span data-stu-id="34ed7-161">Creating company sharable links</span></span>

<span data-ttu-id="34ed7-162">OneDrive for Business und SharePoint unterstützen Links, die nur innerhalb eines Unternehmens freigegeben sind.</span><span class="sxs-lookup"><span data-stu-id="34ed7-162">OneDrive for Business and SharePoint support company sharable links.</span></span>
<span data-ttu-id="34ed7-163">Diese ähneln anonymen Links, funktionieren aber nur für Mitglieder der Besitzorganisation.</span><span class="sxs-lookup"><span data-stu-id="34ed7-163">These are similar to anonymous links, except they only work for members of the owning organization.</span></span>
<span data-ttu-id="34ed7-164">Verwenden Sie den Parameter **scope** mit dem Wert `organization`, um einen Link zu erstellen, der nur innerhalb eines Unternehmens freigegeben ist.</span><span class="sxs-lookup"><span data-stu-id="34ed7-164">To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

### <a name="request"></a><span data-ttu-id="34ed7-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="34ed7-165">Request</span></span>

<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite service.sharepoint" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

### <a name="response"></a><span data-ttu-id="34ed7-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="34ed7-166">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "edit",
    "scope": "organization",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="creating-embeddable-links"></a><span data-ttu-id="34ed7-167">Erstellen von einbettbaren Links</span><span class="sxs-lookup"><span data-stu-id="34ed7-167">Creating embeddable links</span></span>

<span data-ttu-id="34ed7-p113">Bei Verwendung des Linktyps `embed` kann der zurückgegebene Wert für „webUrl“ in ein HTML-Element des Typs `<iframe>` eingebettet werden. Wird ein Einbettungslink erstellt, enthält die Eigenschaft `webHtml` den HTML-Code für einen `<iframe>`, der den Inhalt hostet.</span><span class="sxs-lookup"><span data-stu-id="34ed7-p113">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

<span data-ttu-id="34ed7-170">**Hinweis:** Einbettungslinks werden nur fürdas persönlich OneDrive unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34ed7-170">**Note:** Embed links are only supported for OneDrive personal.</span></span>

### <a name="request"></a><span data-ttu-id="34ed7-171">Anforderung</span><span class="sxs-lookup"><span data-stu-id="34ed7-171">Request</span></span>

<!-- { "blockType": "request", "name": "create-embedded-link", "scopes": "files.readwrite service.onedrive" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```

### <a name="response"></a><span data-ttu-id="34ed7-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="34ed7-172">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["read"],
  "link": {
    "type": "embed",
    "webHtml": "<IFRAME src=\"https://onedrive.live.com/...\"></IFRAME>",
    "webUrl": "https://onedive.live.com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="remarks"></a><span data-ttu-id="34ed7-173">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="34ed7-173">Remarks</span></span>

* <span data-ttu-id="34ed7-174">Mit dieser Aktion erstellte Links laufen nicht ab, es sei denn, für die Organisation wird eine Standardablaufrichtlinie erzwungen.</span><span class="sxs-lookup"><span data-stu-id="34ed7-174">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="34ed7-175">Links sind in den Freigabeberechtigungen für das Element sichtbar und können von einem Besitzer des Elements entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="34ed7-175">Links are visible in the sharing permissions for the item and can be removed by an owner of the item.</span></span>
* <span data-ttu-id="34ed7-176">Links zeigen immer auf die aktuelle Version eines Elements, es sei denn, das Element ist ausgecheckt (nur SharePoint).</span><span class="sxs-lookup"><span data-stu-id="34ed7-176">Links always point to the current version of a item unless the item is checked out (SharePoint only).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Create a new sharing link for an item.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link"
} -->
