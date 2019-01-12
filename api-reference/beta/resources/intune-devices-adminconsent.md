---
title: Ressourcentyp adminConsent
description: Informationen zum Unternehmensadministrator Zustimmung.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 428729ff9a8a8ee5deb64c537922cb7a0417ba2e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962128"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="2e2e4-103">Ressourcentyp adminConsent</span><span class="sxs-lookup"><span data-stu-id="2e2e4-103">adminConsent resource type</span></span>

> <span data-ttu-id="2e2e4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2e2e4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2e2e4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2e2e4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2e2e4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2e2e4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e2e4-107">Informationen zum Unternehmensadministrator Zustimmung.</span><span class="sxs-lookup"><span data-stu-id="2e2e4-107">Admin consent information.</span></span>
## <a name="properties"></a><span data-ttu-id="2e2e4-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2e2e4-108">Properties</span></span>
|<span data-ttu-id="2e2e4-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2e2e4-109">Property</span></span>|<span data-ttu-id="2e2e4-110">Typ</span><span class="sxs-lookup"><span data-stu-id="2e2e4-110">Type</span></span>|<span data-ttu-id="2e2e4-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e2e4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e2e4-112">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="2e2e4-112">shareAPNSData</span></span>|[<span data-ttu-id="2e2e4-113">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="2e2e4-113">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="2e2e4-114">Der Administrator Zustimmung Zustand der Freigabe von Benutzer- und Gerätedaten zu Apple.</span><span class="sxs-lookup"><span data-stu-id="2e2e4-114">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="2e2e4-115">Mögliche Werte sind: `notConfigured`, `granted` und `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="2e2e4-115">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e2e4-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2e2e4-116">Relationships</span></span>
<span data-ttu-id="2e2e4-117">Keine</span><span class="sxs-lookup"><span data-stu-id="2e2e4-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2e2e4-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2e2e4-118">JSON Representation</span></span>
<span data-ttu-id="2e2e4-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2e2e4-119">Here is a JSON representation of the resource.</span></span>
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





