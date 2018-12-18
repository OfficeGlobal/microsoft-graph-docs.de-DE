---
title: iosNotificationSettings-Ressourcentyp
description: Ein Element zur Beschreibung der Benachrichtigungseinstellungen.
author: tfitzmac
ms.openlocfilehash: c24e0719e634d2939f88280431538b41fb0a1b5f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359192"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="79f9e-103">iosNotificationSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="79f9e-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="79f9e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="79f9e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79f9e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="79f9e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="79f9e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="79f9e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79f9e-107">Ein Element zur Beschreibung der Benachrichtigungseinstellungen.</span><span class="sxs-lookup"><span data-stu-id="79f9e-107">An item describing notification setting.</span></span>
## <a name="properties"></a><span data-ttu-id="79f9e-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="79f9e-108">Properties</span></span>
|<span data-ttu-id="79f9e-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="79f9e-109">Property</span></span>|<span data-ttu-id="79f9e-110">Typ</span><span class="sxs-lookup"><span data-stu-id="79f9e-110">Type</span></span>|<span data-ttu-id="79f9e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79f9e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79f9e-112">Paket-ID</span><span class="sxs-lookup"><span data-stu-id="79f9e-112">bundleID</span></span>|<span data-ttu-id="79f9e-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="79f9e-113">String</span></span>|<span data-ttu-id="79f9e-114">Paket-ID der App, auf die diese Benachrichtigungseinstellungen angewandt werden.</span><span class="sxs-lookup"><span data-stu-id="79f9e-114">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="79f9e-115">Anwendungsname</span><span class="sxs-lookup"><span data-stu-id="79f9e-115">appName</span></span>|<span data-ttu-id="79f9e-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="79f9e-116">String</span></span>|<span data-ttu-id="79f9e-117">Anwendungsname, der der Paket-ID zugeordnet werden muss.</span><span class="sxs-lookup"><span data-stu-id="79f9e-117">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="79f9e-118">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="79f9e-118">publisher</span></span>|<span data-ttu-id="79f9e-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="79f9e-119">String</span></span>|<span data-ttu-id="79f9e-120">Herausgeber, der der Paket-ID zugeordnet werden muss.</span><span class="sxs-lookup"><span data-stu-id="79f9e-120">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="79f9e-121">enabled</span><span class="sxs-lookup"><span data-stu-id="79f9e-121">enabled</span></span>|<span data-ttu-id="79f9e-122">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="79f9e-122">Boolean</span></span>|<span data-ttu-id="79f9e-123">Gibt an, ob Benachrichtigungen für diese App zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="79f9e-123">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="79f9e-124">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="79f9e-124">showInNotificationCenter</span></span>|<span data-ttu-id="79f9e-125">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="79f9e-125">Boolean</span></span>|<span data-ttu-id="79f9e-126">Gibt an, ob Benachrichtigungen im Nachrichtencenter angezeigt werden können.</span><span class="sxs-lookup"><span data-stu-id="79f9e-126">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="79f9e-127">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="79f9e-127">showOnLockScreen</span></span>|<span data-ttu-id="79f9e-128">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="79f9e-128">Boolean</span></span>|<span data-ttu-id="79f9e-129">Gibt an, ob Benachrichtigungen auf dem Sperrbildschirm angezeigt werden können.</span><span class="sxs-lookup"><span data-stu-id="79f9e-129">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="79f9e-130">alertType</span><span class="sxs-lookup"><span data-stu-id="79f9e-130">alertType</span></span>|[<span data-ttu-id="79f9e-131">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="79f9e-131">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="79f9e-132">Gibt die Art der Warnung für Benachrichtigungen für diese App an.</span><span class="sxs-lookup"><span data-stu-id="79f9e-132">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="79f9e-133">Mögliche Werte: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="79f9e-133">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="79f9e-134">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="79f9e-134">badgesEnabled</span></span>|<span data-ttu-id="79f9e-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="79f9e-135">Boolean</span></span>|<span data-ttu-id="79f9e-136">Gibt an, ob Badges für diese App zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="79f9e-136">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="79f9e-137">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="79f9e-137">soundsEnabled</span></span>|<span data-ttu-id="79f9e-138">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="79f9e-138">Boolean</span></span>|<span data-ttu-id="79f9e-139">Gibt an, ob Ton für diese App zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="79f9e-139">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79f9e-140">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="79f9e-140">Relationships</span></span>
<span data-ttu-id="79f9e-141">Keine</span><span class="sxs-lookup"><span data-stu-id="79f9e-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="79f9e-142">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="79f9e-142">JSON Representation</span></span>
<span data-ttu-id="79f9e-143">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="79f9e-143">Here is a JSON representation of the resource.</span></span>
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





