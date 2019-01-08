---
title: Organisation abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen der jeweils aktuell authentifizierten Organisation abrufen.
ms.openlocfilehash: f3d2ca5c6881a06f397101a0050fe29f8a646614
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748283"
---
# <a name="get-organization"></a><span data-ttu-id="9304f-103">Organisation abrufen</span><span class="sxs-lookup"><span data-stu-id="9304f-103">Get organization</span></span>

> <span data-ttu-id="9304f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9304f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9304f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9304f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9304f-106">Mit dieser API können Sie die Eigenschaften und Beziehungen der jeweils aktuell authentifizierten Organisation abrufen.</span><span class="sxs-lookup"><span data-stu-id="9304f-106">Retrieve the properties and relationships of currently authenticated organization.</span></span>

<span data-ttu-id="9304f-107">Da die Ressource **Organisation** [Extensions](/graph/extensibility-overview)unterstützt, können Sie auch die `GET` Vorgang zum Abrufen von benutzerdefinierten Eigenschaften und Erweiterungsdaten in einer Instanz der **Organisation** .</span><span class="sxs-lookup"><span data-stu-id="9304f-107">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **organization** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="9304f-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9304f-108">Permissions</span></span>

<span data-ttu-id="9304f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9304f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9304f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9304f-111">Permission type</span></span> | <span data-ttu-id="9304f-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9304f-112">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9304f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9304f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9304f-114">User.Read, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9304f-114">User.Read, Directory.Read.All</span></span> |
|<span data-ttu-id="9304f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9304f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9304f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9304f-116">Not supported.</span></span> |
|<span data-ttu-id="9304f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9304f-117">Application</span></span> | <span data-ttu-id="9304f-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9304f-118">Directory.Read.All</span></span> |

> <span data-ttu-id="9304f-119">Hinweis: Anwendungen, denen die User.Read-Berechtigung gewährt wurde, können nur die *id*-, *displayName*- und *verifiedDomains*-Eigenschaften der Organisation lesen.</span><span class="sxs-lookup"><span data-stu-id="9304f-119">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="9304f-120">Alle anderen Eigenschaften geben `null`-Werte zurück.</span><span class="sxs-lookup"><span data-stu-id="9304f-120">All other properties will return with `null` values.</span></span> <span data-ttu-id="9304f-121">Verwenden Sie zum Lesen aller Eigenschaften Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="9304f-121">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="9304f-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9304f-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9304f-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9304f-123">Optional query parameters</span></span>

<span data-ttu-id="9304f-124">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9304f-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9304f-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9304f-125">Request headers</span></span>

| <span data-ttu-id="9304f-126">Name</span><span class="sxs-lookup"><span data-stu-id="9304f-126">Name</span></span>       | <span data-ttu-id="9304f-127">Typ</span><span class="sxs-lookup"><span data-stu-id="9304f-127">Type</span></span> | <span data-ttu-id="9304f-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9304f-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9304f-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="9304f-129">Authorization</span></span>  | <span data-ttu-id="9304f-130">string</span><span class="sxs-lookup"><span data-stu-id="9304f-130">string</span></span>  | <span data-ttu-id="9304f-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9304f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9304f-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9304f-133">Request body</span></span>

<span data-ttu-id="9304f-134">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9304f-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9304f-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="9304f-135">Response</span></span>

<span data-ttu-id="9304f-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [organization](../resources/organization.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9304f-136">If successful, this method returns a `200 OK` response code and [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9304f-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9304f-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9304f-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9304f-138">Request</span></span>

<span data-ttu-id="9304f-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9304f-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```http
GET https://graph.microsoft.com/beta/organization
```

##### <a name="response"></a><span data-ttu-id="9304f-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="9304f-140">Response</span></span>

<span data-ttu-id="9304f-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9304f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="9304f-144">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="9304f-144">See also</span></span>

- [<span data-ttu-id="9304f-145">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="9304f-145">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="9304f-146">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="9304f-146">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->