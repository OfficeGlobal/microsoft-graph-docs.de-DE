---
title: Ressourcentyp macOSLobChildApp
description: Enthält Eigenschaften, die die Mac OS LOB-App in einem Paket bundle
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a6a8cafc0f9b47f40fe7e922130a41d37a427e5e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403021"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="2cb63-103">Ressourcentyp macOSLobChildApp</span><span class="sxs-lookup"><span data-stu-id="2cb63-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="2cb63-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="2cb63-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2cb63-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2cb63-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2cb63-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2cb63-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cb63-107">Enthält Eigenschaften, die die Mac OS LOB-App in einem Paket bundle</span><span class="sxs-lookup"><span data-stu-id="2cb63-107">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="2cb63-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2cb63-108">Properties</span></span>
|<span data-ttu-id="2cb63-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2cb63-109">Property</span></span>|<span data-ttu-id="2cb63-110">Typ</span><span class="sxs-lookup"><span data-stu-id="2cb63-110">Type</span></span>|<span data-ttu-id="2cb63-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2cb63-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cb63-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="2cb63-112">bundleId</span></span>|<span data-ttu-id="2cb63-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2cb63-113">String</span></span>|<span data-ttu-id="2cb63-114">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="2cb63-114">The Identity Name.</span></span>|
|<span data-ttu-id="2cb63-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="2cb63-115">buildNumber</span></span>|<span data-ttu-id="2cb63-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2cb63-116">String</span></span>|<span data-ttu-id="2cb63-117">Die Buildnummer der Mac OS-Zeile des Business (LoB) app.</span><span class="sxs-lookup"><span data-stu-id="2cb63-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="2cb63-118">versionNumber</span><span class="sxs-lookup"><span data-stu-id="2cb63-118">versionNumber</span></span>|<span data-ttu-id="2cb63-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2cb63-119">String</span></span>|<span data-ttu-id="2cb63-120">Die Versionsnummer der Mac OS-Zeile des Business (LoB) app.</span><span class="sxs-lookup"><span data-stu-id="2cb63-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2cb63-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2cb63-121">Relationships</span></span>
<span data-ttu-id="2cb63-122">Keine</span><span class="sxs-lookup"><span data-stu-id="2cb63-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2cb63-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2cb63-123">JSON Representation</span></span>
<span data-ttu-id="2cb63-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2cb63-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLobChildApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobChildApp",
  "bundleId": "String",
  "buildNumber": "String",
  "versionNumber": "String"
}
```




