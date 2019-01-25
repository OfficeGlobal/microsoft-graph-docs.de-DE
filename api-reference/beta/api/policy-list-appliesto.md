---
title: Liste Anwendungen und Dienstprinzipale mit bestimmten Richtlinie zugewiesen.
description: Abrufen der Anwendung und Service principal-Objekte mit der angegebenen Richtlinie zugewiesen.
localization_priority: Normal
ms.openlocfilehash: d7449428216a2e68d9ab8bb8399ca0e8dc4b72fd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510477"
---
# <a name="list-applications-and-service-principals-with-specific-policy-assigned"></a><span data-ttu-id="6f8f1-103">Liste Anwendungen und Dienstprinzipale mit bestimmten Richtlinie zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="6f8f1-103">List Applications and Service Principals with specific Policy assigned</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f8f1-104">Rufen Sie die Objekte [Application](../resources/application.md) und [Service principal](../resources/serviceprincipal.md) mit der angegebenen Richtlinie zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="6f8f1-104">Retrieve the [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects with the specified policy assigned.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f8f1-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6f8f1-105">Permissions</span></span>
<span data-ttu-id="6f8f1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f8f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f8f1-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6f8f1-108">Permission type</span></span>      | <span data-ttu-id="6f8f1-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6f8f1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f8f1-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6f8f1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6f8f1-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6f8f1-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6f8f1-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6f8f1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f8f1-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f8f1-113">Not supported.</span></span>    |
|<span data-ttu-id="6f8f1-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6f8f1-114">Application</span></span> | <span data-ttu-id="6f8f1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6f8f1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f8f1-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f8f1-116">HTTP request</span></span>
```http
GET /policies/{id}/appliesTo
```

## <a name="request-headers"></a><span data-ttu-id="6f8f1-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6f8f1-117">Request headers</span></span>
| <span data-ttu-id="6f8f1-118">Name</span><span class="sxs-lookup"><span data-stu-id="6f8f1-118">Name</span></span>       | <span data-ttu-id="6f8f1-119">Typ</span><span class="sxs-lookup"><span data-stu-id="6f8f1-119">Type</span></span> | <span data-ttu-id="6f8f1-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6f8f1-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6f8f1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f8f1-121">Authorization</span></span>  | <span data-ttu-id="6f8f1-122">string</span><span class="sxs-lookup"><span data-stu-id="6f8f1-122">string</span></span>  | <span data-ttu-id="6f8f1-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6f8f1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f8f1-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6f8f1-125">Request body</span></span>
<span data-ttu-id="6f8f1-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6f8f1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f8f1-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f8f1-127">Response</span></span>

<span data-ttu-id="6f8f1-128">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` [Code und [Dienstprinzipal](../resources/serviceprincipal.md) und](../resources/application.md) Antwortobjekte im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6f8f1-128">If successful, this method returns `200 OK` response code and [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects in the response body.</span></span> <span data-ttu-id="6f8f1-129">Wenn Sie nicht erfolgreich ist, ein `4xx` mit bestimmten Details entsprechende Fehlermeldung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f8f1-129">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="6f8f1-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6f8f1-130">Example</span></span>
<span data-ttu-id="6f8f1-131">Im folgende Beispiel werden die dienstanwendungen und Dienstprinzipale mit einer bestimmten Richtlinie zugewiesen abgerufen.</span><span class="sxs-lookup"><span data-stu-id="6f8f1-131">The following example retrieves the applications and service principals with a specific policy assigned.</span></span>

##### <a name="request"></a><span data-ttu-id="6f8f1-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6f8f1-132">Request</span></span>
<span data-ttu-id="6f8f1-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6f8f1-133">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}/appliesTo
```

##### <a name="response"></a><span data-ttu-id="6f8f1-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6f8f1-134">Response</span></span>
<span data-ttu-id="6f8f1-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6f8f1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value":[
        {
            "@odata.type"="#microsoft.graph.application",
            "appId":"appId-value",
            "displayName":"displayName-value",
            "errorUrl":"errorUrl-value",
            "groupMembershipClaims":"groupMembershipClaims-value",
            "homepage":"homepage-value",
            "id":"id-value",
            "keyCredentials":[key-credentials],
            "logoutUrl":"logoutUrl-value",
            "replyUrls":["replyUrls-value"]
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-list-appliesto.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
