---
title: iosNotificationSettings-Ressourcentyp
description: Ein Element zur Beschreibung der Benachrichtigungseinstellungen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7db0b6ba438522db0795f6897daba8b5c43258c5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420500"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="b5db5-103">iosNotificationSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b5db5-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="b5db5-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="b5db5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b5db5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b5db5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5db5-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b5db5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5db5-107">Ein Element zur Beschreibung der Benachrichtigungseinstellungen.</span><span class="sxs-lookup"><span data-stu-id="b5db5-107">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="b5db5-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b5db5-108">Properties</span></span>
|<span data-ttu-id="b5db5-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b5db5-109">Property</span></span>|<span data-ttu-id="b5db5-110">Typ</span><span class="sxs-lookup"><span data-stu-id="b5db5-110">Type</span></span>|<span data-ttu-id="b5db5-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b5db5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5db5-112">Paket-ID</span><span class="sxs-lookup"><span data-stu-id="b5db5-112">bundleID</span></span>|<span data-ttu-id="b5db5-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b5db5-113">String</span></span>|<span data-ttu-id="b5db5-114">Paket-ID der App, auf die diese Benachrichtigungseinstellungen angewandt werden.</span><span class="sxs-lookup"><span data-stu-id="b5db5-114">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="b5db5-115">Anwendungsname</span><span class="sxs-lookup"><span data-stu-id="b5db5-115">appName</span></span>|<span data-ttu-id="b5db5-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b5db5-116">String</span></span>|<span data-ttu-id="b5db5-117">Anwendungsname, der der Paket-ID zugeordnet werden muss.</span><span class="sxs-lookup"><span data-stu-id="b5db5-117">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="b5db5-118">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="b5db5-118">publisher</span></span>|<span data-ttu-id="b5db5-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b5db5-119">String</span></span>|<span data-ttu-id="b5db5-120">Herausgeber, der der Paket-ID zugeordnet werden muss.</span><span class="sxs-lookup"><span data-stu-id="b5db5-120">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="b5db5-121">enabled</span><span class="sxs-lookup"><span data-stu-id="b5db5-121">enabled</span></span>|<span data-ttu-id="b5db5-122">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b5db5-122">Boolean</span></span>|<span data-ttu-id="b5db5-123">Gibt an, ob Benachrichtigungen für diese App zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="b5db5-123">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="b5db5-124">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="b5db5-124">showInNotificationCenter</span></span>|<span data-ttu-id="b5db5-125">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b5db5-125">Boolean</span></span>|<span data-ttu-id="b5db5-126">Gibt an, ob Benachrichtigungen im Nachrichtencenter angezeigt werden können.</span><span class="sxs-lookup"><span data-stu-id="b5db5-126">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="b5db5-127">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="b5db5-127">showOnLockScreen</span></span>|<span data-ttu-id="b5db5-128">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b5db5-128">Boolean</span></span>|<span data-ttu-id="b5db5-129">Gibt an, ob Benachrichtigungen auf dem Sperrbildschirm angezeigt werden können.</span><span class="sxs-lookup"><span data-stu-id="b5db5-129">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="b5db5-130">alertType</span><span class="sxs-lookup"><span data-stu-id="b5db5-130">alertType</span></span>|[<span data-ttu-id="b5db5-131">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="b5db5-131">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="b5db5-132">Gibt die Art der Warnung für Benachrichtigungen für diese App an.</span><span class="sxs-lookup"><span data-stu-id="b5db5-132">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="b5db5-133">Mögliche Werte: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="b5db5-133">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="b5db5-134">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="b5db5-134">badgesEnabled</span></span>|<span data-ttu-id="b5db5-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b5db5-135">Boolean</span></span>|<span data-ttu-id="b5db5-136">Gibt an, ob Badges für diese App zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="b5db5-136">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="b5db5-137">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="b5db5-137">soundsEnabled</span></span>|<span data-ttu-id="b5db5-138">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b5db5-138">Boolean</span></span>|<span data-ttu-id="b5db5-139">Gibt an, ob Ton für diese App zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="b5db5-139">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5db5-140">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b5db5-140">Relationships</span></span>
<span data-ttu-id="b5db5-141">Keine</span><span class="sxs-lookup"><span data-stu-id="b5db5-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5db5-142">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b5db5-142">JSON Representation</span></span>
<span data-ttu-id="b5db5-143">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b5db5-143">Here is a JSON representation of the resource.</span></span>
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




