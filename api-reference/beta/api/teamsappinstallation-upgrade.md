---
title: Aktualisieren einer APP in einem Team
description: Aktualisieren einer App-Installation in einem Team
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9ef5c41c8b09512b0ee6ebb888be1df1166cf9c5
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2019
ms.locfileid: "30056980"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="2deb1-103">Aktualisieren einer APP in einem Team</span><span class="sxs-lookup"><span data-stu-id="2deb1-103">Upgrade an app in a team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2deb1-104">Aktualisiert eine [App-Installation](../resources/teamsappinstallation.md) in einem [Team](../resources/team.md) auf die neueste Version der app.</span><span class="sxs-lookup"><span data-stu-id="2deb1-104">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

><span data-ttu-id="2deb1-105">**Hinweis:** Wenn Sie Anwendungsberechtigungen verwenden, tritt ein bekanntes Problem auf.</span><span class="sxs-lookup"><span data-stu-id="2deb1-105">**Note:** If you're using application permissions, a known issue will occur.</span></span> <span data-ttu-id="2deb1-106">Einzelheiten hierzu finden Sie unter [bekannte Probleme](graph/concepts/known-issues.md).</span><span class="sxs-lookup"><span data-stu-id="2deb1-106">For details, see [known issues](graph/concepts/known-issues.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2deb1-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2deb1-107">Permissions</span></span>

<span data-ttu-id="2deb1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2deb1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2deb1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2deb1-110">Permission type</span></span>      | <span data-ttu-id="2deb1-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2deb1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2deb1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2deb1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2deb1-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2deb1-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2deb1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2deb1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2deb1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2deb1-115">Not supported.</span></span>    |
|<span data-ttu-id="2deb1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2deb1-116">Application</span></span> | <span data-ttu-id="2deb1-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2deb1-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2deb1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2deb1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="2deb1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2deb1-119">Request headers</span></span>
| <span data-ttu-id="2deb1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2deb1-120">Header</span></span>       | <span data-ttu-id="2deb1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2deb1-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2deb1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2deb1-122">Authorization</span></span>  | <span data-ttu-id="2deb1-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2deb1-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2deb1-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2deb1-125">Request body</span></span>
<span data-ttu-id="2deb1-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2deb1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2deb1-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="2deb1-127">Response</span></span>

<span data-ttu-id="2deb1-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2deb1-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2deb1-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2deb1-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2deb1-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2deb1-131">Request</span></span>
<span data-ttu-id="2deb1-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2deb1-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
#### <a name="response"></a><span data-ttu-id="2deb1-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="2deb1-133">Response</span></span>
<span data-ttu-id="2deb1-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2deb1-134">The following is an example of the response.</span></span> 

><span data-ttu-id="2deb1-p105">**Hinweis:** Das hier gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="2deb1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/teamsappinstallation-upgrade.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
