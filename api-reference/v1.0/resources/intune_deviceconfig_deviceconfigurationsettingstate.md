# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="ecfa3-101">deviceConfigurationSettingState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ecfa3-101">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="ecfa3-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ecfa3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ecfa3-103">Status der Konfigurationseinstellungen für ein bestimmtes Gerät</span><span class="sxs-lookup"><span data-stu-id="ecfa3-103">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="ecfa3-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ecfa3-104">Properties</span></span>
|<span data-ttu-id="ecfa3-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ecfa3-105">Property</span></span>|<span data-ttu-id="ecfa3-106">Typ</span><span class="sxs-lookup"><span data-stu-id="ecfa3-106">Type</span></span>|<span data-ttu-id="ecfa3-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ecfa3-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecfa3-108">Einstellung</span><span class="sxs-lookup"><span data-stu-id="ecfa3-108">setting</span></span>|<span data-ttu-id="ecfa3-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ecfa3-109">String</span></span>|<span data-ttu-id="ecfa3-110">Die gemeldete Einstellung</span><span class="sxs-lookup"><span data-stu-id="ecfa3-110">The setting that is being reported</span></span>|
|<span data-ttu-id="ecfa3-111">settingName</span><span class="sxs-lookup"><span data-stu-id="ecfa3-111">settingName</span></span>|<span data-ttu-id="ecfa3-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ecfa3-112">String</span></span>|<span data-ttu-id="ecfa3-113">Lokalisierter/benutzerfreundlicher Name der Einstellung, die gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="ecfa3-113">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="ecfa3-114">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="ecfa3-114">instanceDisplayName</span></span>|<span data-ttu-id="ecfa3-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ecfa3-115">String</span></span>|<span data-ttu-id="ecfa3-116">Name der Einstellungsinstanz, die gemeldet wird.</span><span class="sxs-lookup"><span data-stu-id="ecfa3-116">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="ecfa3-117">Status</span><span class="sxs-lookup"><span data-stu-id="ecfa3-117">state</span></span>|[<span data-ttu-id="ecfa3-118">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="ecfa3-118">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="ecfa3-119">Der Compliance-Zustand der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="ecfa3-119">The compliance state of the setting Possible values are: , , , , , , .</span></span> <span data-ttu-id="ecfa3-120">Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="ecfa3-120">The possible values are `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, , , , , or .</span></span>|
|<span data-ttu-id="ecfa3-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="ecfa3-121">errorCode</span></span>|<span data-ttu-id="ecfa3-122">Int64</span><span class="sxs-lookup"><span data-stu-id="ecfa3-122">Int64</span></span>|<span data-ttu-id="ecfa3-123">Fehlercode für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="ecfa3-123">Error code for the setting</span></span>|
|<span data-ttu-id="ecfa3-124">errorDescription</span><span class="sxs-lookup"><span data-stu-id="ecfa3-124">errorDescription</span></span>|<span data-ttu-id="ecfa3-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ecfa3-125">String</span></span>|<span data-ttu-id="ecfa3-126">Fehlerbeschreibung</span><span class="sxs-lookup"><span data-stu-id="ecfa3-126">Error description</span></span>|
|<span data-ttu-id="ecfa3-127">userId</span><span class="sxs-lookup"><span data-stu-id="ecfa3-127">userId</span></span>|<span data-ttu-id="ecfa3-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ecfa3-128">String</span></span>|<span data-ttu-id="ecfa3-129">UserId</span><span class="sxs-lookup"><span data-stu-id="ecfa3-129">UserId</span></span>|
|<span data-ttu-id="ecfa3-130">userName</span><span class="sxs-lookup"><span data-stu-id="ecfa3-130">userName</span></span>|<span data-ttu-id="ecfa3-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ecfa3-131">String</span></span>|<span data-ttu-id="ecfa3-132">UserName</span><span class="sxs-lookup"><span data-stu-id="ecfa3-132">UserName</span></span>|
|<span data-ttu-id="ecfa3-133">userEmail</span><span class="sxs-lookup"><span data-stu-id="ecfa3-133">userEmail</span></span>|<span data-ttu-id="ecfa3-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ecfa3-134">String</span></span>|<span data-ttu-id="ecfa3-135">UserEmail</span><span class="sxs-lookup"><span data-stu-id="ecfa3-135">UserEmail</span></span>|
|<span data-ttu-id="ecfa3-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ecfa3-136">userPrincipalName</span></span>|<span data-ttu-id="ecfa3-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ecfa3-137">String</span></span>|<span data-ttu-id="ecfa3-138">Benutzer-Prinzipalname</span><span class="sxs-lookup"><span data-stu-id="ecfa3-138">UserPrincipalName.</span></span>|
|<span data-ttu-id="ecfa3-139">Datenquellen</span><span class="sxs-lookup"><span data-stu-id="ecfa3-139">sources</span></span>|<span data-ttu-id="ecfa3-140">[settingSource](../resources/intune_deviceconfig_settingsource.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ecfa3-140">[settingSource](../resources/intune_deviceconfig_settingsource.md) collection</span></span>|<span data-ttu-id="ecfa3-141">Beitragende Richtlinien</span><span class="sxs-lookup"><span data-stu-id="ecfa3-141">Contributing policies</span></span>|
|<span data-ttu-id="ecfa3-142">currentValue</span><span class="sxs-lookup"><span data-stu-id="ecfa3-142">currentValue</span></span>|<span data-ttu-id="ecfa3-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ecfa3-143">String</span></span>|<span data-ttu-id="ecfa3-144">Aktueller Wert der Einstellung auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="ecfa3-144">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="ecfa3-145">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ecfa3-145">Relationships</span></span>
<span data-ttu-id="ecfa3-146">Keine</span><span class="sxs-lookup"><span data-stu-id="ecfa3-146">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ecfa3-147">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ecfa3-147">JSON Representation</span></span>
<span data-ttu-id="ecfa3-148">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ecfa3-148">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationSettingState",
  "setting": "String",
  "settingName": "String",
  "instanceDisplayName": "String",
  "state": "String",
  "errorCode": 1024,
  "errorDescription": "String",
  "userId": "String",
  "userName": "String",
  "userEmail": "String",
  "userPrincipalName": "String",
  "sources": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String"
    }
  ],
  "currentValue": "String"
}
```



