---
title: Richtlinie erstellen
description: Erstellen Sie ein neues Gruppenrichtlinienobjekt durch Anzeigename, Richtlinientyp und Beschreibung der Richtlinie angeben.
localization_priority: Normal
ms.openlocfilehash: 4850b2899bfd9add703af912f16602960b2657f4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831234"
---
# <a name="create-policy"></a><span data-ttu-id="0e040-103">Richtlinie erstellen</span><span class="sxs-lookup"><span data-stu-id="0e040-103">Create Policy</span></span>

> <span data-ttu-id="0e040-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0e040-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e040-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0e040-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0e040-106">Erstellen [Sie ein neues Gruppenrichtlinienobjekt](../resources/policy.md) durch Anzeigename, Richtlinientyp und Beschreibung der Richtlinie angeben.</span><span class="sxs-lookup"><span data-stu-id="0e040-106">Create a new [policy](../resources/policy.md) object by specifying display name, policy type, and policy description.</span></span>

><span data-ttu-id="0e040-107">Hinweis: Die Richtliniendetails werden vor dem Speichern überprüft.</span><span class="sxs-lookup"><span data-stu-id="0e040-107">Note: The policy details will be validated before being stored.</span></span> <span data-ttu-id="0e040-108">Wenn sie die Überprüfung nicht bestanden hat, wird ein 400 Ungültige Anforderung zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="0e040-108">If it does not pass validation, a 400 Bad Request will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e040-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0e040-109">Permissions</span></span>
<span data-ttu-id="0e040-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e040-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e040-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0e040-112">Permission type</span></span>      | <span data-ttu-id="0e040-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0e040-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e040-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0e040-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0e040-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0e040-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0e040-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0e040-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e040-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e040-117">Not supported.</span></span>    |
|<span data-ttu-id="0e040-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0e040-118">Application</span></span> | <span data-ttu-id="0e040-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e040-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e040-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e040-120">HTTP request</span></span>

```http
POST /policies
```
## <a name="request-headers"></a><span data-ttu-id="0e040-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0e040-121">Request headers</span></span>
| <span data-ttu-id="0e040-122">Name</span><span class="sxs-lookup"><span data-stu-id="0e040-122">Name</span></span>       | <span data-ttu-id="0e040-123">Typ</span><span class="sxs-lookup"><span data-stu-id="0e040-123">Type</span></span> | <span data-ttu-id="0e040-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e040-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0e040-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e040-125">Authorization</span></span>  | <span data-ttu-id="0e040-126">string</span><span class="sxs-lookup"><span data-stu-id="0e040-126">string</span></span>  | <span data-ttu-id="0e040-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0e040-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0e040-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0e040-129">Content-Type</span></span> | <span data-ttu-id="0e040-130">application/json</span><span class="sxs-lookup"><span data-stu-id="0e040-130">application/json</span></span>  | <span data-ttu-id="0e040-p105">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0e040-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e040-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0e040-133">Request body</span></span>
<span data-ttu-id="0e040-134">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Richtlinienobjekts](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="0e040-134">In the request body, provide a JSON representation of [policy](../resources/policy.md) object.</span></span>

<span data-ttu-id="0e040-135">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie eine Richtlinie erstellen.</span><span class="sxs-lookup"><span data-stu-id="0e040-135">The following table shows the properties that are required when you create a policy.</span></span>

| <span data-ttu-id="0e040-136">Parameter</span><span class="sxs-lookup"><span data-stu-id="0e040-136">Parameter</span></span>    | <span data-ttu-id="0e040-137">Typ</span><span class="sxs-lookup"><span data-stu-id="0e040-137">Type</span></span>   |<span data-ttu-id="0e040-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e040-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e040-139">definition</span><span class="sxs-lookup"><span data-stu-id="0e040-139">definition</span></span>|<span data-ttu-id="0e040-140">String</span><span class="sxs-lookup"><span data-stu-id="0e040-140">String</span></span>|<span data-ttu-id="0e040-141">Die Zeichenfolgenversion des [Richtlinienobjekts](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="0e040-141">The string version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="0e040-142">displayName</span><span class="sxs-lookup"><span data-stu-id="0e040-142">displayName</span></span>|<span data-ttu-id="0e040-143">String</span><span class="sxs-lookup"><span data-stu-id="0e040-143">String</span></span>|<span data-ttu-id="0e040-144">Ein benutzerdefinierter Name für die Richtlinie ein.</span><span class="sxs-lookup"><span data-stu-id="0e040-144">A custom name for the policy.</span></span>|
|<span data-ttu-id="0e040-145">type</span><span class="sxs-lookup"><span data-stu-id="0e040-145">type</span></span>|<span data-ttu-id="0e040-146">String</span><span class="sxs-lookup"><span data-stu-id="0e040-146">String</span></span>|<span data-ttu-id="0e040-147">Gibt den Typ der Richtlinie an.</span><span class="sxs-lookup"><span data-stu-id="0e040-147">Specifies the type of policy.</span></span> <span data-ttu-id="0e040-148">Derzeit muss "TokenLifetimePolicy"</span><span class="sxs-lookup"><span data-stu-id="0e040-148">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="0e040-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e040-149">Response</span></span>

<span data-ttu-id="0e040-150">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code und [Richtlinie](../resources/policy.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0e040-150">If successful, this method returns `201 Created` response code and [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="0e040-151">Wenn Sie nicht erfolgreich ist, ein `4xx` mit bestimmten Details entsprechende Fehlermeldung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0e040-151">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>  

## <a name="example"></a><span data-ttu-id="0e040-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0e040-152">Example</span></span>
<span data-ttu-id="0e040-153">Das folgende Beispiel erstellt eine neue token Lebensdauer Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="0e040-153">The following example creates a new token lifetime Policy.</span></span> <span data-ttu-id="0e040-154">Beachten Sie, dass der Definition Zeichenfolgenparameter doppelte Anführungszeichen Escapezeichen hat.</span><span class="sxs-lookup"><span data-stu-id="0e040-154">Notice the string definition parameter has escaped double quotes.</span></span>

##### <a name="request"></a><span data-ttu-id="0e040-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e040-155">Request</span></span>
<span data-ttu-id="0e040-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0e040-156">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/policies
Content-Type: application/json

{
  "displayName":"CustomTokenLifetimePolicy",
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "type":"TokenLifetimePolicy"
}
```

##### <a name="response"></a><span data-ttu-id="0e040-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e040-157">Response</span></span>
<span data-ttu-id="0e040-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0e040-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#policies/$entity",
  "id":"id-value",
  "alternativeIdentifier":null,
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "displayName":"name-value",
  "isOrganizationDefault":false,
  "keyCredentials",
  "type":"TokenLifetimePolicy"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
