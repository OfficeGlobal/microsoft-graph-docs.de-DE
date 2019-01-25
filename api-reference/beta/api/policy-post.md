---
title: Richtlinie erstellen
description: Erstellen Sie ein neues Gruppenrichtlinienobjekt durch Anzeigename, Richtlinientyp und Beschreibung der Richtlinie angeben.
localization_priority: Normal
ms.openlocfilehash: 30a311b45f9705a07b62541a4f3a110daade09fa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527696"
---
# <a name="create-policy"></a><span data-ttu-id="ce6e3-103">Richtlinie erstellen</span><span class="sxs-lookup"><span data-stu-id="ce6e3-103">Create Policy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce6e3-104">Erstellen [Sie ein neues Gruppenrichtlinienobjekt](../resources/policy.md) durch Anzeigename, Richtlinientyp und Beschreibung der Richtlinie angeben.</span><span class="sxs-lookup"><span data-stu-id="ce6e3-104">Create a new [policy](../resources/policy.md) object by specifying display name, policy type, and policy description.</span></span>

><span data-ttu-id="ce6e3-105">Hinweis: Die Richtliniendetails werden vor dem Speichern überprüft.</span><span class="sxs-lookup"><span data-stu-id="ce6e3-105">Note: The policy details will be validated before being stored.</span></span> <span data-ttu-id="ce6e3-106">Wenn sie die Überprüfung nicht bestanden hat, wird ein 400 Ungültige Anforderung zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="ce6e3-106">If it does not pass validation, a 400 Bad Request will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce6e3-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ce6e3-107">Permissions</span></span>
<span data-ttu-id="ce6e3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce6e3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce6e3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ce6e3-110">Permission type</span></span>      | <span data-ttu-id="ce6e3-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ce6e3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce6e3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ce6e3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ce6e3-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ce6e3-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ce6e3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ce6e3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce6e3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ce6e3-115">Not supported.</span></span>    |
|<span data-ttu-id="ce6e3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ce6e3-116">Application</span></span> | <span data-ttu-id="ce6e3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ce6e3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce6e3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce6e3-118">HTTP request</span></span>

```http
POST /policies
```
## <a name="request-headers"></a><span data-ttu-id="ce6e3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ce6e3-119">Request headers</span></span>
| <span data-ttu-id="ce6e3-120">Name</span><span class="sxs-lookup"><span data-stu-id="ce6e3-120">Name</span></span>       | <span data-ttu-id="ce6e3-121">Typ</span><span class="sxs-lookup"><span data-stu-id="ce6e3-121">Type</span></span> | <span data-ttu-id="ce6e3-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ce6e3-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ce6e3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce6e3-123">Authorization</span></span>  | <span data-ttu-id="ce6e3-124">string</span><span class="sxs-lookup"><span data-stu-id="ce6e3-124">string</span></span>  | <span data-ttu-id="ce6e3-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ce6e3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ce6e3-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ce6e3-127">Content-Type</span></span> | <span data-ttu-id="ce6e3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ce6e3-128">application/json</span></span>  | <span data-ttu-id="ce6e3-p104">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ce6e3-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce6e3-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ce6e3-131">Request body</span></span>
<span data-ttu-id="ce6e3-132">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Richtlinienobjekts](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="ce6e3-132">In the request body, provide a JSON representation of [policy](../resources/policy.md) object.</span></span>

<span data-ttu-id="ce6e3-133">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie eine Richtlinie erstellen.</span><span class="sxs-lookup"><span data-stu-id="ce6e3-133">The following table shows the properties that are required when you create a policy.</span></span>

| <span data-ttu-id="ce6e3-134">Parameter</span><span class="sxs-lookup"><span data-stu-id="ce6e3-134">Parameter</span></span>    | <span data-ttu-id="ce6e3-135">Typ</span><span class="sxs-lookup"><span data-stu-id="ce6e3-135">Type</span></span>   |<span data-ttu-id="ce6e3-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ce6e3-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce6e3-137">definition</span><span class="sxs-lookup"><span data-stu-id="ce6e3-137">definition</span></span>|<span data-ttu-id="ce6e3-138">String</span><span class="sxs-lookup"><span data-stu-id="ce6e3-138">String</span></span>|<span data-ttu-id="ce6e3-139">Die Zeichenfolgenversion des [Richtlinienobjekts](../resources/policy.md) .</span><span class="sxs-lookup"><span data-stu-id="ce6e3-139">The string version of the [policy](../resources/policy.md) object.</span></span>|
|<span data-ttu-id="ce6e3-140">displayName</span><span class="sxs-lookup"><span data-stu-id="ce6e3-140">displayName</span></span>|<span data-ttu-id="ce6e3-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce6e3-141">String</span></span>|<span data-ttu-id="ce6e3-142">Ein benutzerdefinierter Name für die Richtlinie ein.</span><span class="sxs-lookup"><span data-stu-id="ce6e3-142">A custom name for the policy.</span></span>|
|<span data-ttu-id="ce6e3-143">type</span><span class="sxs-lookup"><span data-stu-id="ce6e3-143">type</span></span>|<span data-ttu-id="ce6e3-144">String</span><span class="sxs-lookup"><span data-stu-id="ce6e3-144">String</span></span>|<span data-ttu-id="ce6e3-145">Gibt den Typ der Richtlinie an.</span><span class="sxs-lookup"><span data-stu-id="ce6e3-145">Specifies the type of policy.</span></span> <span data-ttu-id="ce6e3-146">Derzeit muss "TokenLifetimePolicy"</span><span class="sxs-lookup"><span data-stu-id="ce6e3-146">Currently must be "TokenLifetimePolicy"</span></span>|

## <a name="response"></a><span data-ttu-id="ce6e3-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce6e3-147">Response</span></span>

<span data-ttu-id="ce6e3-148">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code und [Richtlinie](../resources/policy.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ce6e3-148">If successful, this method returns `201 Created` response code and [policy](../resources/policy.md) object in the response body.</span></span> <span data-ttu-id="ce6e3-149">Wenn Sie nicht erfolgreich ist, ein `4xx` mit bestimmten Details entsprechende Fehlermeldung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ce6e3-149">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>  

## <a name="example"></a><span data-ttu-id="ce6e3-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ce6e3-150">Example</span></span>
<span data-ttu-id="ce6e3-151">Das folgende Beispiel erstellt eine neue token Lebensdauer Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="ce6e3-151">The following example creates a new token lifetime Policy.</span></span> <span data-ttu-id="ce6e3-152">Beachten Sie, dass der Definition Zeichenfolgenparameter doppelte Anführungszeichen Escapezeichen hat.</span><span class="sxs-lookup"><span data-stu-id="ce6e3-152">Notice the string definition parameter has escaped double quotes.</span></span>

##### <a name="request"></a><span data-ttu-id="ce6e3-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce6e3-153">Request</span></span>
<span data-ttu-id="ce6e3-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ce6e3-154">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/policies
Content-Type: application/json

{
  "displayName":"CustomTokenLifetimePolicy",
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\"}}"],
  "type":"TokenLifetimePolicy"
}
```

##### <a name="response"></a><span data-ttu-id="ce6e3-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce6e3-155">Response</span></span>
<span data-ttu-id="ce6e3-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ce6e3-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
