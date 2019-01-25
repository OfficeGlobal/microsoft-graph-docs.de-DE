---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: Seite "Veröffentlichen"
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a00a69542c2b59b1b268433b08656c87d194feb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507530"
---
# <a name="sitepage-publish"></a><span data-ttu-id="2c27f-102">SitePage: Veröffentlichen</span><span class="sxs-lookup"><span data-stu-id="2c27f-102">sitePage: publish</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c27f-103">Veröffentlichen Sie die neueste Version einer Ressource [SitePage][] , wodurch die Version der Seite für alle Benutzer verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="2c27f-103">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="2c27f-104">Wenn die Seite ausgecheckt ist, überprüfen Sie auf der Seite, und veröffentlichen Sie es.</span><span class="sxs-lookup"><span data-stu-id="2c27f-104">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="2c27f-105">Wenn die Seite mit dem Anrufer dieser API aktiviert ist, wird die Seite automatisch eingecheckt und veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="2c27f-105">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="2c27f-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2c27f-107">Permissions</span></span>

<span data-ttu-id="2c27f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c27f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c27f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2c27f-110">Permission type</span></span>      | <span data-ttu-id="2c27f-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2c27f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c27f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2c27f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2c27f-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c27f-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2c27f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2c27f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c27f-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c27f-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="2c27f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2c27f-116">Application</span></span> | <span data-ttu-id="2c27f-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c27f-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c27f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2c27f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="2c27f-119">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2c27f-119">Request body</span></span>

<span data-ttu-id="2c27f-120">Diese Meldung hat keinen Anforderungstext.</span><span class="sxs-lookup"><span data-stu-id="2c27f-120">This message does not have a request body.</span></span> <span data-ttu-id="2c27f-121">Alle Anforderungstext gesendet werden ignoriert.</span><span class="sxs-lookup"><span data-stu-id="2c27f-121">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="2c27f-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="2c27f-122">Response</span></span>

<span data-ttu-id="2c27f-123">Wenn diese Methode erfolgreich verläuft, gibt der API-Anruf eine `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="2c27f-123">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


<!--
{
  "type": "#page.annotation",
  "description": "Publish a page.",
  "keywords": "publish page",
  "section": "documentation",
  "tocPath": "Pages/Publish",
  "suppressions": [
    "Error: /api-reference/beta/api/sitepage-publish.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
