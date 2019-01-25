---
title: AdministrativeUnit abrufen
description: Rufen Sie die Eigenschaften und die Beziehungen eines AdministrativeUnit-Objekts ab.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 588d116d546503fa8db6c8ba56c5d0e328a10b8a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521607"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="11bcf-103">AdministrativeUnit abrufen</span><span class="sxs-lookup"><span data-stu-id="11bcf-103">Get administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11bcf-104">Rufen Sie die Eigenschaften und die Beziehungen eines [AdministrativeUnit](../resources/administrativeunit.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="11bcf-104">Retrieve the properties and relationships of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="11bcf-105">Da die Ressource **AdministrativeUnit** [Extensions](/graph/extensibility-overview)unterstützt, können Sie auch die `GET` Vorgang zum Abrufen von benutzerdefinierten Eigenschaften und Erweiterungsdaten in eine **AdministrativeUnit** -Instanz.</span><span class="sxs-lookup"><span data-stu-id="11bcf-105">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **administrativeUnit** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="11bcf-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="11bcf-106">Permissions</span></span>
<span data-ttu-id="11bcf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11bcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="11bcf-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="11bcf-109">Permission type</span></span>      | <span data-ttu-id="11bcf-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="11bcf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11bcf-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="11bcf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="11bcf-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="11bcf-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="11bcf-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="11bcf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11bcf-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="11bcf-114">Not supported.</span></span>    |
|<span data-ttu-id="11bcf-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="11bcf-115">Application</span></span> | <span data-ttu-id="11bcf-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11bcf-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="11bcf-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="11bcf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="11bcf-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="11bcf-118">Optional query parameters</span></span>
<span data-ttu-id="11bcf-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="11bcf-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="11bcf-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="11bcf-120">Request headers</span></span>
| <span data-ttu-id="11bcf-121">Name</span><span class="sxs-lookup"><span data-stu-id="11bcf-121">Name</span></span>      |<span data-ttu-id="11bcf-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11bcf-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="11bcf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="11bcf-123">Authorization</span></span>  | <span data-ttu-id="11bcf-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="11bcf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11bcf-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="11bcf-126">Request body</span></span>
<span data-ttu-id="11bcf-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="11bcf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11bcf-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="11bcf-128">Response</span></span>

<span data-ttu-id="11bcf-129">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [AdministrativeUnit](../resources/administrativeunit.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="11bcf-129">If successful, this method returns a `200 OK` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="11bcf-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="11bcf-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="11bcf-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="11bcf-131">Request</span></span>
<span data-ttu-id="11bcf-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="11bcf-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_administrativeunit"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}
```
##### <a name="response"></a><span data-ttu-id="11bcf-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="11bcf-133">Response</span></span>
<span data-ttu-id="11bcf-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="11bcf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value",
  "id": "id-value"
}
```

## <a name="see-also"></a><span data-ttu-id="11bcf-137">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="11bcf-137">See also</span></span>

- [<span data-ttu-id="11bcf-138">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="11bcf-138">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="11bcf-139">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="11bcf-139">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
