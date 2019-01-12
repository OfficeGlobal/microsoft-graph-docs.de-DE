---
title: Ressourcentyp win32LobAppInstallExperience
description: Enthält Eigenschaften für die Softwareinstallation Erfahrung für eine Win32-App
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9eeadf7bc97f53278ef59fe06795bc7120d5bc2c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986299"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="59c1c-103">Ressourcentyp win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="59c1c-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="59c1c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="59c1c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59c1c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="59c1c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="59c1c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="59c1c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59c1c-107">Enthält Eigenschaften für die Softwareinstallation Erfahrung für eine Win32-App</span><span class="sxs-lookup"><span data-stu-id="59c1c-107">Contains installation experience properties for a Win32 App</span></span>
## <a name="properties"></a><span data-ttu-id="59c1c-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="59c1c-108">Properties</span></span>
|<span data-ttu-id="59c1c-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="59c1c-109">Property</span></span>|<span data-ttu-id="59c1c-110">Typ</span><span class="sxs-lookup"><span data-stu-id="59c1c-110">Type</span></span>|<span data-ttu-id="59c1c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="59c1c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59c1c-112">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="59c1c-112">runAsAccount</span></span>|[<span data-ttu-id="59c1c-113">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="59c1c-113">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="59c1c-114">Gibt den Typ des Ausführungskontexts, den die app ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="59c1c-114">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="59c1c-115">Mögliche Werte: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="59c1c-115">Possible values are: `system`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59c1c-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="59c1c-116">Relationships</span></span>
<span data-ttu-id="59c1c-117">Keine</span><span class="sxs-lookup"><span data-stu-id="59c1c-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="59c1c-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="59c1c-118">JSON Representation</span></span>
<span data-ttu-id="59c1c-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="59c1c-119">Here is a JSON representation of the resource.</span></span>
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





