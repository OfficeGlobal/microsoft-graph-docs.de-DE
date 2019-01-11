---
title: Liste arbeiten
description: Berechnete Insight für die Liste der Benutzer, denen ein Benutzer mit gearbeitet hat.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: df7f84bf42887d9052cb9d81042b5735af7bd2b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870336"
---
# <a name="list-workingwith"></a><span data-ttu-id="91a80-103">Liste arbeiten</span><span class="sxs-lookup"><span data-stu-id="91a80-103">List workingWith</span></span>

> <span data-ttu-id="91a80-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="91a80-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91a80-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="91a80-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91a80-106">Berechnete Insight für die Liste der Benutzer, denen ein Benutzer mit gearbeitet hat.</span><span class="sxs-lookup"><span data-stu-id="91a80-106">Calculated insight for the list of users that a user has been working with.</span></span>

## <a name="permissions"></a><span data-ttu-id="91a80-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="91a80-107">Permissions</span></span>
<span data-ttu-id="91a80-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91a80-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91a80-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="91a80-110">Permission type</span></span>      | <span data-ttu-id="91a80-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="91a80-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91a80-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="91a80-112">Delegated (work or school account)</span></span> | <span data-ttu-id="91a80-113">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="91a80-113">User.Read.All</span></span>    |
|<span data-ttu-id="91a80-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="91a80-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91a80-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="91a80-115">Not supported.</span></span>    |
|<span data-ttu-id="91a80-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="91a80-116">Application</span></span> | <span data-ttu-id="91a80-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="91a80-117">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="91a80-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="91a80-118">HTTP request</span></span>
```http
GET /me/workingWith
GET /users/{id | userPrincipalName}/workingWith
GET /drive/root/createdByUser/workingWith
GET /drive/root/lastModifiedByUser/workingWith
```
## <a name="optional-query-parameters"></a><span data-ttu-id="91a80-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="91a80-119">Optional query parameters</span></span>
<span data-ttu-id="91a80-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="91a80-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="91a80-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="91a80-121">Request headers</span></span>
| <span data-ttu-id="91a80-122">Header</span><span class="sxs-lookup"><span data-stu-id="91a80-122">Header</span></span>         | <span data-ttu-id="91a80-123">Wert</span><span class="sxs-lookup"><span data-stu-id="91a80-123">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="91a80-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="91a80-124">Authorization</span></span>  | <span data-ttu-id="91a80-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="91a80-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="91a80-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="91a80-127">Content-Type</span></span>   | <span data-ttu-id="91a80-128">application/json</span><span class="sxs-lookup"><span data-stu-id="91a80-128">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="91a80-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="91a80-129">Request body</span></span>
<span data-ttu-id="91a80-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="91a80-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91a80-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="91a80-131">Response</span></span>

<span data-ttu-id="91a80-132">Wenn erfolgreich, gibt diese Methode einen 200 OK-Antwortcode und eine Auflistung von [Benutzerobjekten](../resources/user.md) in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="91a80-132">If successful, this method returns a 200 OK response code and collection of [User](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91a80-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="91a80-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91a80-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="91a80-134">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/workingWith
```
##### <a name="response"></a><span data-ttu-id="91a80-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="91a80-135">Response</span></span>
<span data-ttu-id="91a80-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="91a80-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
