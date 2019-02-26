---
title: appConfigurationSettingItem-Ressourcentyp
description: Enthält die Eigenschaften für ein App-Konfigurationseinstellungselement.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 11ef3a964d166301c04c49730ac084b68e700b7c
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263819"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="7e844-103">appConfigurationSettingItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7e844-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="7e844-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7e844-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e844-105">Enthält die Eigenschaften für ein App-Konfigurationseinstellungselement.</span><span class="sxs-lookup"><span data-stu-id="7e844-105">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="7e844-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7e844-106">Properties</span></span>
|<span data-ttu-id="7e844-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7e844-107">Property</span></span>|<span data-ttu-id="7e844-108">Typ</span><span class="sxs-lookup"><span data-stu-id="7e844-108">Type</span></span>|<span data-ttu-id="7e844-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e844-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e844-110">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="7e844-110">appConfigKey</span></span>|<span data-ttu-id="7e844-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e844-111">String</span></span>|<span data-ttu-id="7e844-112">App-Konfigurationsschlüssel</span><span class="sxs-lookup"><span data-stu-id="7e844-112">app configuration key.</span></span>|
|<span data-ttu-id="7e844-113">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="7e844-113">appConfigKeyType</span></span>|[<span data-ttu-id="7e844-114">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="7e844-114">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="7e844-115">Typs des App-Konfigurationsschlüssels.</span><span class="sxs-lookup"><span data-stu-id="7e844-115">app configuration key type.</span></span> <span data-ttu-id="7e844-116">Mögliche Werte: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="7e844-116">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="7e844-117">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="7e844-117">appConfigKeyValue</span></span>|<span data-ttu-id="7e844-118">String</span><span class="sxs-lookup"><span data-stu-id="7e844-118">String</span></span>|<span data-ttu-id="7e844-119">Wert des App-Konfigurationsschlüssels</span><span class="sxs-lookup"><span data-stu-id="7e844-119">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e844-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7e844-120">Relationships</span></span>
<span data-ttu-id="7e844-121">Keine</span><span class="sxs-lookup"><span data-stu-id="7e844-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e844-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7e844-122">JSON Representation</span></span>
<span data-ttu-id="7e844-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7e844-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConfigurationSettingItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConfigurationSettingItem",
  "appConfigKey": "String",
  "appConfigKeyType": "String",
  "appConfigKeyValue": "String"
}
```



