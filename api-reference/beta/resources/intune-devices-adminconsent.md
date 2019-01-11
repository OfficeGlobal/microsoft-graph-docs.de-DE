---
title: Ressourcentyp adminConsent
description: Informationen zum Unternehmensadministrator Zustimmung.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4b6b2d9a8c32c9a1ce7e8587ebe853f7646b703a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815586"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="71dd5-103">Ressourcentyp adminConsent</span><span class="sxs-lookup"><span data-stu-id="71dd5-103">adminConsent resource type</span></span>

> <span data-ttu-id="71dd5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="71dd5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71dd5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="71dd5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71dd5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="71dd5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71dd5-107">Informationen zum Unternehmensadministrator Zustimmung.</span><span class="sxs-lookup"><span data-stu-id="71dd5-107">Admin consent information.</span></span>
## <a name="properties"></a><span data-ttu-id="71dd5-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="71dd5-108">Properties</span></span>
|<span data-ttu-id="71dd5-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="71dd5-109">Property</span></span>|<span data-ttu-id="71dd5-110">Typ</span><span class="sxs-lookup"><span data-stu-id="71dd5-110">Type</span></span>|<span data-ttu-id="71dd5-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71dd5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71dd5-112">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="71dd5-112">shareAPNSData</span></span>|[<span data-ttu-id="71dd5-113">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="71dd5-113">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="71dd5-114">Der Administrator Zustimmung Zustand der Freigabe von Benutzer- und Gerätedaten zu Apple.</span><span class="sxs-lookup"><span data-stu-id="71dd5-114">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="71dd5-115">Mögliche Werte sind: `notConfigured`, `granted` und `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="71dd5-115">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71dd5-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="71dd5-116">Relationships</span></span>
<span data-ttu-id="71dd5-117">Keine</span><span class="sxs-lookup"><span data-stu-id="71dd5-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="71dd5-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="71dd5-118">JSON Representation</span></span>
<span data-ttu-id="71dd5-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="71dd5-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "String"
}
```





