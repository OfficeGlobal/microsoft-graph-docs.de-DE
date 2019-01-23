---
title: Ressourcentyp managedDeviceModelsAndManufacturers
description: Modelle und Hersteller Meatadata für verwaltete Geräte im Konto
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: afcf64cb0e8db4e24ce061490ecc593595690930
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396791"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="06863-103">Ressourcentyp managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="06863-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="06863-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="06863-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="06863-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="06863-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06863-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="06863-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06863-107">Modelle und Hersteller Meatadata für verwaltete Geräte im Konto</span><span class="sxs-lookup"><span data-stu-id="06863-107">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="06863-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="06863-108">Properties</span></span>
|<span data-ttu-id="06863-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="06863-109">Property</span></span>|<span data-ttu-id="06863-110">Typ</span><span class="sxs-lookup"><span data-stu-id="06863-110">Type</span></span>|<span data-ttu-id="06863-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06863-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06863-112">deviceModels</span><span class="sxs-lookup"><span data-stu-id="06863-112">deviceModels</span></span>|<span data-ttu-id="06863-113">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="06863-113">String collection</span></span>|<span data-ttu-id="06863-114">Liste der Modelle für verwaltete Geräte im Konto</span><span class="sxs-lookup"><span data-stu-id="06863-114">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="06863-115">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="06863-115">deviceManufacturers</span></span>|<span data-ttu-id="06863-116">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="06863-116">String collection</span></span>|<span data-ttu-id="06863-117">Liste der Hersteller für verwalteten Geräten im Konto</span><span class="sxs-lookup"><span data-stu-id="06863-117">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="06863-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="06863-118">Relationships</span></span>
<span data-ttu-id="06863-119">Keine</span><span class="sxs-lookup"><span data-stu-id="06863-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06863-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="06863-120">JSON Representation</span></span>
<span data-ttu-id="06863-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="06863-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceModelsAndManufacturers",
  "deviceModels": [
    "String"
  ],
  "deviceManufacturers": [
    "String"
  ]
}
```




