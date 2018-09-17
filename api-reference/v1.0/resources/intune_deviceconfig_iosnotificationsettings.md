# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="60443-101">iosNotificationSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="60443-101">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="60443-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="60443-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60443-103">Ein Element zur Beschreibung der Benachrichtigungseinstellungen.</span><span class="sxs-lookup"><span data-stu-id="60443-103">An item describing notification setting.</span></span>
## <a name="properties"></a><span data-ttu-id="60443-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="60443-104">Properties</span></span>
|<span data-ttu-id="60443-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="60443-105">Property</span></span>|<span data-ttu-id="60443-106">Typ</span><span class="sxs-lookup"><span data-stu-id="60443-106">Type</span></span>|<span data-ttu-id="60443-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="60443-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60443-108">Paket-ID</span><span class="sxs-lookup"><span data-stu-id="60443-108">bundleID</span></span>|<span data-ttu-id="60443-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="60443-109">String</span></span>|<span data-ttu-id="60443-110">Paket-ID der App, auf die diese Benachrichtigungseinstellungen angewandt werden.</span><span class="sxs-lookup"><span data-stu-id="60443-110">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="60443-111">Anwendungsname</span><span class="sxs-lookup"><span data-stu-id="60443-111">appName</span></span>|<span data-ttu-id="60443-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="60443-112">String</span></span>|<span data-ttu-id="60443-113">Anwendungsname, der der Paket-ID zugeordnet werden muss.</span><span class="sxs-lookup"><span data-stu-id="60443-113">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="60443-114">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="60443-114">publisher</span></span>|<span data-ttu-id="60443-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="60443-115">String</span></span>|<span data-ttu-id="60443-116">Herausgeber, der der Paket-ID zugeordnet werden muss.</span><span class="sxs-lookup"><span data-stu-id="60443-116">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="60443-117">aktiviert</span><span class="sxs-lookup"><span data-stu-id="60443-117">enabled</span></span>|<span data-ttu-id="60443-118">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="60443-118">Boolean</span></span>|<span data-ttu-id="60443-119">Gibt an, ob Benachrichtigungen für diese App zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="60443-119">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="60443-120">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="60443-120">showInNotificationCenter</span></span>|<span data-ttu-id="60443-121">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="60443-121">Boolean</span></span>|<span data-ttu-id="60443-122">Gibt an, ob Benachrichtigungen im Nachrichtencenter angezeigt werden können.</span><span class="sxs-lookup"><span data-stu-id="60443-122">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="60443-123">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="60443-123">showOnLockScreen</span></span>|<span data-ttu-id="60443-124">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="60443-124">Boolean</span></span>|<span data-ttu-id="60443-125">Gibt an, ob Benachrichtigungen auf dem Sperrbildschirm angezeigt werden können.</span><span class="sxs-lookup"><span data-stu-id="60443-125">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="60443-126">alertType</span><span class="sxs-lookup"><span data-stu-id="60443-126">alertType</span></span>|[<span data-ttu-id="60443-127">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="60443-127">iosNotificationAlertType values</span></span>](../resources/intune_deviceconfig_iosnotificationalerttype.md)|<span data-ttu-id="60443-128">Gibt die Art der Warnung für Benachrichtigungen für diese App an.</span><span class="sxs-lookup"><span data-stu-id="60443-128">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="60443-129">Mögliche Werte: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="60443-129">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="60443-130">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="60443-130">badgesEnabled</span></span>|<span data-ttu-id="60443-131">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="60443-131">Boolean</span></span>|<span data-ttu-id="60443-132">Gibt an, ob Badges für diese App zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="60443-132">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="60443-133">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="60443-133">soundsEnabled</span></span>|<span data-ttu-id="60443-134">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="60443-134">Boolean</span></span>|<span data-ttu-id="60443-135">Gibt an, ob Ton für diese App zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="60443-135">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60443-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="60443-136">Relationships</span></span>
<span data-ttu-id="60443-137">Keine</span><span class="sxs-lookup"><span data-stu-id="60443-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="60443-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="60443-138">JSON Representation</span></span>
<span data-ttu-id="60443-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="60443-139">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNotificationSettings"
}-->
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








