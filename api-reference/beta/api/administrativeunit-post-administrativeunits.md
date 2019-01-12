---
title: Erstellen von administrativeUnit
description: Verwenden Sie diese API, um eine neue AdministrativeUnit erstellen.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fb918d690ceaaa232b4911b5f47a2b381a79444d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917167"
---
# <a name="create-administrativeunit"></a><span data-ttu-id="991b8-103">Erstellen von administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="991b8-103">Create administrativeUnit</span></span>

> <span data-ttu-id="991b8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="991b8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="991b8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="991b8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="991b8-106">Verwenden Sie diese API, um eine neue [AdministrativeUnit](../resources/administrativeunit.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="991b8-106">Use this API to create a new [administrativeUnit](../resources/administrativeunit.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="991b8-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="991b8-107">Permissions</span></span>
<span data-ttu-id="991b8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="991b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="991b8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="991b8-110">Permission type</span></span>      | <span data-ttu-id="991b8-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="991b8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="991b8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="991b8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="991b8-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="991b8-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="991b8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="991b8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="991b8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="991b8-115">Not supported.</span></span>    |
|<span data-ttu-id="991b8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="991b8-116">Application</span></span> | <span data-ttu-id="991b8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="991b8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="991b8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="991b8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits

```
## <a name="request-headers"></a><span data-ttu-id="991b8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="991b8-119">Request headers</span></span>
| <span data-ttu-id="991b8-120">Name</span><span class="sxs-lookup"><span data-stu-id="991b8-120">Name</span></span>      |<span data-ttu-id="991b8-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="991b8-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="991b8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="991b8-122">Authorization</span></span>  | <span data-ttu-id="991b8-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="991b8-p103">Bearer {token}. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="991b8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="991b8-125">Request body</span></span>
<span data-ttu-id="991b8-126">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [AdministrativeUnit](../resources/administrativeunit.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="991b8-126">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="991b8-127">Da die Ressource **AdministrativeUnit** [Extensions](/graph/extensibility-overview)unterstützt, können Sie die `POST` Vorgang und die administrative Einheit beim Erstellen benutzerdefinierte Eigenschaften mit Ihren eigenen Daten hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="991b8-127">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the administrative unit while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="991b8-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="991b8-128">Response</span></span>

<span data-ttu-id="991b8-129">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code und [AdministrativeUnit](../resources/administrativeunit.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="991b8-129">If successful, this method returns `201 Created` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="991b8-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="991b8-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="991b8-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="991b8-131">Request</span></span>
<span data-ttu-id="991b8-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="991b8-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_administrativeunit_from_administrativeunits"
}-->
```http
POST https://graph.microsoft.com/beta/administrativeUnits
Content-type: application/json
Content-length: 150

{
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "true"
}
```
<span data-ttu-id="991b8-133">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [AdministrativeUnit](../resources/administrativeunit.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="991b8-133">In the request body, supply a JSON representation of [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="991b8-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="991b8-134">Response</span></span>
<span data-ttu-id="991b8-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="991b8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 172

{
  "administrativeUnit": {
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "true",
    "id": "7a3dc8f3-b3a0-4164-9a99-ed36f3af039f"
  }
}
```

## <a name="see-also"></a><span data-ttu-id="991b8-138">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="991b8-138">See also</span></span>

- [<span data-ttu-id="991b8-139">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="991b8-139">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="991b8-140">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="991b8-140">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
