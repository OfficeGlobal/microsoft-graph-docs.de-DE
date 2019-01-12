---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Wiederherstellen einer früheren Version eines SharePoint-Listenelements
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b7c81022ebcb4f7afe02520c48f7cfbf103b2943
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983002"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="a5561-102">Frühere Version eines SharePoint-Listenelements wiederherstellen</span><span class="sxs-lookup"><span data-stu-id="a5561-102">Restore a previous version of a ListItem</span></span>

> <span data-ttu-id="a5561-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a5561-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5561-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a5561-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a5561-105">Stellen Sie eine frühere Version eines Listenelements als aktuelle Version wieder her.</span><span class="sxs-lookup"><span data-stu-id="a5561-105">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="a5561-106">Dadurch wird eine neue Version mit dem Inhalt der vorherigen Version erstellt, aber alle vorhandenen Versionen des Elements bleiben erhalten.</span><span class="sxs-lookup"><span data-stu-id="a5561-106">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5561-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a5561-107">Permissions</span></span>

<span data-ttu-id="a5561-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5561-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="a5561-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a5561-110">Permission type</span></span>             |         <span data-ttu-id="a5561-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a5561-111">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="a5561-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a5561-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a5561-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="a5561-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="a5561-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a5561-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5561-115">N/V</span><span class="sxs-lookup"><span data-stu-id="a5561-115">n/a</span></span>                                                          |
| <span data-ttu-id="a5561-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a5561-116">Application</span></span>                            | <span data-ttu-id="a5561-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="a5561-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5561-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5561-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="a5561-119">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a5561-119">Request body</span></span>

<span data-ttu-id="a5561-120">Es ist kein Anforderungstexts erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a5561-120">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="a5561-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a5561-121">Example</span></span>

<span data-ttu-id="a5561-122">In diesem Beispiel wird eine Version eines von `{item-id}` und `{version-id}` identifizierten Listenelements wiederhergestellt.</span><span class="sxs-lookup"><span data-stu-id="a5561-122">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="a5561-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5561-123">Response</span></span>

<span data-ttu-id="a5561-124">Wenn diese Methode erfolgreich verläuft, gibt der API-Anruf eine `204 No content` zurück.</span><span class="sxs-lookup"><span data-stu-id="a5561-124">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
