---
title: Zuweisen der Richtlinie
description: Eine Anwendung oder ein Dienstprinzipal eine Richtlinie zugewiesen.
localization_priority: Normal
ms.openlocfilehash: 15ba6a42f5c5d39caf57b25ebafc5dd4bc7990fc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528214"
---
# <a name="assign-policy"></a><span data-ttu-id="8f0f6-103">Zuweisen der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="8f0f6-103">Assign Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f0f6-104">Eine Anwendung oder ein Dienstprinzipal eine [Richtlinie](../resources/policy.md) zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="8f0f6-104">Assigns a [policy](../resources/policy.md) to an application or service principal.</span></span>

><span data-ttu-id="8f0f6-105">Hinweis: Derzeit gilt richtlinienzuweisung nur Token Lebensdauer Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="8f0f6-105">Note: Currently, policy assignment only applies to Token lifetime Policy.</span></span> <span data-ttu-id="8f0f6-106">Dieser Typ der Richtlinie wird in der [Richtlinie](../resources/policy.md)beschrieben.</span><span class="sxs-lookup"><span data-stu-id="8f0f6-106">This type of policy is described in [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8f0f6-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8f0f6-107">Permissions</span></span>
<span data-ttu-id="8f0f6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f0f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f0f6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8f0f6-110">Permission type</span></span>      | <span data-ttu-id="8f0f6-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8f0f6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f0f6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8f0f6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8f0f6-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8f0f6-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8f0f6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8f0f6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f0f6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8f0f6-115">Not supported.</span></span>    |
|<span data-ttu-id="8f0f6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8f0f6-116">Application</span></span> | <span data-ttu-id="8f0f6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8f0f6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f0f6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8f0f6-118">HTTP request</span></span>

```http
POST /applications/{id}/policies/$ref
POST /serviceprincipals/{id}/policies/$ref
```

> <span data-ttu-id="8f0f6-119">Hinweis: "Id" in der Anforderung ist die Eigenschaft "Id" der Anwendung oder Dienstprinzipal, nicht die Eigenschaft "Appid".</span><span class="sxs-lookup"><span data-stu-id="8f0f6-119">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f0f6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8f0f6-120">Request headers</span></span>
| <span data-ttu-id="8f0f6-121">Name</span><span class="sxs-lookup"><span data-stu-id="8f0f6-121">Name</span></span>       | <span data-ttu-id="8f0f6-122">Typ</span><span class="sxs-lookup"><span data-stu-id="8f0f6-122">Type</span></span> | <span data-ttu-id="8f0f6-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f0f6-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8f0f6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f0f6-124">Authorization</span></span>  | <span data-ttu-id="8f0f6-125">string</span><span class="sxs-lookup"><span data-stu-id="8f0f6-125">string</span></span>  | <span data-ttu-id="8f0f6-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8f0f6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f0f6-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8f0f6-128">Content-Type</span></span> | <span data-ttu-id="8f0f6-129">application/json</span><span class="sxs-lookup"><span data-stu-id="8f0f6-129">application/json</span></span>  | <span data-ttu-id="8f0f6-p104">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8f0f6-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f0f6-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8f0f6-132">Request body</span></span>
<span data-ttu-id="8f0f6-133">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des Richtlinienobjekts hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="8f0f6-133">In the request body, provide a JSON representation of the policy object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="8f0f6-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8f0f6-134">Response</span></span>

<span data-ttu-id="8f0f6-135">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8f0f6-135">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="8f0f6-136">Wenn Sie nicht erfolgreich ist, ein `4xx` mit bestimmten Details entsprechende Fehlermeldung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8f0f6-136">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="8f0f6-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8f0f6-137">Example</span></span>
<span data-ttu-id="8f0f6-138">Das folgende Beispiel weist eine Richtlinie zu einer Anwendung.</span><span class="sxs-lookup"><span data-stu-id="8f0f6-138">The following example assigns a policy to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="8f0f6-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8f0f6-139">Request</span></span>
<span data-ttu-id="8f0f6-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8f0f6-140">Here is an example of the request.</span></span>

```http
POST /applications/{id}/policies/$ref
Content-type: application/json
{
    "@odata.id":"https://graph.microsoft.com/beta/policies/{policyid}"
}
```

##### <a name="response"></a><span data-ttu-id="8f0f6-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="8f0f6-141">Response</span></span>
<span data-ttu-id="8f0f6-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8f0f6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-assign.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
