---
title: win32LobAppInstallExperience-Ressourcentyp
description: Enthält Eigenschaften der Installationsumgebung für eine Win32-App
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 01402384c2628e1f53a854fa35097415181aaa20
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174947"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="c9ac5-103">win32LobAppInstallExperience-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c9ac5-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="c9ac5-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c9ac5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9ac5-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c9ac5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9ac5-106">Enthält Eigenschaften der Installationsumgebung für eine Win32-App</span><span class="sxs-lookup"><span data-stu-id="c9ac5-106">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="c9ac5-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c9ac5-107">Properties</span></span>
|<span data-ttu-id="c9ac5-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c9ac5-108">Property</span></span>|<span data-ttu-id="c9ac5-109">Typ</span><span class="sxs-lookup"><span data-stu-id="c9ac5-109">Type</span></span>|<span data-ttu-id="c9ac5-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c9ac5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9ac5-111">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="c9ac5-111">runAsAccount</span></span>|[<span data-ttu-id="c9ac5-112">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="c9ac5-112">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="c9ac5-113">Gibt den Typ des Ausführungskontexts an, in dem die app ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="c9ac5-113">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="c9ac5-114">Mögliche Werte: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="c9ac5-114">Possible values are: `system`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9ac5-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c9ac5-115">Relationships</span></span>
<span data-ttu-id="c9ac5-116">Keine</span><span class="sxs-lookup"><span data-stu-id="c9ac5-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9ac5-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c9ac5-117">JSON Representation</span></span>
<span data-ttu-id="c9ac5-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c9ac5-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppInstallExperience",
  "runAsAccount": "String"
}
```




