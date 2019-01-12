---
title: Ressourcentyp windows10AssociatedApps
description: Definition der Windows-10-Anwendung verknüpft ist.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d1f6363027ae46263146efdbf3f5ac5254afcd93
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911910"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="df942-103">Ressourcentyp windows10AssociatedApps</span><span class="sxs-lookup"><span data-stu-id="df942-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="df942-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="df942-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df942-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="df942-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df942-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="df942-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df942-107">Definition der Windows-10-Anwendung verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="df942-107">Windows 10 Associated Application definition.</span></span>
## <a name="properties"></a><span data-ttu-id="df942-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="df942-108">Properties</span></span>
|<span data-ttu-id="df942-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="df942-109">Property</span></span>|<span data-ttu-id="df942-110">Typ</span><span class="sxs-lookup"><span data-stu-id="df942-110">Type</span></span>|<span data-ttu-id="df942-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df942-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df942-112">der appType</span><span class="sxs-lookup"><span data-stu-id="df942-112">appType</span></span>|[<span data-ttu-id="df942-113">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="df942-113">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="df942-114">Anwendungstyp.</span><span class="sxs-lookup"><span data-stu-id="df942-114">Application type.</span></span> <span data-ttu-id="df942-115">Mögliche Werte sind: `desktop` und `universal`.</span><span class="sxs-lookup"><span data-stu-id="df942-115">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="df942-116">Bezeichner</span><span class="sxs-lookup"><span data-stu-id="df942-116">identifier</span></span>|<span data-ttu-id="df942-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="df942-117">String</span></span>|<span data-ttu-id="df942-118">Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="df942-118">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df942-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="df942-119">Relationships</span></span>
<span data-ttu-id="df942-120">Keine</span><span class="sxs-lookup"><span data-stu-id="df942-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="df942-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="df942-121">JSON Representation</span></span>
<span data-ttu-id="df942-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="df942-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AssociatedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AssociatedApps",
  "appType": "String",
  "identifier": "String"
}
```





