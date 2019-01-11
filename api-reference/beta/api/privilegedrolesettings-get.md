---
title: Abrufen von privilegedRoleSettings
description: Rufen Sie die rolleneinstellungen für die gegebene Rolle ab. Ein PrivilegedRoleSettings-Objekt wird zurückgegeben.
localization_priority: Normal
ms.openlocfilehash: a80c4027ace009292e7a57b8104e94e114175f1d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879814"
---
# <a name="get-privilegedrolesettings"></a><span data-ttu-id="41530-104">Abrufen von privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="41530-104">Get privilegedRoleSettings</span></span>

> <span data-ttu-id="41530-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="41530-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41530-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="41530-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="41530-107">Rufen Sie die rolleneinstellungen für die gegebene Rolle ab.</span><span class="sxs-lookup"><span data-stu-id="41530-107">Retrieve the role settings for the given role.</span></span> <span data-ttu-id="41530-108">Ein [PrivilegedRoleSettings](../resources/privilegedrolesettings.md) -Objekt wird zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="41530-108">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="41530-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="41530-109">Permissions</span></span>

<span data-ttu-id="41530-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41530-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="41530-112">Der Requestor muss eine der folgenden Rollen verfügen: _Berechtigten Rolle Administrators_, _Globaler Administrator_, _Sicherheitsadministrator_oder _Sicherheit Leser_.</span><span class="sxs-lookup"><span data-stu-id="41530-112">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="41530-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="41530-113">Permission type</span></span>      | <span data-ttu-id="41530-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="41530-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41530-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="41530-115">Delegated (work or school account)</span></span> | <span data-ttu-id="41530-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="41530-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="41530-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="41530-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41530-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="41530-118">Not supported.</span></span>    |
|<span data-ttu-id="41530-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="41530-119">Application</span></span> | <span data-ttu-id="41530-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="41530-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="41530-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="41530-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="41530-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="41530-122">Optional query parameters</span></span>
<span data-ttu-id="41530-123">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="41530-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41530-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="41530-124">Request headers</span></span>
| <span data-ttu-id="41530-125">Name</span><span class="sxs-lookup"><span data-stu-id="41530-125">Name</span></span>      |<span data-ttu-id="41530-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41530-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="41530-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="41530-127">Authorization</span></span>  | <span data-ttu-id="41530-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="41530-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41530-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="41530-130">Request body</span></span>
<span data-ttu-id="41530-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="41530-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41530-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="41530-132">Response</span></span>

<span data-ttu-id="41530-133">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [PrivilegedRoleSettings](../resources/privilegedrolesettings.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="41530-133">If successful, this method returns a `200 OK` response code and [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.</span></span>

<span data-ttu-id="41530-134">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="41530-134">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="41530-135">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="41530-135">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="41530-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="41530-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="41530-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="41530-137">Request</span></span>
<span data-ttu-id="41530-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="41530-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesettings"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
```
##### <a name="response"></a><span data-ttu-id="41530-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="41530-139">Response</span></span>
<span data-ttu-id="41530-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="41530-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
