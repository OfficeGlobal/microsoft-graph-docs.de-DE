---
title: Ressourcentyp win32LobAppInstallExperience
description: Enthält Eigenschaften für die Softwareinstallation Erfahrung für eine Win32-App
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 74e7dd5b036d42d85e49935f454f3050f604827b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866906"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="9d8b6-103">Ressourcentyp win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="9d8b6-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="9d8b6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9d8b6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d8b6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9d8b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9d8b6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9d8b6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d8b6-107">Enthält Eigenschaften für die Softwareinstallation Erfahrung für eine Win32-App</span><span class="sxs-lookup"><span data-stu-id="9d8b6-107">Contains installation experience properties for a Win32 App</span></span>
## <a name="properties"></a><span data-ttu-id="9d8b6-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9d8b6-108">Properties</span></span>
|<span data-ttu-id="9d8b6-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9d8b6-109">Property</span></span>|<span data-ttu-id="9d8b6-110">Typ</span><span class="sxs-lookup"><span data-stu-id="9d8b6-110">Type</span></span>|<span data-ttu-id="9d8b6-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9d8b6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d8b6-112">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="9d8b6-112">runAsAccount</span></span>|[<span data-ttu-id="9d8b6-113">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="9d8b6-113">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="9d8b6-114">Gibt den Typ des Ausführungskontexts, den die app ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9d8b6-114">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="9d8b6-115">Mögliche Werte: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="9d8b6-115">Possible values are: `system`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d8b6-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9d8b6-116">Relationships</span></span>
<span data-ttu-id="9d8b6-117">Keine</span><span class="sxs-lookup"><span data-stu-id="9d8b6-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9d8b6-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9d8b6-118">JSON Representation</span></span>
<span data-ttu-id="9d8b6-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9d8b6-119">Here is a JSON representation of the resource.</span></span>
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





