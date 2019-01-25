---
title: Liste arbeiten
description: Berechnete Insight für die Liste der Benutzer, denen ein Benutzer mit gearbeitet hat.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ca5fdd4602d109d98002c0ef54fde5ad341e1903
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521621"
---
# <a name="list-workingwith"></a><span data-ttu-id="6e4c8-103">Liste arbeiten</span><span class="sxs-lookup"><span data-stu-id="6e4c8-103">List workingWith</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e4c8-104">Berechnete Insight für die Liste der Benutzer, denen ein Benutzer mit gearbeitet hat.</span><span class="sxs-lookup"><span data-stu-id="6e4c8-104">Calculated insight for the list of users that a user has been working with.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e4c8-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6e4c8-105">Permissions</span></span>
<span data-ttu-id="6e4c8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e4c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e4c8-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6e4c8-108">Permission type</span></span>      | <span data-ttu-id="6e4c8-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6e4c8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e4c8-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6e4c8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6e4c8-111">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e4c8-111">User.Read.All</span></span>    |
|<span data-ttu-id="6e4c8-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6e4c8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e4c8-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6e4c8-113">Not supported.</span></span>    |
|<span data-ttu-id="6e4c8-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6e4c8-114">Application</span></span> | <span data-ttu-id="6e4c8-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6e4c8-115">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e4c8-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e4c8-116">HTTP request</span></span>
```http
GET /me/workingWith
GET /users/{id | userPrincipalName}/workingWith
GET /drive/root/createdByUser/workingWith
GET /drive/root/lastModifiedByUser/workingWith
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6e4c8-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6e4c8-117">Optional query parameters</span></span>
<span data-ttu-id="6e4c8-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6e4c8-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e4c8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6e4c8-119">Request headers</span></span>
| <span data-ttu-id="6e4c8-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6e4c8-120">Header</span></span>         | <span data-ttu-id="6e4c8-121">Wert</span><span class="sxs-lookup"><span data-stu-id="6e4c8-121">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="6e4c8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e4c8-122">Authorization</span></span>  | <span data-ttu-id="6e4c8-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6e4c8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6e4c8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6e4c8-125">Content-Type</span></span>   | <span data-ttu-id="6e4c8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e4c8-126">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="6e4c8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6e4c8-127">Request body</span></span>
<span data-ttu-id="6e4c8-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6e4c8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e4c8-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="6e4c8-129">Response</span></span>

<span data-ttu-id="6e4c8-130">Wenn erfolgreich, gibt diese Methode einen 200 OK-Antwortcode und eine Auflistung von [Benutzerobjekten](../resources/user.md) in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6e4c8-130">If successful, this method returns a 200 OK response code and collection of [User](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e4c8-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6e4c8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6e4c8-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6e4c8-132">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/workingWith
```
##### <a name="response"></a><span data-ttu-id="6e4c8-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="6e4c8-133">Response</span></span>
<span data-ttu-id="6e4c8-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6e4c8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "id": "id-value",
  "preferredName": "preferredName-value",
  "Email": "Email-value",
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-workingwith.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
