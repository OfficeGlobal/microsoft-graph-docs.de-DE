# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="558ea-101">iosNotificationSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="558ea-101">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="558ea-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="558ea-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="558ea-103">Ein Element zur Beschreibung der Benachrichtigungseinstellungen.</span><span class="sxs-lookup"><span data-stu-id="558ea-103">An item describing notification setting.</span></span>
## <a name="properties"></a><span data-ttu-id="558ea-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="558ea-104">Properties</span></span>
|<span data-ttu-id="558ea-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="558ea-105">Property</span></span>|<span data-ttu-id="558ea-106">Typ</span><span class="sxs-lookup"><span data-stu-id="558ea-106">Type</span></span>|<span data-ttu-id="558ea-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="558ea-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="558ea-108">Paket-ID</span><span class="sxs-lookup"><span data-stu-id="558ea-108">bundleID</span></span>|<span data-ttu-id="558ea-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="558ea-109">String</span></span>|<span data-ttu-id="558ea-110">Paket-ID der App, auf die diese Benachrichtigungseinstellungen angewandt werden.</span><span class="sxs-lookup"><span data-stu-id="558ea-110">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="558ea-111">Anwendungsname</span><span class="sxs-lookup"><span data-stu-id="558ea-111">appName</span></span>|<span data-ttu-id="558ea-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="558ea-112">String</span></span>|<span data-ttu-id="558ea-113">Anwendungsname, der der Paket-ID zugeordnet werden muss.</span><span class="sxs-lookup"><span data-stu-id="558ea-113">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="558ea-114">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="558ea-114">publisher</span></span>|<span data-ttu-id="558ea-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="558ea-115">String</span></span>|<span data-ttu-id="558ea-116">Herausgeber, der der Paket-ID zugeordnet werden muss.</span><span class="sxs-lookup"><span data-stu-id="558ea-116">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="558ea-117">enabled</span><span class="sxs-lookup"><span data-stu-id="558ea-117">enabled</span></span>|<span data-ttu-id="558ea-118">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="558ea-118">Boolean</span></span>|<span data-ttu-id="558ea-119">Gibt an, ob Benachrichtigungen für diese App zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="558ea-119">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="558ea-120">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="558ea-120">showInNotificationCenter</span></span>|<span data-ttu-id="558ea-121">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="558ea-121">Boolean</span></span>|<span data-ttu-id="558ea-122">Gibt an, ob Benachrichtigungen im Nachrichtencenter angezeigt werden können.</span><span class="sxs-lookup"><span data-stu-id="558ea-122">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="558ea-123">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="558ea-123">showOnLockScreen</span></span>|<span data-ttu-id="558ea-124">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="558ea-124">Boolean</span></span>|<span data-ttu-id="558ea-125">Gibt an, ob Benachrichtigungen auf dem Sperrbildschirm angezeigt werden können.</span><span class="sxs-lookup"><span data-stu-id="558ea-125">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="558ea-126">alertType</span><span class="sxs-lookup"><span data-stu-id="558ea-126">alertType</span></span>|[<span data-ttu-id="558ea-127">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="558ea-127">iosNotificationAlertType</span></span>](../resources/intune_deviceconfig_iosnotificationalerttype.md)|<span data-ttu-id="558ea-128">Gibt die Art der Warnung für Benachrichtigungen für diese App an.</span><span class="sxs-lookup"><span data-stu-id="558ea-128">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="558ea-129">Mögliche Werte: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="558ea-129">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="558ea-130">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="558ea-130">badgesEnabled</span></span>|<span data-ttu-id="558ea-131">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="558ea-131">Boolean</span></span>|<span data-ttu-id="558ea-132">Gibt an, ob Badges für diese App zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="558ea-132">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="558ea-133">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="558ea-133">soundsEnabled</span></span>|<span data-ttu-id="558ea-134">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="558ea-134">Boolean</span></span>|<span data-ttu-id="558ea-135">Gibt an, ob Ton für diese App zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="558ea-135">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="558ea-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="558ea-136">Relationships</span></span>
<span data-ttu-id="558ea-137">Keine</span><span class="sxs-lookup"><span data-stu-id="558ea-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="558ea-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="558ea-138">JSON Representation</span></span>
<span data-ttu-id="558ea-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="558ea-139">Here is a JSON representation of the resource.</span></span>
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



