# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="e2eb4-101">iosNotificationSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e2eb4-101">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="e2eb4-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e2eb4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2eb4-103">Ein Element zur Beschreibung der Benachrichtigungseinstellungen.</span><span class="sxs-lookup"><span data-stu-id="e2eb4-103">An item describing notification setting.</span></span>
## <a name="properties"></a><span data-ttu-id="e2eb4-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e2eb4-104">Properties</span></span>
|<span data-ttu-id="e2eb4-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e2eb4-105">Property</span></span>|<span data-ttu-id="e2eb4-106">Typ</span><span class="sxs-lookup"><span data-stu-id="e2eb4-106">Type</span></span>|<span data-ttu-id="e2eb4-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e2eb4-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2eb4-108">Paket-ID</span><span class="sxs-lookup"><span data-stu-id="e2eb4-108">bundleID</span></span>|<span data-ttu-id="e2eb4-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e2eb4-109">String</span></span>|<span data-ttu-id="e2eb4-110">Paket-ID der App, auf die diese Benachrichtigungseinstellungen angewandt werden.</span><span class="sxs-lookup"><span data-stu-id="e2eb4-110">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="e2eb4-111">Anwendungsname</span><span class="sxs-lookup"><span data-stu-id="e2eb4-111">appname</span></span>|<span data-ttu-id="e2eb4-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e2eb4-112">String</span></span>|<span data-ttu-id="e2eb4-113">Anwendungsname, der der Paket-ID zugeordnet werden muss.</span><span class="sxs-lookup"><span data-stu-id="e2eb4-113">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="e2eb4-114">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="e2eb4-114">Publisher</span></span>|<span data-ttu-id="e2eb4-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e2eb4-115">String</span></span>|<span data-ttu-id="e2eb4-116">Herausgeber, der der Paket-ID zugeordnet werden muss.</span><span class="sxs-lookup"><span data-stu-id="e2eb4-116">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="e2eb4-117">enabled</span><span class="sxs-lookup"><span data-stu-id="e2eb4-117">enabled</span></span>|<span data-ttu-id="e2eb4-118">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e2eb4-118">Boolean</span></span>|<span data-ttu-id="e2eb4-119">Gibt an, ob Benachrichtigungen für diese App zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="e2eb4-119">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="e2eb4-120">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="e2eb4-120">showInNotificationCenter</span></span>|<span data-ttu-id="e2eb4-121">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e2eb4-121">Boolean</span></span>|<span data-ttu-id="e2eb4-122">Gibt an, ob Benachrichtigungen im Nachrichtencenter angezeigt werden können.</span><span class="sxs-lookup"><span data-stu-id="e2eb4-122">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="e2eb4-123">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="e2eb4-123">showOnLockScreen</span></span>|<span data-ttu-id="e2eb4-124">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e2eb4-124">Boolean</span></span>|<span data-ttu-id="e2eb4-125">Gibt an, ob Benachrichtigungen auf dem Sperrbildschirm angezeigt werden können.</span><span class="sxs-lookup"><span data-stu-id="e2eb4-125">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="e2eb4-126">alertType</span><span class="sxs-lookup"><span data-stu-id="e2eb4-126">alertType</span></span>|<span data-ttu-id="e2eb4-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e2eb4-127">String</span></span>|<span data-ttu-id="e2eb4-128">Gibt die Art der Warnung für Benachrichtigungen für diese App an.</span><span class="sxs-lookup"><span data-stu-id="e2eb4-128">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="e2eb4-129">Mögliche Werte: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="e2eb4-129">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="e2eb4-130">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="e2eb4-130">badgesEnabled</span></span>|<span data-ttu-id="e2eb4-131">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e2eb4-131">Boolean</span></span>|<span data-ttu-id="e2eb4-132">Gibt an, ob Badges für diese App zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="e2eb4-132">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="e2eb4-133">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="e2eb4-133">soundsEnabled</span></span>|<span data-ttu-id="e2eb4-134">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e2eb4-134">Boolean</span></span>|<span data-ttu-id="e2eb4-135">Gibt an, ob Ton für diese App zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="e2eb4-135">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2eb4-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e2eb4-136">Relationships</span></span>
<span data-ttu-id="e2eb4-137">Keine</span><span class="sxs-lookup"><span data-stu-id="e2eb4-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e2eb4-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e2eb4-138">JSON Representation</span></span>
<span data-ttu-id="e2eb4-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e2eb4-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



