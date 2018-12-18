---
title: Aktualisieren einer app in einem team
description: Führt ein Upgrade für eine app-Installation in ein team
author: nkramer
ms.openlocfilehash: 1e3ebffa9786d170424dd60618f553c515154140
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341440"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="8dcae-103">Aktualisieren einer app in einem team</span><span class="sxs-lookup"><span data-stu-id="8dcae-103">Upgrade an app in a team</span></span>

> <span data-ttu-id="8dcae-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8dcae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8dcae-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8dcae-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8dcae-106">Führt ein Upgrade einer [app-Installation](../resources/teamsappinstallation.md) in einem [Team](../resources/team.md) auf die neueste Version der app.</span><span class="sxs-lookup"><span data-stu-id="8dcae-106">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="8dcae-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8dcae-107">Permissions</span></span>

<span data-ttu-id="8dcae-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dcae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8dcae-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8dcae-110">Permission type</span></span>      | <span data-ttu-id="8dcae-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8dcae-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8dcae-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8dcae-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8dcae-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dcae-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8dcae-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8dcae-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8dcae-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8dcae-115">Not supported.</span></span>    |
|<span data-ttu-id="8dcae-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8dcae-116">Application</span></span> | <span data-ttu-id="8dcae-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8dcae-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8dcae-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8dcae-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="8dcae-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8dcae-119">Request headers</span></span>
| <span data-ttu-id="8dcae-120">Header</span><span class="sxs-lookup"><span data-stu-id="8dcae-120">Header</span></span>       | <span data-ttu-id="8dcae-121">Wert</span><span class="sxs-lookup"><span data-stu-id="8dcae-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8dcae-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8dcae-122">Authorization</span></span>  | <span data-ttu-id="8dcae-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8dcae-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8dcae-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8dcae-125">Request body</span></span>
<span data-ttu-id="8dcae-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8dcae-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8dcae-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="8dcae-127">Response</span></span>

<span data-ttu-id="8dcae-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8dcae-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8dcae-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8dcae-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8dcae-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8dcae-131">Request</span></span>
<span data-ttu-id="8dcae-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8dcae-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
#### <a name="response"></a><span data-ttu-id="8dcae-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="8dcae-133">Response</span></span>
<span data-ttu-id="8dcae-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8dcae-134">The following is an example of the response.</span></span> 

><span data-ttu-id="8dcae-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="8dcae-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
