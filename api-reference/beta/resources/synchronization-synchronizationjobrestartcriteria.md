---
title: Ressourcentyp synchronizationJobRestartCriteria
description: 'Definiert den Bereich, der die [SynchronizationJob: Neustart](../api/synchronization_synchronizationjob_restart.md) Aktion.'
localization_priority: Normal
ms.openlocfilehash: 960bfa56d0bb6921ca971722d894d1b837bfab49
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572304"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="f7b62-103">Ressourcentyp synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="f7b62-103">synchronizationJobRestartCriteria resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7b62-104">Definiert den Bereich, der die [SynchronizationJob: Neustart](../api/synchronization-synchronizationjob-restart.md) Aktion.</span><span class="sxs-lookup"><span data-stu-id="f7b62-104">Defines the scope of the [synchronizationJob: restart](../api/synchronization-synchronizationjob-restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="f7b62-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f7b62-105">Properties</span></span>
| <span data-ttu-id="f7b62-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f7b62-106">Property</span></span>     | <span data-ttu-id="f7b62-107">Typ</span><span class="sxs-lookup"><span data-stu-id="f7b62-107">Type</span></span>   |<span data-ttu-id="f7b62-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7b62-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7b62-109">resetScope</span><span class="sxs-lookup"><span data-stu-id="f7b62-109">resetScope</span></span>|<span data-ttu-id="f7b62-110">String</span><span class="sxs-lookup"><span data-stu-id="f7b62-110">String</span></span>| <span data-ttu-id="f7b62-111">Durch Trennzeichen getrennte Kombination der folgenden Werte: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span><span class="sxs-lookup"><span data-stu-id="f7b62-111">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="f7b62-112">Verwendung `Full` Wenn Sie alle Optionen möchten.</span><span class="sxs-lookup"><span data-stu-id="f7b62-112">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f7b62-113">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f7b62-113">JSON representation</span></span>

<span data-ttu-id="f7b62-114">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f7b62-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJobRestartCriteria"
}-->

```json
{
  "resetScope": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJobRestartCriteria resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationjobrestartcriteria.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
