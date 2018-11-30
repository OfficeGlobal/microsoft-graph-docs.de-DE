---
title: Zuweisen der Richtlinie
description: Eine Anwendung oder ein Dienstprinzipal eine Richtlinie zugewiesen.
ms.openlocfilehash: 25dee4ac43716949125795114318d2571d5b8647
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064580"
---
# <a name="assign-policy"></a><span data-ttu-id="289f6-103">Zuweisen der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="289f6-103">Assign Policy</span></span>

> <span data-ttu-id="289f6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="289f6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="289f6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="289f6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="289f6-106">Eine Anwendung oder ein Dienstprinzipal eine [Richtlinie](../resources/policy.md) zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="289f6-106">Assigns a [policy](../resources/policy.md) to an application or service principal.</span></span>

><span data-ttu-id="289f6-107">Hinweis: Derzeit gilt richtlinienzuweisung nur Token Lebensdauer Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="289f6-107">Note: Currently, policy assignment only applies to Token lifetime Policy.</span></span> <span data-ttu-id="289f6-108">Dieser Typ der Richtlinie wird in der [Richtlinie](../resources/policy.md)beschrieben.</span><span class="sxs-lookup"><span data-stu-id="289f6-108">This type of policy is described in [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="289f6-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="289f6-109">Permissions</span></span>
<span data-ttu-id="289f6-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="289f6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="289f6-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="289f6-112">Permission type</span></span>      | <span data-ttu-id="289f6-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="289f6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="289f6-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="289f6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="289f6-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="289f6-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="289f6-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="289f6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="289f6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="289f6-117">Not supported.</span></span>    |
|<span data-ttu-id="289f6-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="289f6-118">Application</span></span> | <span data-ttu-id="289f6-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="289f6-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="289f6-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="289f6-120">HTTP request</span></span>

```http
POST /applications/{id}/policies/$ref
POST /serviceprincipals/{id}/policies/$ref
```

> <span data-ttu-id="289f6-121">Hinweis: "Id" in der Anforderung ist die Eigenschaft "Id" der Anwendung oder Dienstprinzipal, nicht die Eigenschaft "Appid".</span><span class="sxs-lookup"><span data-stu-id="289f6-121">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="289f6-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="289f6-122">Request headers</span></span>
| <span data-ttu-id="289f6-123">Name</span><span class="sxs-lookup"><span data-stu-id="289f6-123">Name</span></span>       | <span data-ttu-id="289f6-124">Typ</span><span class="sxs-lookup"><span data-stu-id="289f6-124">Type</span></span> | <span data-ttu-id="289f6-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="289f6-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="289f6-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="289f6-126">Authorization</span></span>  | <span data-ttu-id="289f6-127">string</span><span class="sxs-lookup"><span data-stu-id="289f6-127">string</span></span>  | <span data-ttu-id="289f6-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="289f6-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="289f6-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="289f6-130">Content-Type</span></span> | <span data-ttu-id="289f6-131">application/json</span><span class="sxs-lookup"><span data-stu-id="289f6-131">application/json</span></span>  | <span data-ttu-id="289f6-p105">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="289f6-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="289f6-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="289f6-134">Request body</span></span>
<span data-ttu-id="289f6-135">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des Richtlinienobjekts hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="289f6-135">In the request body, provide a JSON representation of the policy object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="289f6-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="289f6-136">Response</span></span>

<span data-ttu-id="289f6-137">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="289f6-137">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="289f6-138">Wenn Sie nicht erfolgreich ist, ein `4xx` mit bestimmten Details entsprechende Fehlermeldung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="289f6-138">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="289f6-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="289f6-139">Example</span></span>
<span data-ttu-id="289f6-140">Das folgende Beispiel weist eine Richtlinie zu einer Anwendung.</span><span class="sxs-lookup"><span data-stu-id="289f6-140">The following example assigns a policy to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="289f6-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="289f6-141">Request</span></span>
<span data-ttu-id="289f6-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="289f6-142">Here is an example of the request.</span></span>

```http
POST /applications/{id}/policies/$ref
Content-type: application/json
{
    "@odata.id":"https://graph.microsoft.com/beta/policies/{policyid}"
}
```

##### <a name="response"></a><span data-ttu-id="289f6-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="289f6-143">Response</span></span>
<span data-ttu-id="289f6-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="289f6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
