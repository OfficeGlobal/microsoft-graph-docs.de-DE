---
title: Ressourcentyp alertTrigger
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: cda1dde9b22b9304fd412405758435be2f6143bc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516315"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="980d1-104">Ressourcentyp alertTrigger</span><span class="sxs-lookup"><span data-stu-id="980d1-104">alertTrigger resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="980d1-105">Enthält Informationen zu den Eigenschaften, die eine Erkennung ausgelöst (Eigenschaften sind in der Warnung Entität vorhanden).</span><span class="sxs-lookup"><span data-stu-id="980d1-105">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="980d1-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="980d1-106">Properties</span></span>

| <span data-ttu-id="980d1-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="980d1-107">Property</span></span>   | <span data-ttu-id="980d1-108">Typ</span><span class="sxs-lookup"><span data-stu-id="980d1-108">Type</span></span>|<span data-ttu-id="980d1-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="980d1-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="980d1-110">name</span><span class="sxs-lookup"><span data-stu-id="980d1-110">name</span></span>|<span data-ttu-id="980d1-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="980d1-111">String</span></span>|<span data-ttu-id="980d1-112">Der Name der Eigenschaft, die als eine Erkennung Trigger.</span><span class="sxs-lookup"><span data-stu-id="980d1-112">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="980d1-113">type</span><span class="sxs-lookup"><span data-stu-id="980d1-113">type</span></span>|<span data-ttu-id="980d1-114">String</span><span class="sxs-lookup"><span data-stu-id="980d1-114">String</span></span>|<span data-ttu-id="980d1-115">Typ der Eigenschaft im Schlüssel / Wert-Paar für Auslegung.</span><span class="sxs-lookup"><span data-stu-id="980d1-115">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="980d1-116">String, Boolean, beispielsweise usw.</span><span class="sxs-lookup"><span data-stu-id="980d1-116">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="980d1-117">Wert</span><span class="sxs-lookup"><span data-stu-id="980d1-117">value</span></span>|<span data-ttu-id="980d1-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="980d1-118">String</span></span>|<span data-ttu-id="980d1-119">Der Wert der Eigenschaft, die als eine Erkennung Trigger.</span><span class="sxs-lookup"><span data-stu-id="980d1-119">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="980d1-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="980d1-120">JSON representation</span></span>

<span data-ttu-id="980d1-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="980d1-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}

```

## <a name="example"></a><span data-ttu-id="980d1-122">Beispiel</span><span class="sxs-lookup"><span data-stu-id="980d1-122">Example</span></span>

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/alerttrigger.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
