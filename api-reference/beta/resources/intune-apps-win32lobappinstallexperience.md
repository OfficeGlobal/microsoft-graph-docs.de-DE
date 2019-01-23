---
title: Ressourcentyp win32LobAppInstallExperience
description: Enthält Eigenschaften für die Softwareinstallation Erfahrung für eine Win32-App
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 240000dfceaa2ef4e973167cbd3b5a743d346892
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406689"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="68277-103">Ressourcentyp win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="68277-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="68277-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="68277-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="68277-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="68277-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="68277-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="68277-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68277-107">Enthält Eigenschaften für die Softwareinstallation Erfahrung für eine Win32-App</span><span class="sxs-lookup"><span data-stu-id="68277-107">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="68277-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="68277-108">Properties</span></span>
|<span data-ttu-id="68277-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="68277-109">Property</span></span>|<span data-ttu-id="68277-110">Typ</span><span class="sxs-lookup"><span data-stu-id="68277-110">Type</span></span>|<span data-ttu-id="68277-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="68277-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68277-112">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="68277-112">runAsAccount</span></span>|[<span data-ttu-id="68277-113">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="68277-113">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="68277-114">Gibt den Typ des Ausführungskontexts, den die app ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="68277-114">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="68277-115">Mögliche Werte: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="68277-115">Possible values are: `system`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68277-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="68277-116">Relationships</span></span>
<span data-ttu-id="68277-117">Keine</span><span class="sxs-lookup"><span data-stu-id="68277-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68277-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="68277-118">JSON Representation</span></span>
<span data-ttu-id="68277-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="68277-119">Here is a JSON representation of the resource.</span></span>
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




