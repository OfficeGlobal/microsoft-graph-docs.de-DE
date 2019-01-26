---
title: Zugewiesene Anwendung oder Dienstprinzipal Listenrichtlinien
description: Abrufen der Richtlinienobjekte, die eine Anwendung oder ein Service principal zugewiesen.
localization_priority: Normal
ms.openlocfilehash: 417d59228aadd3c6a54c4634416fd577fce11f18
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575961"
---
# <a name="list-policies-assigned-to-application-or-service-principal"></a><span data-ttu-id="1ad43-103">Zugewiesene Anwendung oder Dienstprinzipal Listenrichtlinien</span><span class="sxs-lookup"><span data-stu-id="1ad43-103">List Policies assigned to Application or Service Principal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ad43-104">Abrufen der [Richtlinie](../resources/policy.md) -Objekte, die eine Anwendung oder ein Service principal zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="1ad43-104">Retrieve the [policy](../resources/policy.md) objects assigned to an application or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ad43-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1ad43-105">Permissions</span></span>
<span data-ttu-id="1ad43-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ad43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ad43-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1ad43-108">Permission type</span></span>      | <span data-ttu-id="1ad43-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1ad43-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ad43-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1ad43-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1ad43-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1ad43-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1ad43-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1ad43-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ad43-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1ad43-113">Not supported.</span></span>    |
|<span data-ttu-id="1ad43-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1ad43-114">Application</span></span> | <span data-ttu-id="1ad43-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1ad43-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ad43-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ad43-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/policies
```

> <span data-ttu-id="1ad43-117">Hinweis: "Id" in der Anforderung ist die Eigenschaft "Id" der Anwendung oder Dienstprinzipal, nicht die Eigenschaft "Appid".</span><span class="sxs-lookup"><span data-stu-id="1ad43-117">Note: The "id" in the request is the "id" property of the application or service principal, not the "appid" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ad43-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1ad43-118">Request headers</span></span>
| <span data-ttu-id="1ad43-119">Name</span><span class="sxs-lookup"><span data-stu-id="1ad43-119">Name</span></span>       | <span data-ttu-id="1ad43-120">Typ</span><span class="sxs-lookup"><span data-stu-id="1ad43-120">Type</span></span> | <span data-ttu-id="1ad43-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1ad43-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1ad43-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ad43-122">Authorization</span></span>  | <span data-ttu-id="1ad43-123">string</span><span class="sxs-lookup"><span data-stu-id="1ad43-123">string</span></span>  | <span data-ttu-id="1ad43-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1ad43-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ad43-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1ad43-126">Request body</span></span>
<span data-ttu-id="1ad43-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1ad43-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ad43-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ad43-128">Response</span></span>

<span data-ttu-id="1ad43-129">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortobjekte Code und [Richtlinie](../resources/policy.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="1ad43-129">If successful, this method returns `200 OK` response code and [policy](../resources/policy.md) objects in the response body.</span></span> <span data-ttu-id="1ad43-130">Wenn Sie nicht erfolgreich ist, ein `4xx` mit bestimmten Details entsprechende Fehlermeldung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1ad43-130">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="1ad43-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1ad43-131">Example</span></span>
<span data-ttu-id="1ad43-132">Im folgende Beispiel werden die Richtlinien zugewiesen an eine Anwendung abgerufen.</span><span class="sxs-lookup"><span data-stu-id="1ad43-132">The following example retrieves the policies assigned to an application.</span></span>

##### <a name="request"></a><span data-ttu-id="1ad43-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ad43-133">Request</span></span>
<span data-ttu-id="1ad43-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1ad43-134">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/applications/{id}/policies
```

##### <a name="response"></a><span data-ttu-id="1ad43-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ad43-135">Response</span></span>
<span data-ttu-id="1ad43-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1ad43-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
            "isOrganizationDefault": true | false,
            "keyCredentials":[key-credentials],
            "type":"type-value"
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-list-assigned.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
