---
title: App zu Team hinzufügen
description: Installiert eine APP für das angegebene Team.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 261d186e23b516e58a428ecfdd2883f7a3bc111d
ms.sourcegitcommit: 4e9acb8029aca36dfade509a25f1111e1bd0ec6d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/16/2019
ms.locfileid: "30070827"
---
# <a name="add-app-to-team"></a><span data-ttu-id="371b9-103">App zu Team hinzufügen</span><span class="sxs-lookup"><span data-stu-id="371b9-103">Add app to team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="371b9-104">Installiert eine [App](../resources/teamsapp.md) für das angegebene [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="371b9-104">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

><span data-ttu-id="371b9-105">**Hinweis:** Wenn Sie Anwendungsberechtigungen verwenden, tritt ein bekanntes Problem auf.</span><span class="sxs-lookup"><span data-stu-id="371b9-105">**Note:** If you're using application permissions, a known issue will occur.</span></span> <span data-ttu-id="371b9-106">Einzelheiten hierzu finden Sie unter [bekannte Probleme](/graph/known-issues).</span><span class="sxs-lookup"><span data-stu-id="371b9-106">For details, see [known issues](/graph/known-issues).</span></span>

## <a name="permissions"></a><span data-ttu-id="371b9-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="371b9-107">Permissions</span></span>
<span data-ttu-id="371b9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="371b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="371b9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="371b9-110">Permission type</span></span>      | <span data-ttu-id="371b9-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="371b9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="371b9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="371b9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="371b9-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="371b9-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="371b9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="371b9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="371b9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="371b9-115">Not supported.</span></span>    |
|<span data-ttu-id="371b9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="371b9-116">Application</span></span> | <span data-ttu-id="371b9-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="371b9-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="371b9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="371b9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="371b9-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="371b9-119">Request headers</span></span>
| <span data-ttu-id="371b9-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="371b9-120">Header</span></span>       | <span data-ttu-id="371b9-121">Wert</span><span class="sxs-lookup"><span data-stu-id="371b9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="371b9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="371b9-122">Authorization</span></span>  | <span data-ttu-id="371b9-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="371b9-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="371b9-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="371b9-125">Request body</span></span>

| <span data-ttu-id="371b9-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="371b9-126">Property</span></span>     | <span data-ttu-id="371b9-127">Typ</span><span class="sxs-lookup"><span data-stu-id="371b9-127">Type</span></span>   |<span data-ttu-id="371b9-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="371b9-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="371b9-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="371b9-129">teamsApp</span></span>|<span data-ttu-id="371b9-130">String</span><span class="sxs-lookup"><span data-stu-id="371b9-130">String</span></span>|<span data-ttu-id="371b9-131">Die ID der hinzuzufügenden app.</span><span class="sxs-lookup"><span data-stu-id="371b9-131">The id of the app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="371b9-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="371b9-132">Response</span></span>

<span data-ttu-id="371b9-133">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="371b9-133">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="371b9-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="371b9-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="371b9-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="371b9-135">Request</span></span>
<span data-ttu-id="371b9-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="371b9-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/installedApps
{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
#### <a name="response"></a><span data-ttu-id="371b9-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="371b9-137">Response</span></span>
<span data-ttu-id="371b9-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="371b9-138">The following is an example of the response.</span></span> <span data-ttu-id="371b9-139">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="371b9-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="371b9-140">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="371b9-140">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
}
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
    "Error: /api-reference/beta/api/teamsappinstallation-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

## <a name="see-also"></a><span data-ttu-id="371b9-141">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="371b9-141">See also</span></span>

