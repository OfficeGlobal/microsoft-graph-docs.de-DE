---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentTypeInfo
ms.openlocfilehash: 922f87c77280627efb956e4558e1ff269daa9311
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062457"
---
# <a name="contenttypeinfo-resource-type"></a><span data-ttu-id="f6e5e-102">ContentTypeInfo-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f6e5e-102">ContentTypeInfo resource type</span></span>

> <span data-ttu-id="f6e5e-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f6e5e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f6e5e-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f6e5e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f6e5e-105">Die **ContentTypeInfo**-Ressource gibt den SharePoint-Inhaltstyp eines Elements an.</span><span class="sxs-lookup"><span data-stu-id="f6e5e-105">The **contentTypeInfo** resource indicates the SharePoint content type of an item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6e5e-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f6e5e-106">JSON representation</span></span>

<span data-ttu-id="f6e5e-107">Es folgt eine JSON-Darstellung einer **contentTypeInfo**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="f6e5e-107">Here is a JSON representation of a **contentTypeInfo** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="f6e5e-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f6e5e-108">Properties</span></span>

| <span data-ttu-id="f6e5e-109">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="f6e5e-109">Property name</span></span>  | <span data-ttu-id="f6e5e-110">Typ</span><span class="sxs-lookup"><span data-stu-id="f6e5e-110">Type</span></span>    | <span data-ttu-id="f6e5e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6e5e-111">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="f6e5e-112">**id**</span><span class="sxs-lookup"><span data-stu-id="f6e5e-112">**id**</span></span>         | <span data-ttu-id="f6e5e-113">string</span><span class="sxs-lookup"><span data-stu-id="f6e5e-113">string</span></span>  | <span data-ttu-id="f6e5e-114">Die ID des Inhaltstyps.</span><span class="sxs-lookup"><span data-stu-id="f6e5e-114">The id of the content type.</span></span>
| <span data-ttu-id="f6e5e-115">**name**</span><span class="sxs-lookup"><span data-stu-id="f6e5e-115">**name**</span></span>       | <span data-ttu-id="f6e5e-116">string</span><span class="sxs-lookup"><span data-stu-id="f6e5e-116">string</span></span>  | <span data-ttu-id="f6e5e-117">Der Name des Inhaltstyps.</span><span class="sxs-lookup"><span data-stu-id="f6e5e-117">The name of the content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo"
} -->
