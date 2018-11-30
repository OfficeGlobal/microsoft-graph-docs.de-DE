---
title: Aktualisieren einer app in einem team
description: Führt ein Upgrade für eine app-Installation in ein team
ms.openlocfilehash: 37f42a307b2f86e7a447e3df05030e94495eaa6b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016659"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="87ac8-103">Aktualisieren einer app in einem team</span><span class="sxs-lookup"><span data-stu-id="87ac8-103">Upgrade an app in a team</span></span>



<span data-ttu-id="87ac8-104">Führt ein Upgrade einer [app-Installation](../resources/teamsappinstallation.md) in einem [Team](../resources/team.md) auf die neueste Version der app.</span><span class="sxs-lookup"><span data-stu-id="87ac8-104">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="87ac8-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="87ac8-105">Permissions</span></span>

<span data-ttu-id="87ac8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87ac8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87ac8-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="87ac8-108">Permission type</span></span>      | <span data-ttu-id="87ac8-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="87ac8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87ac8-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="87ac8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="87ac8-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87ac8-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="87ac8-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="87ac8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87ac8-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87ac8-113">Not supported.</span></span>    |
|<span data-ttu-id="87ac8-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="87ac8-114">Application</span></span> | <span data-ttu-id="87ac8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87ac8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="87ac8-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="87ac8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="87ac8-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="87ac8-117">Request headers</span></span>
| <span data-ttu-id="87ac8-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="87ac8-118">Header</span></span>       | <span data-ttu-id="87ac8-119">Wert</span><span class="sxs-lookup"><span data-stu-id="87ac8-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="87ac8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="87ac8-120">Authorization</span></span>  | <span data-ttu-id="87ac8-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="87ac8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="87ac8-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="87ac8-123">Request body</span></span>
<span data-ttu-id="87ac8-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="87ac8-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87ac8-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="87ac8-125">Response</span></span>

<span data-ttu-id="87ac8-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="87ac8-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87ac8-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="87ac8-128">Example</span></span>

#### <a name="request"></a><span data-ttu-id="87ac8-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="87ac8-129">Request</span></span>
<span data-ttu-id="87ac8-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="87ac8-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
#### <a name="response"></a><span data-ttu-id="87ac8-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="87ac8-131">Response</span></span>
<span data-ttu-id="87ac8-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="87ac8-132">The following is an example of the response.</span></span> 

><span data-ttu-id="87ac8-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="87ac8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
