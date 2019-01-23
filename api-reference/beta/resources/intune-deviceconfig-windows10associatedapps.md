---
title: Ressourcentyp windows10AssociatedApps
description: Definition der Windows-10-Anwendung verknüpft ist.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5dd5b664bde2970caa4b09c027592684b9ecd5e2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425918"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="10fea-103">Ressourcentyp windows10AssociatedApps</span><span class="sxs-lookup"><span data-stu-id="10fea-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="10fea-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="10fea-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="10fea-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="10fea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="10fea-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="10fea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10fea-107">Definition der Windows-10-Anwendung verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="10fea-107">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="10fea-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="10fea-108">Properties</span></span>
|<span data-ttu-id="10fea-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="10fea-109">Property</span></span>|<span data-ttu-id="10fea-110">Typ</span><span class="sxs-lookup"><span data-stu-id="10fea-110">Type</span></span>|<span data-ttu-id="10fea-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10fea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10fea-112">der appType</span><span class="sxs-lookup"><span data-stu-id="10fea-112">appType</span></span>|[<span data-ttu-id="10fea-113">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="10fea-113">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="10fea-114">Anwendungstyp.</span><span class="sxs-lookup"><span data-stu-id="10fea-114">Application type.</span></span> <span data-ttu-id="10fea-115">Mögliche Werte sind: `desktop` und `universal`.</span><span class="sxs-lookup"><span data-stu-id="10fea-115">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="10fea-116">Bezeichner</span><span class="sxs-lookup"><span data-stu-id="10fea-116">identifier</span></span>|<span data-ttu-id="10fea-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="10fea-117">String</span></span>|<span data-ttu-id="10fea-118">Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="10fea-118">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10fea-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="10fea-119">Relationships</span></span>
<span data-ttu-id="10fea-120">Keine</span><span class="sxs-lookup"><span data-stu-id="10fea-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10fea-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="10fea-121">JSON Representation</span></span>
<span data-ttu-id="10fea-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="10fea-122">Here is a JSON representation of the resource.</span></span>
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




