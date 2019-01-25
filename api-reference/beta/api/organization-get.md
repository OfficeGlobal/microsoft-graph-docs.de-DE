---
title: Organisation abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen der jeweils aktuell authentifizierten Organisation abrufen.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0313fb5912d8cc9e12319fafac518becfee105a7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520081"
---
# <a name="get-organization"></a><span data-ttu-id="e26bf-103">Organisation abrufen</span><span class="sxs-lookup"><span data-stu-id="e26bf-103">Get organization</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e26bf-104">Mit dieser API können Sie die Eigenschaften und Beziehungen der jeweils aktuell authentifizierten Organisation abrufen.</span><span class="sxs-lookup"><span data-stu-id="e26bf-104">Retrieve the properties and relationships of currently authenticated organization.</span></span>

<span data-ttu-id="e26bf-105">Da die Ressource **Organisation** [Extensions](/graph/extensibility-overview)unterstützt, können Sie auch die `GET` Vorgang zum Abrufen von benutzerdefinierten Eigenschaften und Erweiterungsdaten in einer Instanz der **Organisation** .</span><span class="sxs-lookup"><span data-stu-id="e26bf-105">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **organization** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="e26bf-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e26bf-106">Permissions</span></span>

<span data-ttu-id="e26bf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e26bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e26bf-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e26bf-109">Permission type</span></span> | <span data-ttu-id="e26bf-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e26bf-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e26bf-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e26bf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e26bf-112">User.Read, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e26bf-112">User.Read, Directory.Read.All</span></span> |
|<span data-ttu-id="e26bf-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e26bf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e26bf-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e26bf-114">Not supported.</span></span> |
|<span data-ttu-id="e26bf-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e26bf-115">Application</span></span> | <span data-ttu-id="e26bf-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e26bf-116">Directory.Read.All</span></span> |

> <span data-ttu-id="e26bf-117">Hinweis: Anwendungen, denen die User.Read-Berechtigung gewährt wurde, können nur die *id*-, *displayName*- und *verifiedDomains*-Eigenschaften der Organisation lesen.</span><span class="sxs-lookup"><span data-stu-id="e26bf-117">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="e26bf-118">Alle anderen Eigenschaften geben `null`-Werte zurück.</span><span class="sxs-lookup"><span data-stu-id="e26bf-118">All other properties will return with `null` values.</span></span> <span data-ttu-id="e26bf-119">Verwenden Sie zum Lesen aller Eigenschaften Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="e26bf-119">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="e26bf-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e26bf-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e26bf-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e26bf-121">Optional query parameters</span></span>

<span data-ttu-id="e26bf-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e26bf-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e26bf-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e26bf-123">Request headers</span></span>

| <span data-ttu-id="e26bf-124">Name</span><span class="sxs-lookup"><span data-stu-id="e26bf-124">Name</span></span>       | <span data-ttu-id="e26bf-125">Typ</span><span class="sxs-lookup"><span data-stu-id="e26bf-125">Type</span></span> | <span data-ttu-id="e26bf-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e26bf-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e26bf-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="e26bf-127">Authorization</span></span>  | <span data-ttu-id="e26bf-128">string</span><span class="sxs-lookup"><span data-stu-id="e26bf-128">string</span></span>  | <span data-ttu-id="e26bf-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e26bf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e26bf-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e26bf-131">Request body</span></span>

<span data-ttu-id="e26bf-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e26bf-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e26bf-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="e26bf-133">Response</span></span>

<span data-ttu-id="e26bf-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [organization](../resources/organization.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e26bf-134">If successful, this method returns a `200 OK` response code and [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e26bf-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e26bf-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e26bf-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e26bf-136">Request</span></span>

<span data-ttu-id="e26bf-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e26bf-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```http
GET https://graph.microsoft.com/beta/organization
```

##### <a name="response"></a><span data-ttu-id="e26bf-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="e26bf-138">Response</span></span>

<span data-ttu-id="e26bf-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e26bf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 411

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#organization",
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "datetime-value",
          "capabilityStatus": "capabilityStatus-value",
          "service": "service-value",
          "servicePlanId": "servicePlanId-value"
        }
      ],
      "businessPhones": [
        "businessPhones-value"
      ],
      "city": "city-value",
      "country": "country-value",
      "countryLetterCode": "countryLetterCode-value",
      "displayName": "displayName-value"
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="e26bf-142">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="e26bf-142">See also</span></span>

- [<span data-ttu-id="e26bf-143">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="e26bf-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="e26bf-144">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="e26bf-144">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/organization-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
