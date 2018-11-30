---
title: Löschen von app-Teams
description: Deinstalliert eine app aus dem angegebenen Team.
ms.openlocfilehash: e126dca3812e6b6323820eaf1d230243aebc93e8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064570"
---
# <a name="delete-app-from-team"></a><span data-ttu-id="937ff-103">Löschen von app-Teams</span><span class="sxs-lookup"><span data-stu-id="937ff-103">Delete app from team</span></span>

> <span data-ttu-id="937ff-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="937ff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="937ff-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="937ff-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="937ff-106">Deinstalliert eine [app](../resources/teamsappinstallation.md) aus dem angegebenen [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="937ff-106">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="937ff-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="937ff-107">Permissions</span></span>
<span data-ttu-id="937ff-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="937ff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="937ff-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="937ff-110">Permission type</span></span>      | <span data-ttu-id="937ff-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="937ff-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="937ff-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="937ff-112">Delegated (work or school account)</span></span> | <span data-ttu-id="937ff-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="937ff-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="937ff-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="937ff-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="937ff-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="937ff-115">Not supported.</span></span>    |
|<span data-ttu-id="937ff-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="937ff-116">Application</span></span> | <span data-ttu-id="937ff-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="937ff-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="937ff-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="937ff-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="937ff-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="937ff-119">Request headers</span></span>
| <span data-ttu-id="937ff-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="937ff-120">Header</span></span>       | <span data-ttu-id="937ff-121">Wert</span><span class="sxs-lookup"><span data-stu-id="937ff-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="937ff-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="937ff-122">Authorization</span></span>  | <span data-ttu-id="937ff-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="937ff-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="937ff-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="937ff-125">Request body</span></span>
<span data-ttu-id="937ff-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="937ff-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="937ff-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="937ff-127">Response</span></span>

<span data-ttu-id="937ff-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="937ff-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="937ff-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="937ff-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="937ff-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="937ff-131">Request</span></span>
<span data-ttu-id="937ff-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="937ff-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}
```
#### <a name="response"></a><span data-ttu-id="937ff-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="937ff-133">Response</span></span>
<span data-ttu-id="937ff-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="937ff-134">The following is an example of the response.</span></span> <span data-ttu-id="937ff-135">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="937ff-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="937ff-136">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="937ff-136">All of the properties will be returned from an actual call.</span></span>
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
