---
title: androidMobileAppIdentifier-Ressourcentyp
description: Der Bezeichner für eine Android-App.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6c26c41ffcb36ee325f5e0fae907916a418fb8b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410280"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="a28e3-103">androidMobileAppIdentifier-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a28e3-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="a28e3-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="a28e3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a28e3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a28e3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a28e3-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a28e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a28e3-107">Der Bezeichner für eine Android-App.</span><span class="sxs-lookup"><span data-stu-id="a28e3-107">The identifier for an Android app.</span></span>


<span data-ttu-id="a28e3-108">Erbt von [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="a28e3-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a28e3-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a28e3-109">Properties</span></span>
|<span data-ttu-id="a28e3-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a28e3-110">Property</span></span>|<span data-ttu-id="a28e3-111">Typ</span><span class="sxs-lookup"><span data-stu-id="a28e3-111">Type</span></span>|<span data-ttu-id="a28e3-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a28e3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a28e3-113">packageId</span><span class="sxs-lookup"><span data-stu-id="a28e3-113">packageId</span></span>|<span data-ttu-id="a28e3-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a28e3-114">String</span></span>|<span data-ttu-id="a28e3-115">Der Bezeichner für eine App wie im Play Store definiert.</span><span class="sxs-lookup"><span data-stu-id="a28e3-115">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a28e3-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a28e3-116">Relationships</span></span>
<span data-ttu-id="a28e3-117">Keine</span><span class="sxs-lookup"><span data-stu-id="a28e3-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a28e3-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a28e3-118">JSON Representation</span></span>
<span data-ttu-id="a28e3-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a28e3-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMobileAppIdentifier",
  "packageId": "String"
}
```




