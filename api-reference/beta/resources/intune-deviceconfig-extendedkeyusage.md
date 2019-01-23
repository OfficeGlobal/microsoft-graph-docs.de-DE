---
title: Ressourcentyp extendedKeyUsage
description: Benutzerdefinierte erweiterte Schlüsselverwendung definition
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6ed825f44923d3fe86cc410397747b50a1f2c681
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425967"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="2ec8f-103">Ressourcentyp extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="2ec8f-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="2ec8f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="2ec8f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2ec8f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2ec8f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2ec8f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2ec8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ec8f-107">Benutzerdefinierte erweiterte Schlüsselverwendung definition</span><span class="sxs-lookup"><span data-stu-id="2ec8f-107">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="2ec8f-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2ec8f-108">Properties</span></span>
|<span data-ttu-id="2ec8f-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2ec8f-109">Property</span></span>|<span data-ttu-id="2ec8f-110">Typ</span><span class="sxs-lookup"><span data-stu-id="2ec8f-110">Type</span></span>|<span data-ttu-id="2ec8f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2ec8f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ec8f-112">name</span><span class="sxs-lookup"><span data-stu-id="2ec8f-112">name</span></span>|<span data-ttu-id="2ec8f-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2ec8f-113">String</span></span>|<span data-ttu-id="2ec8f-114">Erweiterte Schlüsselverwendung Name</span><span class="sxs-lookup"><span data-stu-id="2ec8f-114">Extended Key Usage Name</span></span>|
|<span data-ttu-id="2ec8f-115">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="2ec8f-115">objectIdentifier</span></span>|<span data-ttu-id="2ec8f-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2ec8f-116">String</span></span>|<span data-ttu-id="2ec8f-117">Erweiterte Schlüsselverwendung Objektbezeichner</span><span class="sxs-lookup"><span data-stu-id="2ec8f-117">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ec8f-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2ec8f-118">Relationships</span></span>
<span data-ttu-id="2ec8f-119">Keine</span><span class="sxs-lookup"><span data-stu-id="2ec8f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ec8f-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2ec8f-120">JSON Representation</span></span>
<span data-ttu-id="2ec8f-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2ec8f-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extendedKeyUsage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extendedKeyUsage",
  "name": "String",
  "objectIdentifier": "String"
}
```




