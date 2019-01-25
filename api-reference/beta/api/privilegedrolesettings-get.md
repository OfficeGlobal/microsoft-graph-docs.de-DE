---
title: Abrufen von privilegedRoleSettings
description: Rufen Sie die rolleneinstellungen für die gegebene Rolle ab. Ein PrivilegedRoleSettings-Objekt wird zurückgegeben.
localization_priority: Normal
ms.openlocfilehash: 7ecebad77acf2e090263878aacc29f00a9215fc7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508104"
---
# <a name="get-privilegedrolesettings"></a><span data-ttu-id="9513e-104">Abrufen von privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="9513e-104">Get privilegedRoleSettings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9513e-105">Rufen Sie die rolleneinstellungen für die gegebene Rolle ab.</span><span class="sxs-lookup"><span data-stu-id="9513e-105">Retrieve the role settings for the given role.</span></span> <span data-ttu-id="9513e-106">Ein [PrivilegedRoleSettings](../resources/privilegedrolesettings.md) -Objekt wird zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9513e-106">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="9513e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9513e-107">Permissions</span></span>

<span data-ttu-id="9513e-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9513e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="9513e-110">Der Requestor muss eine der folgenden Rollen verfügen: _Berechtigten Rolle Administrators_, _Globaler Administrator_, _Sicherheitsadministrator_oder _Sicherheit Leser_.</span><span class="sxs-lookup"><span data-stu-id="9513e-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="9513e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9513e-111">Permission type</span></span>      | <span data-ttu-id="9513e-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9513e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9513e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9513e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9513e-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9513e-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9513e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9513e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9513e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9513e-116">Not supported.</span></span>    |
|<span data-ttu-id="9513e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9513e-117">Application</span></span> | <span data-ttu-id="9513e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9513e-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9513e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9513e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9513e-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9513e-120">Optional query parameters</span></span>
<span data-ttu-id="9513e-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9513e-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9513e-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9513e-122">Request headers</span></span>
| <span data-ttu-id="9513e-123">Name</span><span class="sxs-lookup"><span data-stu-id="9513e-123">Name</span></span>      |<span data-ttu-id="9513e-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9513e-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9513e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9513e-125">Authorization</span></span>  | <span data-ttu-id="9513e-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9513e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9513e-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9513e-128">Request body</span></span>
<span data-ttu-id="9513e-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9513e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9513e-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="9513e-130">Response</span></span>

<span data-ttu-id="9513e-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [PrivilegedRoleSettings](../resources/privilegedrolesettings.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="9513e-131">If successful, this method returns a `200 OK` response code and [privilegedRoleSettings](../resources/privilegedrolesettings.md) object in the response body.</span></span>

<span data-ttu-id="9513e-132">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="9513e-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="9513e-133">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="9513e-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="9513e-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9513e-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9513e-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9513e-135">Request</span></span>
<span data-ttu-id="9513e-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9513e-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesettings"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
```
##### <a name="response"></a><span data-ttu-id="9513e-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="9513e-137">Response</span></span>
<span data-ttu-id="9513e-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9513e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrolesettings-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
