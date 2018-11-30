---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
ms.openlocfilehash: edb8d97094b4d26dbbcc008664bf5dfee3a4ddf9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059475"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="acaec-102">ColumnLink-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="acaec-102">ColumnLink resource type</span></span>

> <span data-ttu-id="acaec-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="acaec-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="acaec-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="acaec-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="acaec-105">A **ColumnLink** eines [ContentType][] fügt die Website **ColumnDefinition** zu diesem Inhaltstyp hinzu.</span><span class="sxs-lookup"><span data-stu-id="acaec-105">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="acaec-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="acaec-107">JSON representation</span></span>

<span data-ttu-id="acaec-108">Es folgt eine JSON-Darstellung einer **columnLink**-Ressource.</span><span class="sxs-lookup"><span data-stu-id="acaec-108">Here is a JSON representation of a **columnLink** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="acaec-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="acaec-109">Properties</span></span>

| <span data-ttu-id="acaec-110">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="acaec-110">Property name</span></span> | <span data-ttu-id="acaec-111">Typ</span><span class="sxs-lookup"><span data-stu-id="acaec-111">Type</span></span>   | <span data-ttu-id="acaec-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="acaec-112">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="acaec-113">**id**</span><span class="sxs-lookup"><span data-stu-id="acaec-113">**id**</span></span>        | <span data-ttu-id="acaec-114">string</span><span class="sxs-lookup"><span data-stu-id="acaec-114">string</span></span> | <span data-ttu-id="acaec-115">Die eindeutige ID für die Spalte.</span><span class="sxs-lookup"><span data-stu-id="acaec-115">The unique identifier for the column.</span></span>
| <span data-ttu-id="acaec-116">**name**</span><span class="sxs-lookup"><span data-stu-id="acaec-116">**name**</span></span>      | <span data-ttu-id="acaec-117">string</span><span class="sxs-lookup"><span data-stu-id="acaec-117">string</span></span> | <span data-ttu-id="acaec-118">Der Name der Spalte in diesem Inhaltstyp.</span><span class="sxs-lookup"><span data-stu-id="acaec-118">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
