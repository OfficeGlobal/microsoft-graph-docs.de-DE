---
title: keyValuePair-Ressourcentyp
description: Schlüssel-Wert-Paar zum Speichern benutzerdefinierter Einstellungen
ms.openlocfilehash: ac43ddbd18e99983bf4d06e9ceb97445b9d4bf57
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064902"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="ea041-103">keyValuePair-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ea041-103">keyValuePair resource type</span></span>

> <span data-ttu-id="ea041-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ea041-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea041-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ea041-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea041-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ea041-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea041-107">Schlüssel-Wert-Paar zum Speichern benutzerdefinierter Einstellungen</span><span class="sxs-lookup"><span data-stu-id="ea041-107">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="ea041-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ea041-108">Properties</span></span>
|<span data-ttu-id="ea041-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ea041-109">Property</span></span>|<span data-ttu-id="ea041-110">Typ</span><span class="sxs-lookup"><span data-stu-id="ea041-110">Type</span></span>|<span data-ttu-id="ea041-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ea041-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea041-112">name</span><span class="sxs-lookup"><span data-stu-id="ea041-112">name</span></span>|<span data-ttu-id="ea041-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ea041-113">String</span></span>|<span data-ttu-id="ea041-114">Namen für dieses Schlüssel-Wert-Paar</span><span class="sxs-lookup"><span data-stu-id="ea041-114">Name for this key-value pair</span></span>|
|<span data-ttu-id="ea041-115">Wert</span><span class="sxs-lookup"><span data-stu-id="ea041-115">value</span></span>|<span data-ttu-id="ea041-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ea041-116">String</span></span>|<span data-ttu-id="ea041-117">Wert für dieses Schlüssel-Wert-Paar</span><span class="sxs-lookup"><span data-stu-id="ea041-117">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea041-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ea041-118">Relationships</span></span>
<span data-ttu-id="ea041-119">Keine</span><span class="sxs-lookup"><span data-stu-id="ea041-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ea041-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ea041-120">JSON Representation</span></span>
<span data-ttu-id="ea041-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ea041-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```





