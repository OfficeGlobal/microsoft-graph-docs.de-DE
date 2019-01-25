---
title: Erstellen von SynchronisationVorlage
description: Erstellen Sie eine neue Vorlage Synchronisierung für eine bestimmte Anwendung.
localization_priority: Normal
ms.openlocfilehash: ce519b57766956b10d05b6b3745ca16f609b597c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509889"
---
# <a name="create-synchronizationtemplate"></a><span data-ttu-id="df8f8-103">Erstellen von SynchronisationVorlage</span><span class="sxs-lookup"><span data-stu-id="df8f8-103">Create synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df8f8-104">Erstellen Sie eine neue Vorlage Synchronisierung für eine bestimmte Anwendung.</span><span class="sxs-lookup"><span data-stu-id="df8f8-104">Create a new synchronization template for a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="df8f8-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="df8f8-105">Permissions</span></span>
<span data-ttu-id="df8f8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df8f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df8f8-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="df8f8-108">Permission type</span></span>                        | <span data-ttu-id="df8f8-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="df8f8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="df8f8-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="df8f8-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="df8f8-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df8f8-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="df8f8-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="df8f8-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="df8f8-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="df8f8-113">Not supported.</span></span>|
|<span data-ttu-id="df8f8-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="df8f8-114">Application</span></span>                            |<span data-ttu-id="df8f8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="df8f8-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="df8f8-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="df8f8-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/synchronization/templates/
```

## <a name="request-headers"></a><span data-ttu-id="df8f8-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="df8f8-117">Request headers</span></span>

| <span data-ttu-id="df8f8-118">Name</span><span class="sxs-lookup"><span data-stu-id="df8f8-118">Name</span></span>           | <span data-ttu-id="df8f8-119">Typ</span><span class="sxs-lookup"><span data-stu-id="df8f8-119">Type</span></span>    | <span data-ttu-id="df8f8-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df8f8-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="df8f8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="df8f8-121">Authorization</span></span>  | <span data-ttu-id="df8f8-122">string</span><span class="sxs-lookup"><span data-stu-id="df8f8-122">string</span></span>  | <span data-ttu-id="df8f8-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="df8f8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df8f8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="df8f8-125">Request body</span></span>

<span data-ttu-id="df8f8-126">Geben Sie im Textkörper Anforderung [SynchronisationVorlage](../resources/synchronization-synchronizationtemplate.md) -Objekt erstellt werden soll.</span><span class="sxs-lookup"><span data-stu-id="df8f8-126">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to be created.</span></span> <span data-ttu-id="df8f8-127">Die `id`, `applicationId` und `factoryTag` Eigenschaften sind erforderlich.</span><span class="sxs-lookup"><span data-stu-id="df8f8-127">The `id`, `applicationId` and `factoryTag` properties are required.</span></span> <span data-ttu-id="df8f8-128">Wenn keine `schema` erfolgt mit der Vorlage Standardschema verknüpft die `factoryTag` Eigenschaft verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="df8f8-128">When no `schema` is provided with the template, the default schema associated with the `factoryTag` property will be used.</span></span>

### <a name="response"></a><span data-ttu-id="df8f8-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="df8f8-129">Response</span></span>

<span data-ttu-id="df8f8-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [SynchronisationVorlage](../resources/synchronization-synchronizationtemplate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="df8f8-130">If successful, this method returns a `201 Created` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="df8f8-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="df8f8-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="df8f8-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="df8f8-132">Request</span></span>
<span data-ttu-id="df8f8-133">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="df8f8-133">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="df8f8-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="df8f8-134">Response</span></span>
<span data-ttu-id="df8f8-135">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="df8f8-135">The following is an example of a response.</span></span>
><span data-ttu-id="df8f8-136">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="df8f8-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="df8f8-137">Alle Eigenschaften werden in eine tatsächliche Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="df8f8-137">All the properties will be returned in an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
