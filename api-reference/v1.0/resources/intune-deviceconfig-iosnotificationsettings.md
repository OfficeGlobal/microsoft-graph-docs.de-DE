---
title: iosNotificationSettings-Ressourcentyp
description: Ein Element zur Beschreibung der Benachrichtigungseinstellungen.
author: tfitzmac
ms.openlocfilehash: 197de8b9cd59d1f6c998f92460e62aab480ef455
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307840"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="c550a-103">iosNotificationSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c550a-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="c550a-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c550a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c550a-105">Ein Element zur Beschreibung der Benachrichtigungseinstellungen.</span><span class="sxs-lookup"><span data-stu-id="c550a-105">An item describing notification setting.</span></span>
## <a name="properties"></a><span data-ttu-id="c550a-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c550a-106">Properties</span></span>
|<span data-ttu-id="c550a-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c550a-107">Property</span></span>|<span data-ttu-id="c550a-108">Typ</span><span class="sxs-lookup"><span data-stu-id="c550a-108">Type</span></span>|<span data-ttu-id="c550a-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c550a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c550a-110">Paket-ID</span><span class="sxs-lookup"><span data-stu-id="c550a-110">bundleID</span></span>|<span data-ttu-id="c550a-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c550a-111">String</span></span>|<span data-ttu-id="c550a-112">Paket-ID der App, auf die diese Benachrichtigungseinstellungen angewandt werden.</span><span class="sxs-lookup"><span data-stu-id="c550a-112">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="c550a-113">Anwendungsname</span><span class="sxs-lookup"><span data-stu-id="c550a-113">appName</span></span>|<span data-ttu-id="c550a-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c550a-114">String</span></span>|<span data-ttu-id="c550a-115">Anwendungsname, der der Paket-ID zugeordnet werden muss.</span><span class="sxs-lookup"><span data-stu-id="c550a-115">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="c550a-116">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="c550a-116">publisher</span></span>|<span data-ttu-id="c550a-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c550a-117">String</span></span>|<span data-ttu-id="c550a-118">Herausgeber, der der Paket-ID zugeordnet werden muss.</span><span class="sxs-lookup"><span data-stu-id="c550a-118">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="c550a-119">enabled</span><span class="sxs-lookup"><span data-stu-id="c550a-119">enabled</span></span>|<span data-ttu-id="c550a-120">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c550a-120">Boolean</span></span>|<span data-ttu-id="c550a-121">Gibt an, ob Benachrichtigungen für diese App zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="c550a-121">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="c550a-122">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="c550a-122">showInNotificationCenter</span></span>|<span data-ttu-id="c550a-123">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c550a-123">Boolean</span></span>|<span data-ttu-id="c550a-124">Gibt an, ob Benachrichtigungen im Nachrichtencenter angezeigt werden können.</span><span class="sxs-lookup"><span data-stu-id="c550a-124">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="c550a-125">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="c550a-125">showOnLockScreen</span></span>|<span data-ttu-id="c550a-126">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c550a-126">Boolean</span></span>|<span data-ttu-id="c550a-127">Gibt an, ob Benachrichtigungen auf dem Sperrbildschirm angezeigt werden können.</span><span class="sxs-lookup"><span data-stu-id="c550a-127">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="c550a-128">alertType</span><span class="sxs-lookup"><span data-stu-id="c550a-128">alertType</span></span>|[<span data-ttu-id="c550a-129">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="c550a-129">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="c550a-130">Gibt die Art der Warnung für Benachrichtigungen für diese App an.</span><span class="sxs-lookup"><span data-stu-id="c550a-130">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="c550a-131">Mögliche Werte: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="c550a-131">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="c550a-132">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="c550a-132">badgesEnabled</span></span>|<span data-ttu-id="c550a-133">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c550a-133">Boolean</span></span>|<span data-ttu-id="c550a-134">Gibt an, ob Badges für diese App zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="c550a-134">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="c550a-135">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="c550a-135">soundsEnabled</span></span>|<span data-ttu-id="c550a-136">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c550a-136">Boolean</span></span>|<span data-ttu-id="c550a-137">Gibt an, ob Ton für diese App zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="c550a-137">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c550a-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c550a-138">Relationships</span></span>
<span data-ttu-id="c550a-139">Keine</span><span class="sxs-lookup"><span data-stu-id="c550a-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c550a-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c550a-140">JSON Representation</span></span>
<span data-ttu-id="c550a-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c550a-141">Here is a JSON representation of the resource.</span></span>
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



