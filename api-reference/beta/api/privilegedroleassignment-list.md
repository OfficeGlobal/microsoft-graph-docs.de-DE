---
title: Liste privilegedRoleAssignments
description: Abrufen einer Liste von PrivilegedRoleAssignment-Objekten, die alle rollenzuweisungen für die Organisation entsprechen.
ms.openlocfilehash: 7642768348e2fff43f52c6865cabf85aa16ef893
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064157"
---
# <a name="list-privilegedroleassignments"></a><span data-ttu-id="35982-103">Liste privilegedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="35982-103">List privilegedRoleAssignments</span></span>

> <span data-ttu-id="35982-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="35982-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35982-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="35982-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="35982-106">Abrufen einer Liste von [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) -Objekten, die alle rollenzuweisungen für die Organisation entsprechen.</span><span class="sxs-lookup"><span data-stu-id="35982-106">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects, which correspond to all role assignments for the organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="35982-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="35982-107">Permissions</span></span>
<span data-ttu-id="35982-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35982-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="35982-110">Der Requestor muss eine der folgenden Rollen verfügen: _Berechtigten Rolle Administrators_, _Globaler Administrator_, _Sicherheitsadministrator_oder _Sicherheit Leser_.</span><span class="sxs-lookup"><span data-stu-id="35982-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="35982-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="35982-111">Permission type</span></span>      | <span data-ttu-id="35982-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="35982-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35982-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="35982-113">Delegated (work or school account)</span></span> | <span data-ttu-id="35982-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="35982-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="35982-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="35982-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35982-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="35982-116">Not supported.</span></span>    |
|<span data-ttu-id="35982-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="35982-117">Application</span></span> | <span data-ttu-id="35982-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="35982-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="35982-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="35982-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="35982-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="35982-120">Optional query parameters</span></span>
<span data-ttu-id="35982-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="35982-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="35982-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="35982-122">Request headers</span></span>
| <span data-ttu-id="35982-123">Name</span><span class="sxs-lookup"><span data-stu-id="35982-123">Name</span></span>      |<span data-ttu-id="35982-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="35982-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="35982-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="35982-125">Authorization</span></span>  | <span data-ttu-id="35982-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="35982-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35982-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="35982-128">Request body</span></span>
<span data-ttu-id="35982-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="35982-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35982-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="35982-130">Response</span></span>

<span data-ttu-id="35982-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [PrivilegedRoleAssignment](../resources/privilegedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="35982-131">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="35982-132">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="35982-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="35982-133">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="35982-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="examples"></a><span data-ttu-id="35982-134">Beispiele</span><span class="sxs-lookup"><span data-stu-id="35982-134">Examples</span></span>
### <a name="get-all-role-assignments"></a><span data-ttu-id="35982-135">Alle rollenzuweisungen abgerufen</span><span class="sxs-lookup"><span data-stu-id="35982-135">Get all role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="35982-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="35982-136">Request</span></span>
<span data-ttu-id="35982-137">Das folgende Beispiel zeigt eine Anforderung an alle rollenzuweisungen abgerufen:</span><span class="sxs-lookup"><span data-stu-id="35982-137">The following example shows a request to get all role assignments:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments
```
##### <a name="response"></a><span data-ttu-id="35982-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="35982-138">Response</span></span>
<span data-ttu-id="35982-139">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="35982-139">The following example shows the response.</span></span> <span data-ttu-id="35982-140">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="35982-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="35982-141">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="35982-141">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-active-role-assignments"></a><span data-ttu-id="35982-142">Abrufen der aktiven rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="35982-142">Get active role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="35982-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="35982-143">Request</span></span> 
<span data-ttu-id="35982-144">Das folgende Beispiel zeigt eine Anforderung zum aktiven rollenzuweisungen Abfrage:</span><span class="sxs-lookup"><span data-stu-id="35982-144">The following example shows a request to query active role assignments:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true
```
##### <a name="response"></a><span data-ttu-id="35982-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="35982-145">Response</span></span>
<span data-ttu-id="35982-146">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="35982-146">The following example shows the response.</span></span> <span data-ttu-id="35982-147">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="35982-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="35982-148">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="35982-148">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-permanent-role-assignments"></a><span data-ttu-id="35982-149">Abrufen der permanente rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="35982-149">Get permanent role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="35982-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="35982-150">Request</span></span> 
<span data-ttu-id="35982-151">Das folgende Beispiel zeigt eine Anforderung an die Abfrage permanente rollenzuweisungen, wobei ``expirationDateTime`` Wert ist ``null``:</span><span class="sxs-lookup"><span data-stu-id="35982-151">The following example shows a request to query permanent role assignments, where ``expirationDateTime`` value is ``null``:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20eq%20null
```
##### <a name="response"></a><span data-ttu-id="35982-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="35982-152">Response</span></span>
<span data-ttu-id="35982-153">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="35982-153">The following example shows the response.</span></span> <span data-ttu-id="35982-154">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="35982-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="35982-155">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="35982-155">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-eligible-role-assignments"></a><span data-ttu-id="35982-156">Abrufen von zu auswählbaren rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="35982-156">Get eligible role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="35982-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="35982-157">Request</span></span> 
<span data-ttu-id="35982-158">Das folgende Beispiel zeigt eine Anforderung an die Abfrage zu auswählbaren rollenzuweisungen, einschließlich der aktiven und inaktiven:</span><span class="sxs-lookup"><span data-stu-id="35982-158">The following example shows a request to query eligible role assignments, including the active and non-active ones:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20ne%20null%20or%20isElevated%20eq%20false
```
##### <a name="response"></a><span data-ttu-id="35982-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="35982-159">Response</span></span> 
<span data-ttu-id="35982-160">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="35982-160">The following example shows the response.</span></span> <span data-ttu-id="35982-161">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="35982-161">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="35982-162">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="35982-162">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List privilegedRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
