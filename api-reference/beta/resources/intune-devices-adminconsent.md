---
title: Ressourcentyp adminConsent
description: Informationen zum Unternehmensadministrator Zustimmung.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c76ac169bb15792afec908f62b9740e81a4d7e5b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415880"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="2add2-103">Ressourcentyp adminConsent</span><span class="sxs-lookup"><span data-stu-id="2add2-103">adminConsent resource type</span></span>

> <span data-ttu-id="2add2-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="2add2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2add2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2add2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2add2-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2add2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2add2-107">Informationen zum Unternehmensadministrator Zustimmung.</span><span class="sxs-lookup"><span data-stu-id="2add2-107">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="2add2-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2add2-108">Properties</span></span>
|<span data-ttu-id="2add2-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2add2-109">Property</span></span>|<span data-ttu-id="2add2-110">Typ</span><span class="sxs-lookup"><span data-stu-id="2add2-110">Type</span></span>|<span data-ttu-id="2add2-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2add2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2add2-112">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="2add2-112">shareAPNSData</span></span>|[<span data-ttu-id="2add2-113">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="2add2-113">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="2add2-114">Der Administrator Zustimmung Zustand der Freigabe von Benutzer- und Gerätedaten zu Apple.</span><span class="sxs-lookup"><span data-stu-id="2add2-114">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="2add2-115">Mögliche Werte sind: `notConfigured`, `granted` und `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="2add2-115">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2add2-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2add2-116">Relationships</span></span>
<span data-ttu-id="2add2-117">Keine</span><span class="sxs-lookup"><span data-stu-id="2add2-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2add2-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2add2-118">JSON Representation</span></span>
<span data-ttu-id="2add2-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2add2-119">Here is a JSON representation of the resource.</span></span>
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




