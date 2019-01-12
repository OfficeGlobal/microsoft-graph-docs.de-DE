---
title: AdministrativeUnit abrufen
description: Rufen Sie die Eigenschaften und die Beziehungen eines AdministrativeUnit-Objekts ab.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d91db6fa5365d9e0db7f655ecab75fa594b4ea8b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931944"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="ed222-103">AdministrativeUnit abrufen</span><span class="sxs-lookup"><span data-stu-id="ed222-103">Get administrativeUnit</span></span>

> <span data-ttu-id="ed222-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ed222-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed222-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ed222-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ed222-106">Rufen Sie die Eigenschaften und die Beziehungen eines [AdministrativeUnit](../resources/administrativeunit.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="ed222-106">Retrieve the properties and relationships of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="ed222-107">Da die Ressource **AdministrativeUnit** [Extensions](/graph/extensibility-overview)unterstützt, können Sie auch die `GET` Vorgang zum Abrufen von benutzerdefinierten Eigenschaften und Erweiterungsdaten in eine **AdministrativeUnit** -Instanz.</span><span class="sxs-lookup"><span data-stu-id="ed222-107">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **administrativeUnit** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed222-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ed222-108">Permissions</span></span>
<span data-ttu-id="ed222-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed222-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ed222-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ed222-111">Permission type</span></span>      | <span data-ttu-id="ed222-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ed222-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed222-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ed222-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ed222-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ed222-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ed222-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ed222-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed222-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed222-116">Not supported.</span></span>    |
|<span data-ttu-id="ed222-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ed222-117">Application</span></span> | <span data-ttu-id="ed222-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed222-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed222-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed222-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ed222-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ed222-120">Optional query parameters</span></span>
<span data-ttu-id="ed222-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ed222-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed222-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ed222-122">Request headers</span></span>
| <span data-ttu-id="ed222-123">Name</span><span class="sxs-lookup"><span data-stu-id="ed222-123">Name</span></span>      |<span data-ttu-id="ed222-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ed222-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ed222-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed222-125">Authorization</span></span>  | <span data-ttu-id="ed222-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ed222-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed222-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ed222-128">Request body</span></span>
<span data-ttu-id="ed222-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ed222-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed222-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed222-130">Response</span></span>

<span data-ttu-id="ed222-131">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [AdministrativeUnit](../resources/administrativeunit.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ed222-131">If successful, this method returns a `200 OK` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ed222-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ed222-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ed222-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed222-133">Request</span></span>
<span data-ttu-id="ed222-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ed222-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_administrativeunit"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}
```
##### <a name="response"></a><span data-ttu-id="ed222-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed222-135">Response</span></span>
<span data-ttu-id="ed222-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ed222-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="ed222-139">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="ed222-139">See also</span></span>

- [<span data-ttu-id="ed222-140">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="ed222-140">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="ed222-141">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="ed222-141">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
