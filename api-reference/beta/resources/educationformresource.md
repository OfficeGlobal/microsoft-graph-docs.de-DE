---
title: educationFormResource-Ressourcentyp
description: Eine Unterklasse von educationResource. Diese Ressource ist ein Formular.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5e0b03eeea8c0e9d22a9f7279c821f6d90211470
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2019
ms.locfileid: "30801005"
---
# <a name="educationformresource-resource-type"></a><span data-ttu-id="a5dd0-104">educationFormResource-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a5dd0-104">educationFormResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5dd0-105">Eine Unterklasse von [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="a5dd0-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="a5dd0-106">Diese Ressource ist ein Formular.</span><span class="sxs-lookup"><span data-stu-id="a5dd0-106">This resource is a form.</span></span>


## <a name="properties"></a><span data-ttu-id="a5dd0-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a5dd0-107">Properties</span></span>
| <span data-ttu-id="a5dd0-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a5dd0-108">Property</span></span>     | <span data-ttu-id="a5dd0-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a5dd0-109">Type</span></span>   |<span data-ttu-id="a5dd0-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a5dd0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5dd0-111">originalFormId</span><span class="sxs-lookup"><span data-stu-id="a5dd0-111">originalFormId</span></span>|<span data-ttu-id="a5dd0-112">String</span><span class="sxs-lookup"><span data-stu-id="a5dd0-112">String</span></span>|<span data-ttu-id="a5dd0-113">Die ursprüngliche ID des Formulars.</span><span class="sxs-lookup"><span data-stu-id="a5dd0-113">Original id of the Form.</span></span>|
|<span data-ttu-id="a5dd0-114">formId</span><span class="sxs-lookup"><span data-stu-id="a5dd0-114">formId</span></span>|<span data-ttu-id="a5dd0-115">String</span><span class="sxs-lookup"><span data-stu-id="a5dd0-115">String</span></span>|<span data-ttu-id="a5dd0-116">Die ID des Formulars.</span><span class="sxs-lookup"><span data-stu-id="a5dd0-116">Id of the Form.</span></span>|
|<span data-ttu-id="a5dd0-117">isGroupForm</span><span class="sxs-lookup"><span data-stu-id="a5dd0-117">isGroupForm</span></span>|<span data-ttu-id="a5dd0-118">Boolesch</span><span class="sxs-lookup"><span data-stu-id="a5dd0-118">Boolean</span></span>|<span data-ttu-id="a5dd0-119">Gibt an, ob das Formular zu einer Klassengruppe gehört.</span><span class="sxs-lookup"><span data-stu-id="a5dd0-119">Whether the Form belongs to a class group.</span></span>|
|<span data-ttu-id="a5dd0-120">viewUrl</span><span class="sxs-lookup"><span data-stu-id="a5dd0-120">viewUrl</span></span>|<span data-ttu-id="a5dd0-121">String</span><span class="sxs-lookup"><span data-stu-id="a5dd0-121">String</span></span>|<span data-ttu-id="a5dd0-122">Schüler-URL für das Formular.</span><span class="sxs-lookup"><span data-stu-id="a5dd0-122">Student URL for the Form.</span></span>|
|<span data-ttu-id="a5dd0-123">viewUrl</span><span class="sxs-lookup"><span data-stu-id="a5dd0-123">viewUrl</span></span>|<span data-ttu-id="a5dd0-124">String</span><span class="sxs-lookup"><span data-stu-id="a5dd0-124">String</span></span>|<span data-ttu-id="a5dd0-125">Schüler-URL für das Formular.</span><span class="sxs-lookup"><span data-stu-id="a5dd0-125">Student URL for the Form.</span></span>|
|<span data-ttu-id="a5dd0-126">editUrl</span><span class="sxs-lookup"><span data-stu-id="a5dd0-126">editUrl</span></span>|<span data-ttu-id="a5dd0-127">String</span><span class="sxs-lookup"><span data-stu-id="a5dd0-127">String</span></span>|<span data-ttu-id="a5dd0-128">Lehrer-URL für das Formular.</span><span class="sxs-lookup"><span data-stu-id="a5dd0-128">Teacher URL for the Form.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a5dd0-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a5dd0-129">JSON representation</span></span>

<span data-ttu-id="a5dd0-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a5dd0-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFormResource"
}-->

```json
{
  "originalFormId": "String"
  "formId": "String"
  "isGroupForm": "Boolean"
  "viewUrl": "String"
  "editUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationFormResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationformresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
