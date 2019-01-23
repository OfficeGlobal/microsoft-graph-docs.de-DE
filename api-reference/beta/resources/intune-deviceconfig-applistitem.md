---
title: appListItem-Ressourcentyp
description: Stellt eine App in der Liste der verwalteten Anwendungen dar.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9571b622fc098f384f7c3a6c62b1d1e10d89f663
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405415"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="b4d9b-103">appListItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b4d9b-103">appListItem resource type</span></span>

> <span data-ttu-id="b4d9b-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="b4d9b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b4d9b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b4d9b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4d9b-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b4d9b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4d9b-107">Stellt eine App in der Liste der verwalteten Anwendungen dar.</span><span class="sxs-lookup"><span data-stu-id="b4d9b-107">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="b4d9b-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b4d9b-108">Properties</span></span>
|<span data-ttu-id="b4d9b-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b4d9b-109">Property</span></span>|<span data-ttu-id="b4d9b-110">Typ</span><span class="sxs-lookup"><span data-stu-id="b4d9b-110">Type</span></span>|<span data-ttu-id="b4d9b-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4d9b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4d9b-112">name</span><span class="sxs-lookup"><span data-stu-id="b4d9b-112">name</span></span>|<span data-ttu-id="b4d9b-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4d9b-113">String</span></span>|<span data-ttu-id="b4d9b-114">Anwendungsname</span><span class="sxs-lookup"><span data-stu-id="b4d9b-114">The application name</span></span>|
|<span data-ttu-id="b4d9b-115">publisher</span><span class="sxs-lookup"><span data-stu-id="b4d9b-115">publisher</span></span>|<span data-ttu-id="b4d9b-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4d9b-116">String</span></span>|<span data-ttu-id="b4d9b-117">Herausgeber der App</span><span class="sxs-lookup"><span data-stu-id="b4d9b-117">The publisher of the application</span></span>|
|<span data-ttu-id="b4d9b-118">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b4d9b-118">appStoreUrl</span></span>|<span data-ttu-id="b4d9b-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4d9b-119">String</span></span>|<span data-ttu-id="b4d9b-120">Store-URL der Anwendung</span><span class="sxs-lookup"><span data-stu-id="b4d9b-120">The Store URL of the application</span></span>|
|<span data-ttu-id="b4d9b-121">appId</span><span class="sxs-lookup"><span data-stu-id="b4d9b-121">appId</span></span>|<span data-ttu-id="b4d9b-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4d9b-122">String</span></span>|<span data-ttu-id="b4d9b-123">Anwendungs- oder Paket-ID der Anwendung</span><span class="sxs-lookup"><span data-stu-id="b4d9b-123">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4d9b-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b4d9b-124">Relationships</span></span>
<span data-ttu-id="b4d9b-125">Keine</span><span class="sxs-lookup"><span data-stu-id="b4d9b-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4d9b-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b4d9b-126">JSON Representation</span></span>
<span data-ttu-id="b4d9b-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b4d9b-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```




