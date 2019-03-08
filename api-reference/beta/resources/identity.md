---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/14/2017
title: Identität
localization_priority: Normal
ms.openlocfilehash: 1f2d1f5a305698438748ee69f73b4143b8afd8fa
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481566"
---
# <a name="identity-resource-type"></a><span data-ttu-id="28990-102">Identitäts Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="28990-102">identity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28990-p101">Die **Identity**-Ressource stellt eine Identität von einem _Akteur_ dar. Ein Akteur kann z. B. ein Benutzer, Gerät oder eine Anwendung sein.</span><span class="sxs-lookup"><span data-stu-id="28990-p101">The **Identity** resource represents an identity of an _actor_. For example, an actor can be a user, device, or application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="28990-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="28990-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity", "optionalProperties": ["displayName", "tenantId", "thumbnails"], "openType": true } -->

```json
{
  "displayName": "string",
  "id": "string",
  "tenantId": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

## <a name="properties"></a><span data-ttu-id="28990-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="28990-106">Properties</span></span>

| <span data-ttu-id="28990-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="28990-107">Property</span></span>            | <span data-ttu-id="28990-108">Typ</span><span class="sxs-lookup"><span data-stu-id="28990-108">Type</span></span>   | <span data-ttu-id="28990-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28990-109">Description</span></span>                                                                                                                                                                                                                                                                                                           |
|:--------------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="28990-110">displayName</span><span class="sxs-lookup"><span data-stu-id="28990-110">displayName</span></span>         | <span data-ttu-id="28990-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="28990-111">String</span></span> | <span data-ttu-id="28990-p102">Der Anzeigenamen der Identität. Beachten Sie, dass dieser möglicherweise nicht immer verfügbar oder auf dem neuesten Stand ist. Wenn sich z. B. der Anzeigename eines Benutzers ändert, zeigt die API möglicherweise den neuen Wert in einer zukünftigen Antwort an, aber für die dem Benutzer zugeordneten Elemente wird mit [delta](../api/driveitem-delta.md) nicht angezeigt, dass sie sich geändert haben.</span><span class="sxs-lookup"><span data-stu-id="28990-p102">The identity's display name. Note that this may not always be available or up to date. For example, if a user changes their display name, the API may show the new value in a future response, but the items associated with the user won't show up as having changed when using [delta](../api/driveitem-delta.md).</span></span>  |
| <span data-ttu-id="28990-115">id</span><span class="sxs-lookup"><span data-stu-id="28990-115">id</span></span>                  | <span data-ttu-id="28990-116">String</span><span class="sxs-lookup"><span data-stu-id="28990-116">String</span></span> | <span data-ttu-id="28990-117">Eindeutiger Bezeichner für die Identität.</span><span class="sxs-lookup"><span data-stu-id="28990-117">Unique identifier for the identity.</span></span>                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="28990-118">tenantId</span><span class="sxs-lookup"><span data-stu-id="28990-118">tenantId</span></span>            | <span data-ttu-id="28990-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="28990-119">String</span></span> | <span data-ttu-id="28990-120">Eindeutige Identität des Mandanten (optional).</span><span class="sxs-lookup"><span data-stu-id="28990-120">Unique identity of the tenant (optional).</span></span>                                                                                                                                                                                                                                                                             |

## <a name="remarks"></a><span data-ttu-id="28990-121">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="28990-121">Remarks</span></span>

<span data-ttu-id="28990-p103">Unter gewissen Umständen steht der eindeutige Bezeichner für den Akteur möglicherweise nicht zur Verfügung. In diesem Fall die wird die Eigenschaft **DisplayName** für die Identität zurückgegeben werden, aber die **Id**-Eigenschaft ist aus der Ressource nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="28990-p103">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity",
  "suppressions": [
    "Error: /api-reference/beta/resources/identity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
