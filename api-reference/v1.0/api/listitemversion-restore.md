---
title: Frühere Version eines SharePoint-Listenelements wiederherstellen
description: Stellen Sie eine frühere Version eines Listenelements als aktuelle Version wieder her. Dadurch wird eine neue Version mit dem Inhalt der vorherigen Version erstellt, aber alle vorhandenen Versionen des Elements bleiben erhalten.
localization_priority: Normal
ms.openlocfilehash: 6fb315986a8dc22363e22235f8cf65e0cbc21fed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866962"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="13656-104">Frühere Version eines SharePoint-Listenelements wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="13656-104">Restore a previous version of a ListItem</span></span>

<span data-ttu-id="13656-105">Stellen Sie eine frühere Version eines Listenelements als aktuelle Version wieder her.</span><span class="sxs-lookup"><span data-stu-id="13656-105">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="13656-106">Dadurch wird eine neue Version mit dem Inhalt der vorherigen Version erstellt, aber alle vorhandenen Versionen des Elements bleiben erhalten.</span><span class="sxs-lookup"><span data-stu-id="13656-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="13656-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="13656-107">Permissions</span></span>

<span data-ttu-id="13656-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13656-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="13656-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="13656-110">Permission type</span></span>             |         <span data-ttu-id="13656-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="13656-111">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="13656-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="13656-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="13656-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="13656-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="13656-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="13656-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13656-115">N/V</span><span class="sxs-lookup"><span data-stu-id="13656-115">n/a</span></span>                                                          |
| <span data-ttu-id="13656-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="13656-116">Application</span></span>                            | <span data-ttu-id="13656-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="13656-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="13656-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="13656-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="13656-119">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="13656-119">Request body</span></span>

<span data-ttu-id="13656-120">Es ist kein Anforderungstexts erforderlich.</span><span class="sxs-lookup"><span data-stu-id="13656-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="13656-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="13656-121">Example</span></span>

<span data-ttu-id="13656-122">In diesem Beispiel wird eine Version eines von `{item-id}` und `{version-id}` identifizierten Listenelements wiederhergestellt.</span><span class="sxs-lookup"><span data-stu-id="13656-122">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite sites.readwrite.all", "target": "action", "tags": "service.graph service.sharepoint" } -->

```http
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="13656-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="13656-123">Response</span></span>

<span data-ttu-id="13656-124">Wenn diese Methode erfolgreich verläuft, gibt der API-Anruf eine `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="13656-124">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
