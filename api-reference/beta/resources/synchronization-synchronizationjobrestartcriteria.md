---
title: Ressourcentyp synchronizationJobRestartCriteria
description: 'Definiert den Bereich, der die [SynchronizationJob: Neustart](../api/synchronization_synchronizationjob_restart.md) Aktion.'
ms.openlocfilehash: edf5cf258750df72dda2c9754d3543e07fc32e39
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058549"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="e3c89-103">Ressourcentyp synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="e3c89-103">synchronizationJobRestartCriteria resource type</span></span>

> <span data-ttu-id="e3c89-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e3c89-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3c89-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e3c89-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e3c89-106">Definiert den Bereich, der die [SynchronizationJob: Neustart](../api/synchronization_synchronizationjob_restart.md) Aktion.</span><span class="sxs-lookup"><span data-stu-id="e3c89-106">Defines the scope of the [synchronizationJob: restart](../api/synchronization_synchronizationjob_restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="e3c89-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e3c89-107">Properties</span></span>
| <span data-ttu-id="e3c89-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e3c89-108">Property</span></span>     | <span data-ttu-id="e3c89-109">Typ</span><span class="sxs-lookup"><span data-stu-id="e3c89-109">Type</span></span>   |<span data-ttu-id="e3c89-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3c89-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3c89-111">resetScope</span><span class="sxs-lookup"><span data-stu-id="e3c89-111">resetScope</span></span>|<span data-ttu-id="e3c89-112">String</span><span class="sxs-lookup"><span data-stu-id="e3c89-112">String</span></span>| <span data-ttu-id="e3c89-113">Durch Trennzeichen getrennte Kombination der folgenden Werte: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span><span class="sxs-lookup"><span data-stu-id="e3c89-113">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="e3c89-114">Verwendung `Full` Wenn Sie alle Optionen möchten.</span><span class="sxs-lookup"><span data-stu-id="e3c89-114">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e3c89-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e3c89-115">JSON representation</span></span>

<span data-ttu-id="e3c89-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e3c89-116">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJobRestartCriteria resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->