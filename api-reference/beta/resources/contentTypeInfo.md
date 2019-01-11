---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentTypeInfo
localization_priority: Normal
ms.openlocfilehash: e394d52a5f7ed5e8dce1c61d31d787d62bd36e56
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892337"
---
# <a name="contenttypeinfo-resource-type"></a><span data-ttu-id="0fbc8-102">ContentTypeInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0fbc8-102">ContentTypeInfo resource type</span></span>

> <span data-ttu-id="0fbc8-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0fbc8-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0fbc8-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0fbc8-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0fbc8-105">Die **ContentTypeInfo**-Ressource gibt den SharePoint-Inhaltstyp eines Elements an.</span><span class="sxs-lookup"><span data-stu-id="0fbc8-105">The **contentTypeInfo** resource indicates the SharePoint content type of an item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0fbc8-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0fbc8-106">JSON representation</span></span>

<span data-ttu-id="0fbc8-107">Es folgt eine JSON-Darstellung einer **contentTypeInfo**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="0fbc8-107">Here is a JSON representation of a **contentTypeInfo** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="0fbc8-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0fbc8-108">Properties</span></span>

| <span data-ttu-id="0fbc8-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="0fbc8-109">Property name</span></span>  | <span data-ttu-id="0fbc8-110">Typ</span><span class="sxs-lookup"><span data-stu-id="0fbc8-110">Type</span></span>    | <span data-ttu-id="0fbc8-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0fbc8-111">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="0fbc8-112">**id**</span><span class="sxs-lookup"><span data-stu-id="0fbc8-112">**id**</span></span>         | <span data-ttu-id="0fbc8-113">string</span><span class="sxs-lookup"><span data-stu-id="0fbc8-113">string</span></span>  | <span data-ttu-id="0fbc8-114">Die ID des Inhaltstyps.</span><span class="sxs-lookup"><span data-stu-id="0fbc8-114">The id of the content type.</span></span>
| <span data-ttu-id="0fbc8-115">**name**</span><span class="sxs-lookup"><span data-stu-id="0fbc8-115">**name**</span></span>       | <span data-ttu-id="0fbc8-116">string</span><span class="sxs-lookup"><span data-stu-id="0fbc8-116">string</span></span>  | <span data-ttu-id="0fbc8-117">Der Name des Inhaltstyps.</span><span class="sxs-lookup"><span data-stu-id="0fbc8-117">The name of the content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo"
} -->
