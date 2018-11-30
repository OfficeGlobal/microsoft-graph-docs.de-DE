---
title: Zugewiesene Anwendung oder Dienstprinzipal Listenrichtlinien
description: Abrufen der Richtlinienobjekte, die eine Anwendung oder ein Service principal zugewiesen.
ms.openlocfilehash: cfdcf3d8e6709080f4c8f7bfc3e2dbc256789f6f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060679"
---
# <a name="list-policies-assigned-to-application-or-service-principal"></a><span data-ttu-id="da6e1-103">Zugewiesene Anwendung oder Dienstprinzipal Listenrichtlinien</span><span class="sxs-lookup"><span data-stu-id="da6e1-103">List Policies assigned to Application or Service Principal</span></span>

> <span data-ttu-id="da6e1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="da6e1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da6e1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="da6e1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="da6e1-106">Abrufen der [Richtlinie](../resources/policy.md) -Objekte, die eine Anwendung oder ein Service principal zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="da6e1-106">Retrieve the [policy](../resources/policy.md) objects assigned to an application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="da6e1-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="da6e1-107">Permissions</span></span>
<span data-ttu-id="da6e1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da6e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da6e1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="da6e1-110">Permission type</span></span>      | <span data-ttu-id="da6e1-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="da6e1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da6e1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="da6e1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="da6e1-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="da6e1-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="da6e1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="da6e1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da6e1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="da6e1-115">Not supported.</span></span>    |
|<span data-ttu-id="da6e1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="da6e1-116">Application</span></span> | <span data-ttu-id="da6e1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="da6e1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="da6e1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="da6e1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/policies
```

> <span data-ttu-id="da6e1-119">Hinweis: "Id" in der Anforderung ist die Eigenschaft "Id" der Anwendung oder Dienstprinzipal, nicht die Eigenschaft "Appid".</span><span class="sxs-lookup"><span data-stu-id="da6e1-119">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da6e1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="da6e1-120">Request headers</span></span>
| <span data-ttu-id="da6e1-121">Name</span><span class="sxs-lookup"><span data-stu-id="da6e1-121">Name</span></span>       | <span data-ttu-id="da6e1-122">Typ</span><span class="sxs-lookup"><span data-stu-id="da6e1-122">Type</span></span> | <span data-ttu-id="da6e1-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da6e1-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="da6e1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="da6e1-124">Authorization</span></span>  | <span data-ttu-id="da6e1-125">string</span><span class="sxs-lookup"><span data-stu-id="da6e1-125">string</span></span>  | <span data-ttu-id="da6e1-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="da6e1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da6e1-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="da6e1-128">Request body</span></span>
<span data-ttu-id="da6e1-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="da6e1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da6e1-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="da6e1-130">Response</span></span>

<span data-ttu-id="da6e1-131">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortobjekte Code und [Richtlinie](../resources/policy.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="da6e1-131">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="da6e1-132">Wenn Sie nicht erfolgreich ist, ein `4xx` mit bestimmten Details entsprechende Fehlermeldung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="da6e1-132">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="da6e1-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="da6e1-133">Example</span></span>
<span data-ttu-id="da6e1-134">Im folgende Beispiel werden die Richtlinien zugewiesen an eine Anwendung abgerufen.</span><span class="sxs-lookup"><span data-stu-id="da6e1-134">The following example retrieves the policies assigned to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="da6e1-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="da6e1-135">Request</span></span>
<span data-ttu-id="da6e1-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="da6e1-136">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/applications/{id}/policies
```

##### <a name="response"></a><span data-ttu-id="da6e1-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="da6e1-137">Response</span></span>
<span data-ttu-id="da6e1-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="da6e1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Cache-Control: private
Content-Type: application/json

{
    "value":[
        {
            "@odata.type":"#microsoft.graph.policy",
            "id":"id-value",
            "alternativeIdentifier":null,
            "definition":["policy-definition"],
            "displayName":"name-value",
            "isOrganizationDefault":boolean-value,
            "keyCredentials":[key-credentials],
            "type":"type-value"
        }
    ]
}
```
