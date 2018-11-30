---
title: Ressourcentyp resourceReference
description: Komplexer Typ mit Eigenschaften des Insights.
ms.openlocfilehash: d171151a1c3547aa6863a7f70cc3a42ddec13e5d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062948"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="9fb7c-103">Ressourcentyp resourceReference</span><span class="sxs-lookup"><span data-stu-id="9fb7c-103">resourceReference resource type</span></span>

> <span data-ttu-id="9fb7c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9fb7c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9fb7c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9fb7c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9fb7c-106">Komplexer Typ mit Eigenschaften des [Insights](insights.md).</span><span class="sxs-lookup"><span data-stu-id="9fb7c-106">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fb7c-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9fb7c-107">JSON representation</span></span>

<span data-ttu-id="9fb7c-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9fb7c-108">Here is a JSON representation of the resource</span></span>

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="9fb7c-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9fb7c-109">Properties</span></span>

| <span data-ttu-id="9fb7c-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9fb7c-110">Property</span></span>      | <span data-ttu-id="9fb7c-111">Typ</span><span class="sxs-lookup"><span data-stu-id="9fb7c-111">Type</span></span>      | <span data-ttu-id="9fb7c-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9fb7c-112">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="9fb7c-113">webUrl</span><span class="sxs-lookup"><span data-stu-id="9fb7c-113">webUrl</span></span>        | <span data-ttu-id="9fb7c-114">String</span><span class="sxs-lookup"><span data-stu-id="9fb7c-114">String</span></span>    | <span data-ttu-id="9fb7c-115">Eine URL, die auf das verwiesene Element führende.</span><span class="sxs-lookup"><span data-stu-id="9fb7c-115">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="9fb7c-116">id</span><span class="sxs-lookup"><span data-stu-id="9fb7c-116">id</span></span>            | <span data-ttu-id="9fb7c-117">String</span><span class="sxs-lookup"><span data-stu-id="9fb7c-117">String</span></span>    | <span data-ttu-id="9fb7c-118">Eindeutiger Bezeichner des Elements.</span><span class="sxs-lookup"><span data-stu-id="9fb7c-118">The item's unique identifier.</span></span>           |
| <span data-ttu-id="9fb7c-119">Typ</span><span class="sxs-lookup"><span data-stu-id="9fb7c-119">type</span></span>          | <span data-ttu-id="9fb7c-120">String</span><span class="sxs-lookup"><span data-stu-id="9fb7c-120">String</span></span>    | <span data-ttu-id="9fb7c-121">Ein String-Wert, der verwendet werden kann, um das Element, wie beispielsweise "microsoft.graph.driveItem" klassifizieren</span><span class="sxs-lookup"><span data-stu-id="9fb7c-121">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |