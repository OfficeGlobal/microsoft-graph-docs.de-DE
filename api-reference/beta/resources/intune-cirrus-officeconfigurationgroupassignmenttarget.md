---
title: Ressourcentyp officeConfigurationGroupAssignmentTarget
description: Office-Client-Konfiguration AAD Zuordnung Ziel gruppieren
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 411af117999498050288405874bd6b5baff5b6b5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422747"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="733a0-103">Ressourcentyp officeConfigurationGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="733a0-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="733a0-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="733a0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="733a0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="733a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="733a0-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="733a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="733a0-107">Office-Client-Konfiguration AAD Zuordnung Ziel gruppieren</span><span class="sxs-lookup"><span data-stu-id="733a0-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="733a0-108">Erbt vom [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="733a0-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="733a0-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="733a0-109">Properties</span></span>
|<span data-ttu-id="733a0-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="733a0-110">Property</span></span>|<span data-ttu-id="733a0-111">Typ</span><span class="sxs-lookup"><span data-stu-id="733a0-111">Type</span></span>|<span data-ttu-id="733a0-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="733a0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="733a0-113">groupId</span><span class="sxs-lookup"><span data-stu-id="733a0-113">groupId</span></span>|<span data-ttu-id="733a0-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="733a0-114">String</span></span>|<span data-ttu-id="733a0-115">Die Id der Gruppe AAD sind wir Gerätekonfiguration zu adressieren.</span><span class="sxs-lookup"><span data-stu-id="733a0-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="733a0-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="733a0-116">Relationships</span></span>
<span data-ttu-id="733a0-117">Keine</span><span class="sxs-lookup"><span data-stu-id="733a0-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="733a0-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="733a0-118">JSON Representation</span></span>
<span data-ttu-id="733a0-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="733a0-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfigurationGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfigurationGroupAssignmentTarget",
  "groupId": "String"
}
```



