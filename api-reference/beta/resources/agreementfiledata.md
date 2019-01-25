---
title: Ressourcentyp agreementFileData
description: Stellt den Blob eines Azure Active Directory (Azure AD) Begriffe der Vereinbarung-Datei verwenden.
localization_priority: Normal
ms.openlocfilehash: bc0e7395875f64a3ee52e43b26da1a2df6276c9c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517029"
---
# <a name="agreementfiledata-resource-type"></a><span data-ttu-id="fd8e1-103">Ressourcentyp agreementFileData</span><span class="sxs-lookup"><span data-stu-id="fd8e1-103">agreementFileData resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd8e1-104">Stellt den Blob eines Azure Active Directory (Azure AD) Begriffe der Vereinbarung-Datei verwenden.</span><span class="sxs-lookup"><span data-stu-id="fd8e1-104">Represents the blob of an Azure Active Directory (Azure AD) terms of use agreement file.</span></span>

## <a name="properties"></a><span data-ttu-id="fd8e1-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fd8e1-105">Properties</span></span>
| <span data-ttu-id="fd8e1-106">Methode</span><span class="sxs-lookup"><span data-stu-id="fd8e1-106">Method</span></span>       | <span data-ttu-id="fd8e1-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="fd8e1-107">Return Type</span></span> | <span data-ttu-id="fd8e1-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd8e1-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fd8e1-109">data</span><span class="sxs-lookup"><span data-stu-id="fd8e1-109">data</span></span>|<span data-ttu-id="fd8e1-110">Binär</span><span class="sxs-lookup"><span data-stu-id="fd8e1-110">Binary</span></span>|<span data-ttu-id="fd8e1-111">Daten, die die Begriffe verwenden PDF-Dokument darstellt.</span><span class="sxs-lookup"><span data-stu-id="fd8e1-111">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="fd8e1-112">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="fd8e1-112">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fd8e1-113">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fd8e1-113">JSON representation</span></span>

<span data-ttu-id="fd8e1-114">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fd8e1-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileData"
}-->

```json
{
  "data": "Binary"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFileData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/agreementfiledata.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
