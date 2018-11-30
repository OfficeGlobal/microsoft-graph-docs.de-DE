---
title: Abrufen von privilegedRoleSettings
description: Rufen Sie die rolleneinstellungen für die gegebene Rolle ab. Ein PrivilegedRoleSettings-Objekt wird zurückgegeben.
ms.openlocfilehash: c064e2eb11a4e91247894338c43c7c6dd9f9dcc3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059429"
---
# <a name="get-privilegedrolesettings"></a><span data-ttu-id="7724a-104">Abrufen von privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="7724a-104">Get privilegedRoleSettings</span></span>

> <span data-ttu-id="7724a-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7724a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7724a-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7724a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7724a-107">Rufen Sie die rolleneinstellungen für die gegebene Rolle ab.</span><span class="sxs-lookup"><span data-stu-id="7724a-107">Retrieve the role settings for the given role.</span></span> <span data-ttu-id="7724a-108">Ein [PrivilegedRoleSettings](../resources/privilegedrolesettings.md) -Objekt wird zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7724a-108">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="7724a-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7724a-109">Permissions</span></span>

<span data-ttu-id="7724a-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7724a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="7724a-112">Der Requestor muss eine der folgenden Rollen verfügen: _Berechtigten Rolle Administrators_, _Globaler Administrator_, _Sicherheitsadministrator_oder _Sicherheit Leser_.</span><span class="sxs-lookup"><span data-stu-id="7724a-112">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="7724a-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7724a-113">Permission type</span></span>      | <span data-ttu-id="7724a-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7724a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7724a-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7724a-115">Delegated (work or school account)</span></span> | <span data-ttu-id="7724a-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7724a-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7724a-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7724a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7724a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7724a-118">Not supported.</span></span>    |
|<span data-ttu-id="7724a-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7724a-119">Application</span></span> | <span data-ttu-id="7724a-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7724a-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7724a-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7724a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7724a-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7724a-122">Optional query parameters</span></span>
<span data-ttu-id="7724a-123">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7724a-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7724a-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7724a-124">Request headers</span></span>
| <span data-ttu-id="7724a-125">Name</span><span class="sxs-lookup"><span data-stu-id="7724a-125">Name</span></span>      |<span data-ttu-id="7724a-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7724a-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7724a-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="7724a-127">Authorization</span></span>  | <span data-ttu-id="7724a-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7724a-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7724a-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7724a-130">Request body</span></span>
<span data-ttu-id="7724a-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7724a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7724a-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="7724a-132">Response</span></span>

<span data-ttu-id="7724a-133">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [PrivilegedRoleSettings](../resources/privilegedrolesettings.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="7724a-133">If successful, this method returns a `200 OK` response code and [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.</span></span>

<span data-ttu-id="7724a-134">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="7724a-134">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="7724a-135">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="7724a-135">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="7724a-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7724a-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7724a-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7724a-137">Request</span></span>
<span data-ttu-id="7724a-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7724a-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesettings"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
```
##### <a name="response"></a><span data-ttu-id="7724a-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="7724a-139">Response</span></span>
<span data-ttu-id="7724a-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7724a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 228

{
  "minElevationDuration": "2016-10-19T10:37:00Z",
  "maxElavationDuration": "2016-10-19T10:37:00Z",
  "elevationDuration": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->