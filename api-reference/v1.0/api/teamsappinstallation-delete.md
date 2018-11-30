---
title: Löschen von app-Teams
description: Deinstalliert eine app aus dem angegebenen Team.
ms.openlocfilehash: a1ba2ce7234796e3a2df508d40432a15690b1a63
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016989"
---
# <a name="delete-app-from-team"></a><span data-ttu-id="fe67f-103">Löschen von app-Teams</span><span class="sxs-lookup"><span data-stu-id="fe67f-103">Delete app from team</span></span>



<span data-ttu-id="fe67f-104">Deinstalliert eine [app](../resources/teamsappinstallation.md) aus dem angegebenen [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="fe67f-104">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fe67f-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fe67f-105">Permissions</span></span>
<span data-ttu-id="fe67f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe67f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe67f-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fe67f-108">Permission type</span></span>      | <span data-ttu-id="fe67f-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fe67f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe67f-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fe67f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fe67f-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe67f-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fe67f-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fe67f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe67f-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fe67f-113">Not supported.</span></span>    |
|<span data-ttu-id="fe67f-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fe67f-114">Application</span></span> | <span data-ttu-id="fe67f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fe67f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe67f-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fe67f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fe67f-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fe67f-117">Request headers</span></span>
| <span data-ttu-id="fe67f-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fe67f-118">Header</span></span>       | <span data-ttu-id="fe67f-119">Wert</span><span class="sxs-lookup"><span data-stu-id="fe67f-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fe67f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe67f-120">Authorization</span></span>  | <span data-ttu-id="fe67f-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fe67f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fe67f-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fe67f-123">Request body</span></span>
<span data-ttu-id="fe67f-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fe67f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe67f-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="fe67f-125">Response</span></span>

<span data-ttu-id="fe67f-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fe67f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe67f-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fe67f-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fe67f-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fe67f-129">Request</span></span>
<span data-ttu-id="fe67f-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fe67f-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}
```
#### <a name="response"></a><span data-ttu-id="fe67f-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="fe67f-131">Response</span></span>
<span data-ttu-id="fe67f-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fe67f-132">The following is an example of the response.</span></span> <span data-ttu-id="fe67f-133">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="fe67f-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fe67f-134">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fe67f-134">All of the properties will be returned from an actual call.</span></span>
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
