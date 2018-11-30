---
title: Erstellen von SynchronisationVorlage
description: Erstellen Sie eine neue Vorlage Synchronisierung für eine bestimmte Anwendung.
ms.openlocfilehash: 1c7bc08eee4088796123d3c7fa2cac5c83becac2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060090"
---
# <a name="create-synchronizationtemplate"></a><span data-ttu-id="b4962-103">Erstellen von SynchronisationVorlage</span><span class="sxs-lookup"><span data-stu-id="b4962-103">Create synchronizationTemplate</span></span>

> <span data-ttu-id="b4962-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b4962-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4962-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b4962-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b4962-106">Erstellen Sie eine neue Vorlage Synchronisierung für eine bestimmte Anwendung.</span><span class="sxs-lookup"><span data-stu-id="b4962-106">Create a new synchronization template for a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4962-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b4962-107">Permissions</span></span>
<span data-ttu-id="b4962-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4962-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4962-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b4962-110">Permission type</span></span>                        | <span data-ttu-id="b4962-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b4962-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4962-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b4962-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="b4962-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4962-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="b4962-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b4962-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="b4962-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4962-115">Not supported.</span></span>|
|<span data-ttu-id="b4962-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b4962-116">Application</span></span>                            |<span data-ttu-id="b4962-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4962-117">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="b4962-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4962-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/synchronization/templates/
```

## <a name="request-headers"></a><span data-ttu-id="b4962-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b4962-119">Request headers</span></span>

| <span data-ttu-id="b4962-120">Name</span><span class="sxs-lookup"><span data-stu-id="b4962-120">Name</span></span>           | <span data-ttu-id="b4962-121">Typ</span><span class="sxs-lookup"><span data-stu-id="b4962-121">Type</span></span>    | <span data-ttu-id="b4962-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4962-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="b4962-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4962-123">Authorization</span></span>  | <span data-ttu-id="b4962-124">string</span><span class="sxs-lookup"><span data-stu-id="b4962-124">string</span></span>  | <span data-ttu-id="b4962-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b4962-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4962-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b4962-127">Request body</span></span>

<span data-ttu-id="b4962-128">Geben Sie im Textkörper Anforderung [SynchronisationVorlage](../resources/synchronization-synchronizationtemplate.md) -Objekt erstellt werden soll.</span><span class="sxs-lookup"><span data-stu-id="b4962-128">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to be created.</span></span> <span data-ttu-id="b4962-129">Die `id`, `applicationId` und `factoryTag` Eigenschaften sind erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b4962-129">The `id`, `applicationId` and `factoryTag` properties are required.</span></span> <span data-ttu-id="b4962-130">Wenn keine `schema` erfolgt mit der Vorlage Standardschema verknüpft die `factoryTag` Eigenschaft verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="b4962-130">When no `schema` is provided with the template, the default schema associated with the `factoryTag` property will be used.</span></span>

### <a name="response"></a><span data-ttu-id="b4962-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4962-131">Response</span></span>

<span data-ttu-id="b4962-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [SynchronisationVorlage](../resources/synchronization-synchronizationtemplate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b4962-132">If successful, this method returns a `201 Created` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="b4962-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b4962-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b4962-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4962-134">Request</span></span>
<span data-ttu-id="b4962-135">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b4962-135">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_synchronizationtemplate_from_synchronization"
}-->
```http
POST https://graph.microsoft.com/beta/applications/{id}/synchronization/templates
Content-type: application/json

{ 
    "id": "SCIM-Test1",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```

##### <a name="response"></a><span data-ttu-id="b4962-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4962-136">Response</span></span>
<span data-ttu-id="b4962-137">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="b4962-137">The following is an example of a response.</span></span>
><span data-ttu-id="b4962-138">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="b4962-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b4962-139">Alle Eigenschaften werden in eine tatsächliche Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b4962-139">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 201 Created

{
    "id": "SCIM-Test1",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM",
    "schema": {
        "directories": [],
        "synchronizationRules": []
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->