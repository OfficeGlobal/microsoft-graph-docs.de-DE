---
title: keyValuePair-Ressourcentyp
description: Schlüssel-Wert-Paar zum Speichern benutzerdefinierter Einstellungen
author: tfitzmac
ms.openlocfilehash: f6438d97376d46f66e02026acc87c948ab2a91bb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329316"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="8e834-103">keyValuePair-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8e834-103">keyValuePair resource type</span></span>

> <span data-ttu-id="8e834-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8e834-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e834-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8e834-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8e834-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8e834-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e834-107">Schlüssel-Wert-Paar zum Speichern benutzerdefinierter Einstellungen</span><span class="sxs-lookup"><span data-stu-id="8e834-107">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="8e834-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8e834-108">Properties</span></span>
|<span data-ttu-id="8e834-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8e834-109">Property</span></span>|<span data-ttu-id="8e834-110">Typ</span><span class="sxs-lookup"><span data-stu-id="8e834-110">Type</span></span>|<span data-ttu-id="8e834-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e834-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e834-112">name</span><span class="sxs-lookup"><span data-stu-id="8e834-112">name</span></span>|<span data-ttu-id="8e834-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8e834-113">String</span></span>|<span data-ttu-id="8e834-114">Namen für dieses Schlüssel-Wert-Paar</span><span class="sxs-lookup"><span data-stu-id="8e834-114">Name for this key-value pair</span></span>|
|<span data-ttu-id="8e834-115">Wert</span><span class="sxs-lookup"><span data-stu-id="8e834-115">value</span></span>|<span data-ttu-id="8e834-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8e834-116">String</span></span>|<span data-ttu-id="8e834-117">Wert für dieses Schlüssel-Wert-Paar</span><span class="sxs-lookup"><span data-stu-id="8e834-117">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e834-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8e834-118">Relationships</span></span>
<span data-ttu-id="8e834-119">Keine</span><span class="sxs-lookup"><span data-stu-id="8e834-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8e834-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8e834-120">JSON Representation</span></span>
<span data-ttu-id="8e834-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8e834-121">Here is a JSON representation of the resource.</span></span>
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





