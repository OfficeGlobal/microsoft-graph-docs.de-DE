---
title: iosNotificationSettings-Ressourcentyp
description: Ein Element zur Beschreibung der Benachrichtigungseinstellungen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2876146e7e20ad94a7356f623a5b2e17443a18f8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172702"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="c915d-103">iosNotificationSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c915d-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="c915d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c915d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c915d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c915d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c915d-106">Ein Element zur Beschreibung der Benachrichtigungseinstellungen.</span><span class="sxs-lookup"><span data-stu-id="c915d-106">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="c915d-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c915d-107">Properties</span></span>
|<span data-ttu-id="c915d-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c915d-108">Property</span></span>|<span data-ttu-id="c915d-109">Typ</span><span class="sxs-lookup"><span data-stu-id="c915d-109">Type</span></span>|<span data-ttu-id="c915d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c915d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c915d-111">Paket-ID</span><span class="sxs-lookup"><span data-stu-id="c915d-111">bundleID</span></span>|<span data-ttu-id="c915d-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c915d-112">String</span></span>|<span data-ttu-id="c915d-113">Paket-ID der App, auf die diese Benachrichtigungseinstellungen angewandt werden.</span><span class="sxs-lookup"><span data-stu-id="c915d-113">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="c915d-114">Anwendungsname</span><span class="sxs-lookup"><span data-stu-id="c915d-114">appName</span></span>|<span data-ttu-id="c915d-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c915d-115">String</span></span>|<span data-ttu-id="c915d-116">Anwendungsname, der der Paket-ID zugeordnet werden muss.</span><span class="sxs-lookup"><span data-stu-id="c915d-116">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="c915d-117">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="c915d-117">publisher</span></span>|<span data-ttu-id="c915d-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c915d-118">String</span></span>|<span data-ttu-id="c915d-119">Herausgeber, der der Paket-ID zugeordnet werden muss.</span><span class="sxs-lookup"><span data-stu-id="c915d-119">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="c915d-120">enabled</span><span class="sxs-lookup"><span data-stu-id="c915d-120">enabled</span></span>|<span data-ttu-id="c915d-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="c915d-121">Boolean</span></span>|<span data-ttu-id="c915d-122">Gibt an, ob Benachrichtigungen für diese App zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="c915d-122">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="c915d-123">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="c915d-123">showInNotificationCenter</span></span>|<span data-ttu-id="c915d-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="c915d-124">Boolean</span></span>|<span data-ttu-id="c915d-125">Gibt an, ob Benachrichtigungen im Nachrichtencenter angezeigt werden können.</span><span class="sxs-lookup"><span data-stu-id="c915d-125">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="c915d-126">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="c915d-126">showOnLockScreen</span></span>|<span data-ttu-id="c915d-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="c915d-127">Boolean</span></span>|<span data-ttu-id="c915d-128">Gibt an, ob Benachrichtigungen auf dem Sperrbildschirm angezeigt werden können.</span><span class="sxs-lookup"><span data-stu-id="c915d-128">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="c915d-129">alertType</span><span class="sxs-lookup"><span data-stu-id="c915d-129">alertType</span></span>|[<span data-ttu-id="c915d-130">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="c915d-130">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="c915d-131">Gibt die Art der Warnung für Benachrichtigungen für diese App an.</span><span class="sxs-lookup"><span data-stu-id="c915d-131">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="c915d-132">Mögliche Werte: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="c915d-132">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="c915d-133">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="c915d-133">badgesEnabled</span></span>|<span data-ttu-id="c915d-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="c915d-134">Boolean</span></span>|<span data-ttu-id="c915d-135">Gibt an, ob Badges für diese App zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="c915d-135">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="c915d-136">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="c915d-136">soundsEnabled</span></span>|<span data-ttu-id="c915d-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c915d-137">Boolean</span></span>|<span data-ttu-id="c915d-138">Gibt an, ob Ton für diese App zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="c915d-138">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c915d-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c915d-139">Relationships</span></span>
<span data-ttu-id="c915d-140">Keine</span><span class="sxs-lookup"><span data-stu-id="c915d-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c915d-141">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c915d-141">JSON Representation</span></span>
<span data-ttu-id="c915d-142">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c915d-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNotificationSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNotificationSettings",
  "bundleID": "String",
  "appName": "String",
  "publisher": "String",
  "enabled": true,
  "showInNotificationCenter": true,
  "showOnLockScreen": true,
  "alertType": "String",
  "badgesEnabled": true,
  "soundsEnabled": true
}
```




