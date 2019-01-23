---
title: Ressourcentyp iosWebContentFilterAutoFilter
description: Stellt eine iOS Webinhaltsfilter Einstellungstyp, der ermöglicht automatische Filterfunktion iOS und zusätzliche URL-Zugriffssteuerung. Wenn keine-Eigenschaft Werte erstellt wird, wird das Gerät iOS den automatischen Filter unabhängig aktivieren.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d5be275b74e2675881b9d36b047e2017ef95adb2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401229"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="730fc-104">Ressourcentyp iosWebContentFilterAutoFilter</span><span class="sxs-lookup"><span data-stu-id="730fc-104">iosWebContentFilterAutoFilter resource type</span></span>

> <span data-ttu-id="730fc-105">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="730fc-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="730fc-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="730fc-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="730fc-107">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="730fc-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="730fc-108">Stellt eine iOS Webinhaltsfilter Einstellungstyp, der ermöglicht automatische Filterfunktion iOS und zusätzliche URL-Zugriffssteuerung.</span><span class="sxs-lookup"><span data-stu-id="730fc-108">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="730fc-109">Wenn keine-Eigenschaft Werte erstellt wird, wird das Gerät iOS den automatischen Filter unabhängig aktivieren.</span><span class="sxs-lookup"><span data-stu-id="730fc-109">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>


<span data-ttu-id="730fc-110">Erbt vom [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="730fc-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="730fc-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="730fc-111">Properties</span></span>
|<span data-ttu-id="730fc-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="730fc-112">Property</span></span>|<span data-ttu-id="730fc-113">Typ</span><span class="sxs-lookup"><span data-stu-id="730fc-113">Type</span></span>|<span data-ttu-id="730fc-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="730fc-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="730fc-115">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="730fc-115">allowedUrls</span></span>|<span data-ttu-id="730fc-116">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="730fc-116">String collection</span></span>|<span data-ttu-id="730fc-117">Zusätzliche URLs für den Zugriff zulässig</span><span class="sxs-lookup"><span data-stu-id="730fc-117">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="730fc-118">blockedUrls</span><span class="sxs-lookup"><span data-stu-id="730fc-118">blockedUrls</span></span>|<span data-ttu-id="730fc-119">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="730fc-119">String collection</span></span>|<span data-ttu-id="730fc-120">Zusätzliche URLs für den Zugriff blockiert</span><span class="sxs-lookup"><span data-stu-id="730fc-120">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="730fc-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="730fc-121">Relationships</span></span>
<span data-ttu-id="730fc-122">Keine</span><span class="sxs-lookup"><span data-stu-id="730fc-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="730fc-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="730fc-123">JSON Representation</span></span>
<span data-ttu-id="730fc-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="730fc-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterAutoFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterAutoFilter",
  "allowedUrls": [
    "String"
  ],
  "blockedUrls": [
    "String"
  ]
}
```




