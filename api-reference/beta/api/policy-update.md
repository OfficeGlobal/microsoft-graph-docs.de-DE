---
title: Update-Richtlinie
description: Aktualisieren von Eigenschaften in einer vorhandenen Richtlinie.
localization_priority: Normal
ms.openlocfilehash: 2992f2f76c0e8b213ad8aabca1bfd0fe59883989
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857155"
---
# <a name="update-policy"></a><span data-ttu-id="7199a-103">Update-Richtlinie</span><span class="sxs-lookup"><span data-stu-id="7199a-103">Update Policy</span></span>

> <span data-ttu-id="7199a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7199a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7199a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7199a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7199a-106">Aktualisieren von Eigenschaften in einer vorhandenen [Richtlinie](../resources/policy.md).</span><span class="sxs-lookup"><span data-stu-id="7199a-106">Update properties in a preexisting [policy](../resources/policy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7199a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7199a-107">Permissions</span></span>
<span data-ttu-id="7199a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7199a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7199a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7199a-110">Permission type</span></span>      | <span data-ttu-id="7199a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7199a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7199a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7199a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7199a-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7199a-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7199a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7199a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7199a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7199a-115">Not supported.</span></span>    |
|<span data-ttu-id="7199a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7199a-116">Application</span></span> | <span data-ttu-id="7199a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7199a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7199a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7199a-118">HTTP request</span></span>

```http
PATCH /policies/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7199a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7199a-119">Request headers</span></span>
| <span data-ttu-id="7199a-120">Name</span><span class="sxs-lookup"><span data-stu-id="7199a-120">Name</span></span>       | <span data-ttu-id="7199a-121">Typ</span><span class="sxs-lookup"><span data-stu-id="7199a-121">Type</span></span> | <span data-ttu-id="7199a-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7199a-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7199a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7199a-123">Authorization</span></span>  | <span data-ttu-id="7199a-124">string</span><span class="sxs-lookup"><span data-stu-id="7199a-124">string</span></span>  | <span data-ttu-id="7199a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7199a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7199a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7199a-127">Content-Type</span></span> | <span data-ttu-id="7199a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7199a-128">application/json</span></span>  | <span data-ttu-id="7199a-p104">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7199a-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7199a-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7199a-131">Request body</span></span>
<span data-ttu-id="7199a-132">Geben Sie im Textkörper Anforderung ein JSON-Objekt mit den Parametern, die aktualisiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="7199a-132">In the request body, provide a JSON object with the parameters that need to be updated.</span></span> <span data-ttu-id="7199a-133">Die folgende Tabelle zeigt die möglichen Parameter.</span><span class="sxs-lookup"><span data-stu-id="7199a-133">The following table shows the possible parameters.</span></span>

| <span data-ttu-id="7199a-134">Parameter</span><span class="sxs-lookup"><span data-stu-id="7199a-134">Parameter</span></span>    | <span data-ttu-id="7199a-135">Typ</span><span class="sxs-lookup"><span data-stu-id="7199a-135">Type</span></span>   |<span data-ttu-id="7199a-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7199a-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7199a-137">definition</span><span class="sxs-lookup"><span data-stu-id="7199a-137">definition</span></span>|<span data-ttu-id="7199a-138">String</span><span class="sxs-lookup"><span data-stu-id="7199a-138">String</span></span>|<span data-ttu-id="7199a-139">Die stringified Version des [Richtlinienobjekts](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="7199a-139">The stringified version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="7199a-140">displayName</span><span class="sxs-lookup"><span data-stu-id="7199a-140">displayName</span></span>|<span data-ttu-id="7199a-141">String</span><span class="sxs-lookup"><span data-stu-id="7199a-141">String</span></span>|<span data-ttu-id="7199a-142">Ein benutzerdefinierter Name für die Richtlinie ein.</span><span class="sxs-lookup"><span data-stu-id="7199a-142">A custom name for the policy.</span></span>|
|<span data-ttu-id="7199a-143">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="7199a-143">isOrganizationDefault</span></span>|<span data-ttu-id="7199a-144">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7199a-144">Boolean</span></span>|<span data-ttu-id="7199a-145">Gibt an, ob diese Richtlinie standardmäßig angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="7199a-145">Specifies if this policy is applied by default.</span></span>|
|<span data-ttu-id="7199a-146">type</span><span class="sxs-lookup"><span data-stu-id="7199a-146">type</span></span>|<span data-ttu-id="7199a-147">String</span><span class="sxs-lookup"><span data-stu-id="7199a-147">String</span></span>|<span data-ttu-id="7199a-148">Gibt den Typ der Richtlinie an.</span><span class="sxs-lookup"><span data-stu-id="7199a-148">Specifies the type of policy.</span></span> <span data-ttu-id="7199a-149">Derzeit muss "TokenLifetimePolicy"</span><span class="sxs-lookup"><span data-stu-id="7199a-149">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="7199a-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="7199a-150">Response</span></span>

<span data-ttu-id="7199a-151">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7199a-151">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="7199a-152">Wenn Sie nicht erfolgreich ist, ein `4xx` mit bestimmten Details entsprechende Fehlermeldung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7199a-152">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="7199a-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7199a-153">Example</span></span>
<span data-ttu-id="7199a-154">Im folgende Beispiel wird die Definition der Richtlinie Gültigkeitsdauer von token aktualisiert und platziert es als Standard Organisation.</span><span class="sxs-lookup"><span data-stu-id="7199a-154">The following example updates the definition of the token lifetime policy and sets it as the organization default.</span></span>

##### <a name="request"></a><span data-ttu-id="7199a-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7199a-155">Request</span></span>
<span data-ttu-id="7199a-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7199a-156">Here is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/{id}
Content-Type: application/json
{
    "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
    "isOrganizationDefault":true
}
```

##### <a name="response"></a><span data-ttu-id="7199a-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="7199a-157">Response</span></span>
<span data-ttu-id="7199a-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7199a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 204 No Content
```
