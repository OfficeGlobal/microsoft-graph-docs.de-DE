---
title: Löschen von app-Teams
description: Deinstalliert eine app aus dem angegebenen Team.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 55e5b1a87c010a0e9a36353d8da82a8433dd3ebd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983576"
---
# <a name="delete-app-from-team"></a><span data-ttu-id="31161-103">Löschen von app-Teams</span><span class="sxs-lookup"><span data-stu-id="31161-103">Delete app from team</span></span>

> <span data-ttu-id="31161-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="31161-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31161-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="31161-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="31161-106">Deinstalliert eine [app](../resources/teamsappinstallation.md) aus dem angegebenen [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="31161-106">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="31161-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="31161-107">Permissions</span></span>
<span data-ttu-id="31161-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31161-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31161-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="31161-110">Permission type</span></span>      | <span data-ttu-id="31161-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="31161-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31161-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="31161-112">Delegated (work or school account)</span></span> | <span data-ttu-id="31161-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31161-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="31161-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="31161-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31161-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="31161-115">Not supported.</span></span>    |
|<span data-ttu-id="31161-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="31161-116">Application</span></span> | <span data-ttu-id="31161-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="31161-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="31161-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="31161-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="31161-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="31161-119">Request headers</span></span>
| <span data-ttu-id="31161-120">Header</span><span class="sxs-lookup"><span data-stu-id="31161-120">Header</span></span>       | <span data-ttu-id="31161-121">Wert</span><span class="sxs-lookup"><span data-stu-id="31161-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="31161-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="31161-122">Authorization</span></span>  | <span data-ttu-id="31161-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="31161-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="31161-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="31161-125">Request body</span></span>
<span data-ttu-id="31161-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="31161-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31161-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="31161-127">Response</span></span>

<span data-ttu-id="31161-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="31161-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31161-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="31161-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="31161-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="31161-131">Request</span></span>
<span data-ttu-id="31161-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="31161-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}
```
#### <a name="response"></a><span data-ttu-id="31161-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="31161-133">Response</span></span>
<span data-ttu-id="31161-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="31161-134">The following is an example of the response.</span></span> <span data-ttu-id="31161-135">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="31161-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="31161-136">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="31161-136">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
