---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Freigeben einer Datei mit einem Link
ms.openlocfilehash: 342e6ce403225a5d4b8b555a79355a721055e465
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="create-a-sharing-link-for-a-driveitem"></a><span data-ttu-id="0be09-102">Freigabelink für ein DriveItem erstellen</span><span class="sxs-lookup"><span data-stu-id="0be09-102">Create a sharing link for a DriveItem</span></span>

<span data-ttu-id="0be09-103">Sie können die Aktion **createLink** verwenden, um ein [DriveItem](../resources/driveitem.md) über einen Freigabelink freizugeben.</span><span class="sxs-lookup"><span data-stu-id="0be09-103">You can use **createLink** action to share a [DriveItem](../resources/driveitem.md) via a sharing link.</span></span>

<span data-ttu-id="0be09-p101">Die Aktion **createLink** erstellt einen neuen Freigabelink, falls der angegebene Linktyp für die aufrufende Anwendung noch nicht existiert. Existiert für die App bereits ein Freigabelink des angegebenen Typs, wird dieser bereits vorhandene Freigabelink zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0be09-p101">The **createLink** action will create a new sharing link if the specified link type doesn't already exist for the calling application. If a sharing link of the specified type already exists for the app, the existing sharing link will be returned.</span></span>

<span data-ttu-id="0be09-106">DriveItem-Ressourcen erben Freigabe-Berechtigungen von ihren Vorgängern.</span><span class="sxs-lookup"><span data-stu-id="0be09-106">DriveItem resources inherit permissions from their ancestors.</span></span>

## <a name="permissions"></a><span data-ttu-id="0be09-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0be09-107">Permissions</span></span>

<span data-ttu-id="0be09-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0be09-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0be09-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0be09-110">Permission type</span></span>      | <span data-ttu-id="0be09-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0be09-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0be09-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0be09-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0be09-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0be09-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0be09-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0be09-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0be09-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0be09-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="0be09-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0be09-116">Application</span></span> | <span data-ttu-id="0be09-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0be09-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0be09-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0be09-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createLink
POST /groups/{groupId}/drive/items/{itemId}/createLink
POST /me/drive/items/{itemId}/createLink
POST /sites/{siteId}/drive/items/{itemId}/createLink
POST /users/{userId}/drive/items/{itemId}/createLink
```

### <a name="request-body"></a><span data-ttu-id="0be09-119">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0be09-119">Request body</span></span>

<span data-ttu-id="0be09-120">Der Anforderungstext definiert die Eigenschaften des Freigabelinks, den Ihre Anwendung anfordert.</span><span class="sxs-lookup"><span data-stu-id="0be09-120">The body of the request defines properties of the sharing link your application is requesting.</span></span>
<span data-ttu-id="0be09-121">Bei der Anforderung sollte es sich um ein JSON-Objekt mit folgenden Eigenschaften handeln:</span><span class="sxs-lookup"><span data-stu-id="0be09-121">The request body should be a JSON object with the following properties:</span></span>

|   <span data-ttu-id="0be09-122">Name</span><span class="sxs-lookup"><span data-stu-id="0be09-122">Name</span></span>    |  <span data-ttu-id="0be09-123">Typ</span><span class="sxs-lookup"><span data-stu-id="0be09-123">Type</span></span>  |                                 <span data-ttu-id="0be09-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0be09-124">Description</span></span>                                  |
| :-------- | :----- | :--------------------------------------------------------------------------- |
| <span data-ttu-id="0be09-125">**type**</span><span class="sxs-lookup"><span data-stu-id="0be09-125">**type**</span></span>  | <span data-ttu-id="0be09-126">string</span><span class="sxs-lookup"><span data-stu-id="0be09-126">string</span></span> | <span data-ttu-id="0be09-p104">Der Typ Freigabelink, der erstellt werden soll. Möglich sind `view`, `edit` oder `embed`.</span><span class="sxs-lookup"><span data-stu-id="0be09-p104">The type of sharing link to create. Either `view`, `edit`, or `embed`.</span></span>       |
| <span data-ttu-id="0be09-129">**scope**</span><span class="sxs-lookup"><span data-stu-id="0be09-129">**scope**</span></span> | <span data-ttu-id="0be09-130">string</span><span class="sxs-lookup"><span data-stu-id="0be09-130">string</span></span> | <span data-ttu-id="0be09-131">Optional.</span><span class="sxs-lookup"><span data-stu-id="0be09-131">Optional.</span></span> <span data-ttu-id="0be09-132">Der Bereich des zu erstellenden Links.</span><span class="sxs-lookup"><span data-stu-id="0be09-132">The scope of link to create. Either  or . Optional.</span></span> <span data-ttu-id="0be09-133">Möglich sind `anonymous` oder `organization`.</span><span class="sxs-lookup"><span data-stu-id="0be09-133">Either `anonymous` or `organization`.</span></span> |


### <a name="link-types"></a><span data-ttu-id="0be09-134">Linktypen</span><span class="sxs-lookup"><span data-stu-id="0be09-134">Link types</span></span>

<span data-ttu-id="0be09-135">Für den Parameter **type** sind die folgenden Werte zulässig:</span><span class="sxs-lookup"><span data-stu-id="0be09-135">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="0be09-136">Typwert</span><span class="sxs-lookup"><span data-stu-id="0be09-136">Type value</span></span> | <span data-ttu-id="0be09-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0be09-137">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | <span data-ttu-id="0be09-138">Erstellt einen schreibgeschützten Link zum DriveItem.</span><span class="sxs-lookup"><span data-stu-id="0be09-138">Creates a read-only link to the item.</span></span>                                                        |
| `edit`     | <span data-ttu-id="0be09-139">Erstellt einen Link mit Lese-/Schreibzugriff zum DriveItem.</span><span class="sxs-lookup"><span data-stu-id="0be09-139">Creates a read-write link to the item.</span></span>                                                       |
| `embed`    | <span data-ttu-id="0be09-140">Erstellt einen einbettbaren Link zum DriveItem.</span><span class="sxs-lookup"><span data-stu-id="0be09-140">Creates an embeddable link to the DriveItem.</span></span> <span data-ttu-id="0be09-141">Diese Option ist nur für das persönliche OneDrive verfügbar.</span><span class="sxs-lookup"><span data-stu-id="0be09-141">This option is only available for files in OneDrive personal.</span></span> |

### <a name="scope-types"></a><span data-ttu-id="0be09-142">Bereichstypen</span><span class="sxs-lookup"><span data-stu-id="0be09-142">Scope types</span></span>

<span data-ttu-id="0be09-143">Für den Parameter **scope** sind die nachfolgend aufgeführten Werte zulässig.</span><span class="sxs-lookup"><span data-stu-id="0be09-143">The following values are allowed for the **type** parameter.</span></span>
<span data-ttu-id="0be09-144">Wenn er **scope**-Parameter nicht angegeben ist, wird der Standardlinktyp für die Organisation erstellt.</span><span class="sxs-lookup"><span data-stu-id="0be09-144">If the **scope** parameter is not specified, the default link type for the organization is created.</span></span>

| <span data-ttu-id="0be09-145">Typwert</span><span class="sxs-lookup"><span data-stu-id="0be09-145">Type value</span></span>     | <span data-ttu-id="0be09-146">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0be09-146">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="0be09-147">Erstellt einen Link zum DriveItem, auf das alle über den Link zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="0be09-147">Creates a link to the DriveItem accessible to anyone with the link.</span></span> <span data-ttu-id="0be09-148">Anonyme Links können von einem Administrator deaktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="0be09-148">Anonymous links may be disabled by an administrator.</span></span>                 |
| `organization` | <span data-ttu-id="0be09-149">Erstellt einen Link zum DriveItem, auf das alle innerhalb der Organisation des Benutzers zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="0be09-149">Creates a link to the DriveItem accessible to anyone within the user's organization.</span></span> <span data-ttu-id="0be09-150">Der Linkbereich „organization“ ist nicht für das persönliche OneDrive verfügbar.</span><span class="sxs-lookup"><span data-stu-id="0be09-150">Organization link scope is not available for OneDrive personal.</span></span> |

## <a name="response"></a><span data-ttu-id="0be09-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="0be09-151">Response</span></span>

<span data-ttu-id="0be09-152">Bei Erfolg gibt diese Methode eine einzige Ressource des Typs [Permission](../resources/permission.md) im Antworttext zurück. Dabei handelt es sich um die angeforderten Freigabe-Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="0be09-152">If successful, this method returns a single [Permission](../resources/permission.md) resource in the response body that represents the requested sharing link permission.</span></span>

<span data-ttu-id="0be09-153">Wird ein neuer Freigabelink für das Element erstellt, lautet die Antwort `201 Created`. Wird ein bereits vorhandener Link zurückgegeben, lautet die Antwort `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="0be09-153">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

## <a name="example"></a><span data-ttu-id="0be09-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0be09-154">Example</span></span>

<span data-ttu-id="0be09-155">Im folgende Beispiel wird das Erstellen eines Freigabelinks für das DriveItem angefordert, das durch {ItemId} im OneDrive des Benutzers angegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="0be09-155">The following example requests a sharing link to be created for the DriveItem specified by {itemId} in the user's OneDrive.</span></span>
<span data-ttu-id="0be09-156">Der Freigabelink ist schreibgeschützt konfiguriert und kann von allen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="0be09-156">The sharing link is configured to be read-only and usable by anyone with the link.</span></span>

### <a name="request"></a><span data-ttu-id="0be09-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0be09-157">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="0be09-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="0be09-158">Response</span></span>

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

## <a name="creating-company-sharable-links"></a><span data-ttu-id="0be09-159">Erstellen von nur innerhalb eines Unternehmens freigegebenen Links</span><span class="sxs-lookup"><span data-stu-id="0be09-159">Creating company sharable links</span></span>

<span data-ttu-id="0be09-160">OneDrive for Business und SharePoint unterstützen Links, die nur innerhalb eines Unternehmens freigegeben sind.</span><span class="sxs-lookup"><span data-stu-id="0be09-160">OneDrive for Business and SharePoint support company sharable links.</span></span>
<span data-ttu-id="0be09-161">Diese ähneln anonymen Links, funktionieren aber nur für Mitglieder der Besitzorganisation.</span><span class="sxs-lookup"><span data-stu-id="0be09-161">These are similar to anonymous links, except they only work for members of the owning organization.</span></span>
<span data-ttu-id="0be09-162">Verwenden Sie den Parameter **scope** mit dem Wert `organization`, um einen Link zu erstellen, der nur innerhalb eines Unternehmens freigegeben ist.</span><span class="sxs-lookup"><span data-stu-id="0be09-162">To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

### <a name="request"></a><span data-ttu-id="0be09-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0be09-163">Request</span></span>

<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite service.sharepoint" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

### <a name="response"></a><span data-ttu-id="0be09-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="0be09-164">Response</span></span>

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

## <a name="creating-embeddable-links"></a><span data-ttu-id="0be09-165">Erstellen von einbettbaren Links</span><span class="sxs-lookup"><span data-stu-id="0be09-165">Creating embeddable links</span></span>

<span data-ttu-id="0be09-p112">Bei Verwendung des Linktyps `embed` kann der zurückgegebene Wert für „webUrl“ in ein HTML-Element des Typs `<iframe>` eingebettet werden. Wird ein Einbettungslink erstellt, enthält die Eigenschaft `webHtml` den HTML-Code für einen `<iframe>`, der den Inhalt hostet.</span><span class="sxs-lookup"><span data-stu-id="0be09-p112">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

<span data-ttu-id="0be09-168">**Hinweis:** Einbettungslinks werden nur fürdas persönlich OneDrive unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0be09-168">**Note:** Embed links are only supported for OneDrive Personal.</span></span>

### <a name="request"></a><span data-ttu-id="0be09-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0be09-169">Request</span></span>

<!-- { "blockType": "request", "name": "create-embedded-link", "scopes": "files.readwrite service.onedrive" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```

### <a name="response"></a><span data-ttu-id="0be09-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="0be09-170">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="0be09-171">HinwBemerkungeneise</span><span class="sxs-lookup"><span data-stu-id="0be09-171">Remarks</span></span>

* <span data-ttu-id="0be09-172">Mit dieser Aktion erstellte Links laufen nicht ab, es sei denn, für die Organisation wird eine Standardablaufrichtlinie erzwungen.</span><span class="sxs-lookup"><span data-stu-id="0be09-172">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="0be09-173">Links sind in den Freigabeberechtigungen für das Element sichtbar und können von einem Besitzer des Elements entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="0be09-173">Links are visible in the sharing permissions for the item and can be removed by an owner of the item.</span></span>
* <span data-ttu-id="0be09-174">Links zeigen immer auf die aktuelle Version eines Elements, es sei denn, das Element ist ausgecheckt (nur SharePoint).</span><span class="sxs-lookup"><span data-stu-id="0be09-174">Links always point to the current version of a item unless the item is checked out (SharePoint only).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Create a new sharing link for an item.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link"
} -->
