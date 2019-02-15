---
title: Löschen der APP aus dem Team
description: Deinstalliert eine APP aus dem angegebenen Team.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: aa75f72375432609afb748959cb82ff63fa1b721
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057022"
---
# <a name="delete-app-from-team"></a><span data-ttu-id="9d3f1-103">Löschen der APP aus dem Team</span><span class="sxs-lookup"><span data-stu-id="9d3f1-103">Delete app from team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d3f1-104">Deinstalliert eine [App](../resources/teamsappinstallation.md) aus dem angegebenen [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="9d3f1-104">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

><span data-ttu-id="9d3f1-105">**Hinweis:** Wenn Sie Anwendungsberechtigungen verwenden, tritt ein bekanntes Problem auf.</span><span class="sxs-lookup"><span data-stu-id="9d3f1-105">**Note:** If you're using application permissions, a known issue will occur.</span></span> <span data-ttu-id="9d3f1-106">Einzelheiten hierzu finden Sie unter [bekannte Probleme](graph/concepts/known-issues.md).</span><span class="sxs-lookup"><span data-stu-id="9d3f1-106">For details, see [known issues](graph/concepts/known-issues.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9d3f1-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9d3f1-107">Permissions</span></span>
<span data-ttu-id="9d3f1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d3f1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d3f1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9d3f1-110">Permission type</span></span>      | <span data-ttu-id="9d3f1-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9d3f1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d3f1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9d3f1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9d3f1-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d3f1-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9d3f1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9d3f1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d3f1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9d3f1-115">Not supported.</span></span>    |
|<span data-ttu-id="9d3f1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9d3f1-116">Application</span></span> | <span data-ttu-id="9d3f1-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d3f1-117">Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="9d3f1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d3f1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9d3f1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9d3f1-119">Request headers</span></span>
| <span data-ttu-id="9d3f1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9d3f1-120">Header</span></span>       | <span data-ttu-id="9d3f1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="9d3f1-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9d3f1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d3f1-122">Authorization</span></span>  | <span data-ttu-id="9d3f1-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9d3f1-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9d3f1-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9d3f1-125">Request body</span></span>
<span data-ttu-id="9d3f1-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9d3f1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d3f1-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d3f1-127">Response</span></span>

<span data-ttu-id="9d3f1-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9d3f1-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d3f1-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9d3f1-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9d3f1-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d3f1-131">Request</span></span>
<span data-ttu-id="9d3f1-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9d3f1-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}
```
#### <a name="response"></a><span data-ttu-id="9d3f1-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d3f1-133">Response</span></span>
<span data-ttu-id="9d3f1-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9d3f1-134">The following is an example of the response.</span></span> <span data-ttu-id="9d3f1-135">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="9d3f1-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9d3f1-136">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9d3f1-136">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/teamsappinstallation-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
