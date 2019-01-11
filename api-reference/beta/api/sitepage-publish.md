---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: Seite "Veröffentlichen"
localization_priority: Normal
ms.openlocfilehash: 0b98f22dda2c4b08d04150b8b24126fdff5ca505
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836155"
---
# <a name="sitepage-publish"></a><span data-ttu-id="ff0b9-102">SitePage: Veröffentlichen</span><span class="sxs-lookup"><span data-stu-id="ff0b9-102">sitePage: publish</span></span>

> <span data-ttu-id="ff0b9-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ff0b9-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff0b9-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ff0b9-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ff0b9-105">Veröffentlichen Sie die neueste Version einer Ressource [SitePage][] , wodurch die Version der Seite für alle Benutzer verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="ff0b9-105">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="ff0b9-106">Wenn die Seite ausgecheckt ist, überprüfen Sie auf der Seite, und veröffentlichen Sie es.</span><span class="sxs-lookup"><span data-stu-id="ff0b9-106">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="ff0b9-107">Wenn die Seite mit dem Anrufer dieser API aktiviert ist, wird die Seite automatisch eingecheckt und veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="ff0b9-107">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="ff0b9-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ff0b9-109">Permissions</span></span>

<span data-ttu-id="ff0b9-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff0b9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff0b9-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ff0b9-112">Permission type</span></span>      | <span data-ttu-id="ff0b9-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ff0b9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff0b9-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ff0b9-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ff0b9-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff0b9-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ff0b9-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ff0b9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff0b9-117">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff0b9-117">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ff0b9-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ff0b9-118">Application</span></span> | <span data-ttu-id="ff0b9-119">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff0b9-119">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff0b9-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff0b9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="ff0b9-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ff0b9-121">Request body</span></span>

<span data-ttu-id="ff0b9-122">Diese Meldung hat keinen Anforderungstext.</span><span class="sxs-lookup"><span data-stu-id="ff0b9-122">This message does not have a request body.</span></span> <span data-ttu-id="ff0b9-123">Alle Anforderungstext gesendet werden ignoriert.</span><span class="sxs-lookup"><span data-stu-id="ff0b9-123">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="ff0b9-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff0b9-124">Response</span></span>

<span data-ttu-id="ff0b9-125">Wenn diese Methode erfolgreich verläuft, gibt der API-Anruf eine `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="ff0b9-125">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


<!-- {
  "type": "#page.annotation",
  "description": "Publish a page.",
  "keywords": "publish page",
  "section": "documentation",
  "tocPath": "Pages/Publish"
} -->
