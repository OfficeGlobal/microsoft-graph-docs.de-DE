---
title: iosNotificationSettings-Ressourcentyp
description: Ein Element zur Beschreibung der Benachrichtigungseinstellungen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ce016579729353f69f2e7671ff67b5da0004536
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260382"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="68f9b-103">iosNotificationSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="68f9b-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="68f9b-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="68f9b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68f9b-105">Ein Element zur Beschreibung der Benachrichtigungseinstellungen.</span><span class="sxs-lookup"><span data-stu-id="68f9b-105">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="68f9b-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="68f9b-106">Properties</span></span>
|<span data-ttu-id="68f9b-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="68f9b-107">Property</span></span>|<span data-ttu-id="68f9b-108">Typ</span><span class="sxs-lookup"><span data-stu-id="68f9b-108">Type</span></span>|<span data-ttu-id="68f9b-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="68f9b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68f9b-110">Paket-ID</span><span class="sxs-lookup"><span data-stu-id="68f9b-110">bundleID</span></span>|<span data-ttu-id="68f9b-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="68f9b-111">String</span></span>|<span data-ttu-id="68f9b-112">Paket-ID der App, auf die diese Benachrichtigungseinstellungen angewandt werden.</span><span class="sxs-lookup"><span data-stu-id="68f9b-112">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="68f9b-113">Anwendungsname</span><span class="sxs-lookup"><span data-stu-id="68f9b-113">appName</span></span>|<span data-ttu-id="68f9b-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="68f9b-114">String</span></span>|<span data-ttu-id="68f9b-115">Anwendungsname, der der Paket-ID zugeordnet werden muss.</span><span class="sxs-lookup"><span data-stu-id="68f9b-115">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="68f9b-116">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="68f9b-116">publisher</span></span>|<span data-ttu-id="68f9b-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="68f9b-117">String</span></span>|<span data-ttu-id="68f9b-118">Herausgeber, der der Paket-ID zugeordnet werden muss.</span><span class="sxs-lookup"><span data-stu-id="68f9b-118">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="68f9b-119">enabled</span><span class="sxs-lookup"><span data-stu-id="68f9b-119">enabled</span></span>|<span data-ttu-id="68f9b-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="68f9b-120">Boolean</span></span>|<span data-ttu-id="68f9b-121">Gibt an, ob Benachrichtigungen für diese App zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="68f9b-121">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="68f9b-122">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="68f9b-122">showInNotificationCenter</span></span>|<span data-ttu-id="68f9b-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="68f9b-123">Boolean</span></span>|<span data-ttu-id="68f9b-124">Gibt an, ob Benachrichtigungen im Nachrichtencenter angezeigt werden können.</span><span class="sxs-lookup"><span data-stu-id="68f9b-124">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="68f9b-125">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="68f9b-125">showOnLockScreen</span></span>|<span data-ttu-id="68f9b-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="68f9b-126">Boolean</span></span>|<span data-ttu-id="68f9b-127">Gibt an, ob Benachrichtigungen auf dem Sperrbildschirm angezeigt werden können.</span><span class="sxs-lookup"><span data-stu-id="68f9b-127">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="68f9b-128">alertType</span><span class="sxs-lookup"><span data-stu-id="68f9b-128">alertType</span></span>|[<span data-ttu-id="68f9b-129">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="68f9b-129">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="68f9b-130">Gibt die Art der Warnung für Benachrichtigungen für diese App an.</span><span class="sxs-lookup"><span data-stu-id="68f9b-130">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="68f9b-131">Mögliche Werte: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="68f9b-131">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="68f9b-132">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="68f9b-132">badgesEnabled</span></span>|<span data-ttu-id="68f9b-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="68f9b-133">Boolean</span></span>|<span data-ttu-id="68f9b-134">Gibt an, ob Badges für diese App zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="68f9b-134">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="68f9b-135">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="68f9b-135">soundsEnabled</span></span>|<span data-ttu-id="68f9b-136">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="68f9b-136">Boolean</span></span>|<span data-ttu-id="68f9b-137">Gibt an, ob Ton für diese App zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="68f9b-137">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68f9b-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="68f9b-138">Relationships</span></span>
<span data-ttu-id="68f9b-139">Keine</span><span class="sxs-lookup"><span data-stu-id="68f9b-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68f9b-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="68f9b-140">JSON Representation</span></span>
<span data-ttu-id="68f9b-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="68f9b-141">Here is a JSON representation of the resource.</span></span>
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



