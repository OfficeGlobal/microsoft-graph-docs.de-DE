---
title: Update-Richtlinie
description: Aktualisieren von Eigenschaften in einer vorhandenen Richtlinie.
localization_priority: Normal
ms.openlocfilehash: d99aa42c4a67f6b874cbc1e266da76287388c05e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515412"
---
# <a name="update-policy"></a><span data-ttu-id="e5c92-103">Update-Richtlinie</span><span class="sxs-lookup"><span data-stu-id="e5c92-103">Update Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5c92-104">Aktualisieren von Eigenschaften in einer vorhandenen [Richtlinie](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="e5c92-104">Update properties in a preexisting [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e5c92-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e5c92-105">Permissions</span></span>
<span data-ttu-id="e5c92-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5c92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5c92-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e5c92-108">Permission type</span></span>      | <span data-ttu-id="e5c92-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e5c92-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5c92-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e5c92-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e5c92-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e5c92-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e5c92-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e5c92-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5c92-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e5c92-113">Not supported.</span></span>    |
|<span data-ttu-id="e5c92-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e5c92-114">Application</span></span> | <span data-ttu-id="e5c92-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e5c92-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5c92-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e5c92-116">HTTP request</span></span>

```http
PATCH /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e5c92-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e5c92-117">Request headers</span></span>
| <span data-ttu-id="e5c92-118">Name</span><span class="sxs-lookup"><span data-stu-id="e5c92-118">Name</span></span>       | <span data-ttu-id="e5c92-119">Typ</span><span class="sxs-lookup"><span data-stu-id="e5c92-119">Type</span></span> | <span data-ttu-id="e5c92-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e5c92-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e5c92-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5c92-121">Authorization</span></span>  | <span data-ttu-id="e5c92-122">string</span><span class="sxs-lookup"><span data-stu-id="e5c92-122">string</span></span>  | <span data-ttu-id="e5c92-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e5c92-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e5c92-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e5c92-125">Content-Type</span></span> | <span data-ttu-id="e5c92-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5c92-126">application/json</span></span>  | <span data-ttu-id="e5c92-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e5c92-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5c92-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e5c92-129">Request body</span></span>
<span data-ttu-id="e5c92-130">Geben Sie im Textkörper Anforderung ein JSON-Objekt mit den Parametern, die aktualisiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="e5c92-130">In the request body, provide a JSON object with the parameters that need to be updated.</span></span> <span data-ttu-id="e5c92-131">Die folgende Tabelle zeigt die möglichen Parameter.</span><span class="sxs-lookup"><span data-stu-id="e5c92-131">The following table shows the possible parameters.</span></span>

| <span data-ttu-id="e5c92-132">Parameter</span><span class="sxs-lookup"><span data-stu-id="e5c92-132">Parameter</span></span>    | <span data-ttu-id="e5c92-133">Typ</span><span class="sxs-lookup"><span data-stu-id="e5c92-133">Type</span></span>   |<span data-ttu-id="e5c92-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e5c92-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5c92-135">definition</span><span class="sxs-lookup"><span data-stu-id="e5c92-135">definition</span></span>|<span data-ttu-id="e5c92-136">String</span><span class="sxs-lookup"><span data-stu-id="e5c92-136">String</span></span>|<span data-ttu-id="e5c92-137">Die stringified Version des [Richtlinienobjekts](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="e5c92-137">The stringified version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="e5c92-138">displayName</span><span class="sxs-lookup"><span data-stu-id="e5c92-138">displayName</span></span>|<span data-ttu-id="e5c92-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e5c92-139">String</span></span>|<span data-ttu-id="e5c92-140">Ein benutzerdefinierter Name für die Richtlinie ein.</span><span class="sxs-lookup"><span data-stu-id="e5c92-140">A custom name for the policy.</span></span>|
|<span data-ttu-id="e5c92-141">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="e5c92-141">isOrganizationDefault</span></span>|<span data-ttu-id="e5c92-142">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e5c92-142">Boolean</span></span>|<span data-ttu-id="e5c92-143">Gibt an, ob diese Richtlinie standardmäßig angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="e5c92-143">Specifies if this policy is applied by default.</span></span>|
|<span data-ttu-id="e5c92-144">type</span><span class="sxs-lookup"><span data-stu-id="e5c92-144">type</span></span>|<span data-ttu-id="e5c92-145">String</span><span class="sxs-lookup"><span data-stu-id="e5c92-145">String</span></span>|<span data-ttu-id="e5c92-146">Gibt den Typ der Richtlinie an.</span><span class="sxs-lookup"><span data-stu-id="e5c92-146">Specifies the type of policy.</span></span> <span data-ttu-id="e5c92-147">Derzeit muss "TokenLifetimePolicy"</span><span class="sxs-lookup"><span data-stu-id="e5c92-147">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="e5c92-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="e5c92-148">Response</span></span>

<span data-ttu-id="e5c92-149">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e5c92-149">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="e5c92-150">Wenn Sie nicht erfolgreich ist, ein `4xx` mit bestimmten Details entsprechende Fehlermeldung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e5c92-150">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="e5c92-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e5c92-151">Example</span></span>
<span data-ttu-id="e5c92-152">Im folgende Beispiel wird die Definition der Richtlinie Gültigkeitsdauer von token aktualisiert und platziert es als Standard Organisation.</span><span class="sxs-lookup"><span data-stu-id="e5c92-152">The following example updates the definition of the token lifetime policy and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="e5c92-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e5c92-153">Request</span></span>
<span data-ttu-id="e5c92-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e5c92-154">Here is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/{id}
Content-Type: application/json
{
    "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
    "isOrganizationDefault":true
}
```

##### <a name="response"></a><span data-ttu-id="e5c92-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="e5c92-155">Response</span></span>
<span data-ttu-id="e5c92-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e5c92-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
