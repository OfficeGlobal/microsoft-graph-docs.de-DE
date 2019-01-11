---
title: deviceOperatingSystemSummary-Ressourcentyp
description: Betriebssystemzusammenfassung für das Gerät
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0b69e8fa922df976a75a3750523da982582e073e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879506"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="81263-103">deviceOperatingSystemSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="81263-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="81263-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="81263-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81263-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="81263-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81263-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="81263-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81263-107">Betriebssystem des Geräts – Zusammenfassung.</span><span class="sxs-lookup"><span data-stu-id="81263-107">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="81263-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="81263-108">Properties</span></span>
|<span data-ttu-id="81263-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="81263-109">Property</span></span>|<span data-ttu-id="81263-110">Typ</span><span class="sxs-lookup"><span data-stu-id="81263-110">Type</span></span>|<span data-ttu-id="81263-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="81263-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81263-112">androidCount</span><span class="sxs-lookup"><span data-stu-id="81263-112">androidCount</span></span>|<span data-ttu-id="81263-113">Int32</span><span class="sxs-lookup"><span data-stu-id="81263-113">Int32</span></span>|<span data-ttu-id="81263-114">Anzahl der Android-Geräte.</span><span class="sxs-lookup"><span data-stu-id="81263-114">Number of android device count.</span></span>|
|<span data-ttu-id="81263-115">iosCount</span><span class="sxs-lookup"><span data-stu-id="81263-115">iosCount</span></span>|<span data-ttu-id="81263-116">Int32</span><span class="sxs-lookup"><span data-stu-id="81263-116">Int32</span></span>|<span data-ttu-id="81263-117">Anzahl der iOS-Geräte.</span><span class="sxs-lookup"><span data-stu-id="81263-117">Number of iOS device count.</span></span>|
|<span data-ttu-id="81263-118">macOSCount</span><span class="sxs-lookup"><span data-stu-id="81263-118">macOSCount</span></span>|<span data-ttu-id="81263-119">Int32</span><span class="sxs-lookup"><span data-stu-id="81263-119">Int32</span></span>|<span data-ttu-id="81263-120">Anzahl der Mac OS X-Geräte.</span><span class="sxs-lookup"><span data-stu-id="81263-120">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="81263-121">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="81263-121">windowsMobileCount</span></span>|<span data-ttu-id="81263-122">Int32</span><span class="sxs-lookup"><span data-stu-id="81263-122">Int32</span></span>|<span data-ttu-id="81263-123">Anzahl der Windows Mobile-Geräte.</span><span class="sxs-lookup"><span data-stu-id="81263-123">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="81263-124">windowsCount</span><span class="sxs-lookup"><span data-stu-id="81263-124">windowsCount</span></span>|<span data-ttu-id="81263-125">Int32</span><span class="sxs-lookup"><span data-stu-id="81263-125">Int32</span></span>|<span data-ttu-id="81263-126">Anzahl der Windows-Geräte.</span><span class="sxs-lookup"><span data-stu-id="81263-126">Number of Windows device count.</span></span>|
|<span data-ttu-id="81263-127">unknownCount</span><span class="sxs-lookup"><span data-stu-id="81263-127">unknownCount</span></span>|<span data-ttu-id="81263-128">Int32</span><span class="sxs-lookup"><span data-stu-id="81263-128">Int32</span></span>|<span data-ttu-id="81263-129">Anzahl von unbekannten Geräten.</span><span class="sxs-lookup"><span data-stu-id="81263-129">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81263-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="81263-130">Relationships</span></span>
<span data-ttu-id="81263-131">Keine</span><span class="sxs-lookup"><span data-stu-id="81263-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="81263-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="81263-132">JSON Representation</span></span>
<span data-ttu-id="81263-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="81263-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCount": 1024,
  "iosCount": 1024,
  "macOSCount": 1024,
  "windowsMobileCount": 1024,
  "windowsCount": 1024,
  "unknownCount": 1024
}
```





