---
title: Liste privilegedRoleAssignments
description: Abrufen einer Liste von PrivilegedRoleAssignment-Objekten, die alle rollenzuweisungen für die Organisation entsprechen.
localization_priority: Normal
ms.openlocfilehash: c576e0d9c0a278e02159e02cea94ddd927561e08
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516588"
---
# <a name="list-privilegedroleassignments"></a><span data-ttu-id="31ee0-103">Liste privilegedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="31ee0-103">List privilegedRoleAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31ee0-104">Abrufen einer Liste von [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) -Objekten, die alle rollenzuweisungen für die Organisation entsprechen.</span><span class="sxs-lookup"><span data-stu-id="31ee0-104">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects, which correspond to all role assignments for the organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="31ee0-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="31ee0-105">Permissions</span></span>
<span data-ttu-id="31ee0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31ee0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="31ee0-108">Der Requestor muss eine der folgenden Rollen verfügen: _Berechtigten Rolle Administrators_, _Globaler Administrator_, _Sicherheitsadministrator_oder _Sicherheit Leser_.</span><span class="sxs-lookup"><span data-stu-id="31ee0-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="31ee0-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="31ee0-109">Permission type</span></span>      | <span data-ttu-id="31ee0-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="31ee0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31ee0-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="31ee0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="31ee0-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="31ee0-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="31ee0-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="31ee0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31ee0-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="31ee0-114">Not supported.</span></span>    |
|<span data-ttu-id="31ee0-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="31ee0-115">Application</span></span> | <span data-ttu-id="31ee0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="31ee0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="31ee0-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="31ee0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="31ee0-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="31ee0-118">Optional query parameters</span></span>
<span data-ttu-id="31ee0-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="31ee0-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31ee0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="31ee0-120">Request headers</span></span>
| <span data-ttu-id="31ee0-121">Name</span><span class="sxs-lookup"><span data-stu-id="31ee0-121">Name</span></span>      |<span data-ttu-id="31ee0-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="31ee0-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="31ee0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="31ee0-123">Authorization</span></span>  | <span data-ttu-id="31ee0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="31ee0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31ee0-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="31ee0-126">Request body</span></span>
<span data-ttu-id="31ee0-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="31ee0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31ee0-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="31ee0-128">Response</span></span>

<span data-ttu-id="31ee0-129">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="31ee0-129">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="31ee0-130">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="31ee0-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="31ee0-131">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="31ee0-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="examples"></a><span data-ttu-id="31ee0-132">Beispiele</span><span class="sxs-lookup"><span data-stu-id="31ee0-132">Examples</span></span>
### <a name="get-all-role-assignments"></a><span data-ttu-id="31ee0-133">Alle rollenzuweisungen abgerufen</span><span class="sxs-lookup"><span data-stu-id="31ee0-133">Get all role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="31ee0-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="31ee0-134">Request</span></span>
<span data-ttu-id="31ee0-135">Das folgende Beispiel zeigt eine Anforderung an alle rollenzuweisungen abgerufen:</span><span class="sxs-lookup"><span data-stu-id="31ee0-135">The following example shows a request to get all role assignments:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments
```
##### <a name="response"></a><span data-ttu-id="31ee0-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="31ee0-136">Response</span></span>
<span data-ttu-id="31ee0-137">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="31ee0-137">The following example shows the response.</span></span> <span data-ttu-id="31ee0-138">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="31ee0-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="31ee0-139">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="31ee0-139">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```
### <a name="get-active-role-assignments"></a><span data-ttu-id="31ee0-140">Abrufen der aktiven rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="31ee0-140">Get active role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="31ee0-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="31ee0-141">Request</span></span> 
<span data-ttu-id="31ee0-142">Das folgende Beispiel zeigt eine Anforderung zum aktiven rollenzuweisungen Abfrage:</span><span class="sxs-lookup"><span data-stu-id="31ee0-142">The following example shows a request to query active role assignments:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true
```
##### <a name="response"></a><span data-ttu-id="31ee0-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="31ee0-143">Response</span></span>
<span data-ttu-id="31ee0-144">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="31ee0-144">The following example shows the response.</span></span> <span data-ttu-id="31ee0-145">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="31ee0-145">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="31ee0-146">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="31ee0-146">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_62e90394-69f5-4237-9190-012177145e10",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "62e90394-69f5-4237-9190-012177145e10",
            "isElevated": true,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "isElevated": true,
            "expirationDateTime": "2017-07-25T17:38:49.563Z",
            "resultMessage": null
        }
  ]
}
```
### <a name="get-permanent-role-assignments"></a><span data-ttu-id="31ee0-147">Abrufen der permanente rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="31ee0-147">Get permanent role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="31ee0-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="31ee0-148">Request</span></span> 
<span data-ttu-id="31ee0-149">Das folgende Beispiel zeigt eine Anforderung an die Abfrage permanente rollenzuweisungen, wobei ``expirationDateTime`` Wert ist ``null``:</span><span class="sxs-lookup"><span data-stu-id="31ee0-149">The following example shows a request to query permanent role assignments, where ``expirationDateTime`` value is ``null``:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20eq%20null
```
##### <a name="response"></a><span data-ttu-id="31ee0-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="31ee0-150">Response</span></span>
<span data-ttu-id="31ee0-151">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="31ee0-151">The following example shows the response.</span></span> <span data-ttu-id="31ee0-152">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="31ee0-152">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="31ee0-153">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="31ee0-153">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_194ae4cb-b126-40b2-bd5b-6091b380977d",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "194ae4cb-b126-40b2-bd5b-6091b380977d",
            "isElevated": true,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_44367163-eba1-44c3-98af-f5787879f96a",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "44367163-eba1-44c3-98af-f5787879f96a",
            "isElevated": true,
            "expirationDateTime": null,
            "resultMessage": null
        }
  ]
}
```
### <a name="get-eligible-role-assignments"></a><span data-ttu-id="31ee0-154">Abrufen von zu auswählbaren rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="31ee0-154">Get eligible role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="31ee0-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="31ee0-155">Request</span></span> 
<span data-ttu-id="31ee0-156">Das folgende Beispiel zeigt eine Anforderung an die Abfrage zu auswählbaren rollenzuweisungen, einschließlich der aktiven und inaktiven:</span><span class="sxs-lookup"><span data-stu-id="31ee0-156">The following example shows a request to query eligible role assignments, including the active and non-active ones:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20ne%20null%20or%20isElevated%20eq%20false
```
##### <a name="response"></a><span data-ttu-id="31ee0-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="31ee0-157">Response</span></span> 
<span data-ttu-id="31ee0-158">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="31ee0-158">The following example shows the response.</span></span> <span data-ttu-id="31ee0-159">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="31ee0-159">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="31ee0-160">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="31ee0-160">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "isElevated": true,
            "expirationDateTime": "2017-07-25T18:42:26.823Z",
            "resultMessage": null
        },
        {
            "id": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81_194ae4cb-b126-40b2-bd5b-6091b380977d",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81",
            "roleId": "194ae4cb-b126-40b2-bd5b-6091b380977d",
            "isElevated": false,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81_9360feb5-f418-4baa-8175-e2a00bac4301",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81",
            "roleId": "9360feb5-f418-4baa-8175-e2a00bac4301",
            "isElevated": false,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81_95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "isElevated": false,
            "expirationDateTime": null,
            "resultMessage": null
        }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignment-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
