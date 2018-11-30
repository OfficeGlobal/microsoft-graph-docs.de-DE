---
title: Liste Anwendungen und Dienstprinzipale mit bestimmten Richtlinie zugewiesen.
description: Abrufen der Anwendung und Service principal-Objekte mit der angegebenen Richtlinie zugewiesen.
ms.openlocfilehash: 3f281d7c60a506676a78637ad71f1ce26de35e34
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064579"
---
# <a name="list-applications-and-service-principals-with-specific-policy-assigned"></a><span data-ttu-id="99bfe-103">Liste Anwendungen und Dienstprinzipale mit bestimmten Richtlinie zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="99bfe-103">List Applications and Service Principals with specific Policy assigned</span></span>

> <span data-ttu-id="99bfe-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="99bfe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99bfe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="99bfe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99bfe-106">Rufen Sie die Objekte [Application](../resources/application.md) und [Service principal](../resources/serviceprincipal.md) mit der angegebenen Richtlinie zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="99bfe-106">Retrieve the [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects with the specified policy assigned.</span></span>

## <a name="permissions"></a><span data-ttu-id="99bfe-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="99bfe-107">Permissions</span></span>
<span data-ttu-id="99bfe-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99bfe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99bfe-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="99bfe-110">Permission type</span></span>      | <span data-ttu-id="99bfe-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="99bfe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99bfe-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="99bfe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="99bfe-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="99bfe-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="99bfe-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="99bfe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99bfe-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="99bfe-115">Not supported.</span></span>    |
|<span data-ttu-id="99bfe-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="99bfe-116">Application</span></span> | <span data-ttu-id="99bfe-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="99bfe-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="99bfe-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="99bfe-118">HTTP request</span></span>
```http
GET /policies/{id}/appliesTo
```

## <a name="request-headers"></a><span data-ttu-id="99bfe-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="99bfe-119">Request headers</span></span>
| <span data-ttu-id="99bfe-120">Name</span><span class="sxs-lookup"><span data-stu-id="99bfe-120">Name</span></span>       | <span data-ttu-id="99bfe-121">Typ</span><span class="sxs-lookup"><span data-stu-id="99bfe-121">Type</span></span> | <span data-ttu-id="99bfe-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="99bfe-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="99bfe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="99bfe-123">Authorization</span></span>  | <span data-ttu-id="99bfe-124">string</span><span class="sxs-lookup"><span data-stu-id="99bfe-124">string</span></span>  | <span data-ttu-id="99bfe-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="99bfe-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99bfe-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="99bfe-127">Request body</span></span>
<span data-ttu-id="99bfe-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="99bfe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99bfe-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="99bfe-129">Response</span></span>

<span data-ttu-id="99bfe-130">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` [Code und [Dienstprinzipal](../resources/serviceprincipal.md) und](../resources/application.md) Antwortobjekte im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="99bfe-130">If successful, this method returns `200 OK` response code and [application](../resources/application.md) and [service principal](../resources/serviceprincipal.md) objects in the response body.</span></span> <span data-ttu-id="99bfe-131">Wenn Sie nicht erfolgreich ist, ein `4xx` mit bestimmten Details entsprechende Fehlermeldung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="99bfe-131">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="99bfe-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="99bfe-132">Example</span></span>
<span data-ttu-id="99bfe-133">Im folgende Beispiel werden die dienstanwendungen und Dienstprinzipale mit einer bestimmten Richtlinie zugewiesen abgerufen.</span><span class="sxs-lookup"><span data-stu-id="99bfe-133">The following example retrieves the applications and service principals with a specific policy assigned.</span></span>

##### <a name="request"></a><span data-ttu-id="99bfe-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="99bfe-134">Request</span></span>
<span data-ttu-id="99bfe-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="99bfe-135">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/policies/{id}/appliesTo
```

##### <a name="response"></a><span data-ttu-id="99bfe-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="99bfe-136">Response</span></span>
<span data-ttu-id="99bfe-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="99bfe-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
