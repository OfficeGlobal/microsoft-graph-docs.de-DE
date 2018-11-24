# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="095f6-101">deviceCompliancePolicySettingState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="095f6-101">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="095f6-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="095f6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="095f6-103">Zustand der Gerätekonformitätsrichtlinien-Einstellung für ein bestimmtes Gerät.</span><span class="sxs-lookup"><span data-stu-id="095f6-103">Device Compilance Policy Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="095f6-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="095f6-104">Properties</span></span>
|<span data-ttu-id="095f6-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="095f6-105">Property</span></span>|<span data-ttu-id="095f6-106">Typ</span><span class="sxs-lookup"><span data-stu-id="095f6-106">Type</span></span>|<span data-ttu-id="095f6-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="095f6-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="095f6-108">setting</span><span class="sxs-lookup"><span data-stu-id="095f6-108">setting</span></span>|<span data-ttu-id="095f6-109">String</span><span class="sxs-lookup"><span data-stu-id="095f6-109">String</span></span>|<span data-ttu-id="095f6-110">Die gemeldete Einstellung</span><span class="sxs-lookup"><span data-stu-id="095f6-110">The setting that is being reported</span></span>|
|<span data-ttu-id="095f6-111">settingName</span><span class="sxs-lookup"><span data-stu-id="095f6-111">settingName</span></span>|<span data-ttu-id="095f6-112">String</span><span class="sxs-lookup"><span data-stu-id="095f6-112">String</span></span>|<span data-ttu-id="095f6-113">Lokalisierter/benutzerfreundlicher Name der Einstellung, die gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="095f6-113">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="095f6-114">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="095f6-114">instanceDisplayName</span></span>|<span data-ttu-id="095f6-115">String</span><span class="sxs-lookup"><span data-stu-id="095f6-115">String</span></span>|<span data-ttu-id="095f6-116">Name der Einstellungsinstanz, die gemeldet wird.</span><span class="sxs-lookup"><span data-stu-id="095f6-116">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="095f6-117">state</span><span class="sxs-lookup"><span data-stu-id="095f6-117">state</span></span>|[<span data-ttu-id="095f6-118">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="095f6-118">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="095f6-119">Der Compliance-Zustand der Einstellung.</span><span class="sxs-lookup"><span data-stu-id="095f6-119">The compliance state of the setting.</span></span> <span data-ttu-id="095f6-120">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="095f6-120">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="095f6-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="095f6-121">errorCode</span></span>|<span data-ttu-id="095f6-122">Int64</span><span class="sxs-lookup"><span data-stu-id="095f6-122">Int64</span></span>|<span data-ttu-id="095f6-123">Fehlercode für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="095f6-123">Error code for the setting</span></span>|
|<span data-ttu-id="095f6-124">errorDescription</span><span class="sxs-lookup"><span data-stu-id="095f6-124">errorDescription</span></span>|<span data-ttu-id="095f6-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="095f6-125">String</span></span>|<span data-ttu-id="095f6-126">Fehlerbeschreibung</span><span class="sxs-lookup"><span data-stu-id="095f6-126">Error description</span></span>|
|<span data-ttu-id="095f6-127">userId</span><span class="sxs-lookup"><span data-stu-id="095f6-127">userId</span></span>|<span data-ttu-id="095f6-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="095f6-128">String</span></span>|<span data-ttu-id="095f6-129">UserId</span><span class="sxs-lookup"><span data-stu-id="095f6-129">UserId</span></span>|
|<span data-ttu-id="095f6-130">userName</span><span class="sxs-lookup"><span data-stu-id="095f6-130">userName</span></span>|<span data-ttu-id="095f6-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="095f6-131">String</span></span>|<span data-ttu-id="095f6-132">UserName</span><span class="sxs-lookup"><span data-stu-id="095f6-132">UserName</span></span>|
|<span data-ttu-id="095f6-133">userEmail</span><span class="sxs-lookup"><span data-stu-id="095f6-133">userEmail</span></span>|<span data-ttu-id="095f6-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="095f6-134">String</span></span>|<span data-ttu-id="095f6-135">UserEmail</span><span class="sxs-lookup"><span data-stu-id="095f6-135">UserEmail</span></span>|
|<span data-ttu-id="095f6-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="095f6-136">userPrincipalName</span></span>|<span data-ttu-id="095f6-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="095f6-137">String</span></span>|<span data-ttu-id="095f6-138">Benutzer-Prinzipalname</span><span class="sxs-lookup"><span data-stu-id="095f6-138">UserPrincipalName.</span></span>|
|<span data-ttu-id="095f6-139">sources</span><span class="sxs-lookup"><span data-stu-id="095f6-139">sources</span></span>|<span data-ttu-id="095f6-140">[settingSource](../resources/intune_deviceconfig_settingsource.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="095f6-140">[settingSource](../resources/intune_deviceconfig_settingsource.md) collection</span></span>|<span data-ttu-id="095f6-141">Beitragende Richtlinien</span><span class="sxs-lookup"><span data-stu-id="095f6-141">Contributing policies</span></span>|
|<span data-ttu-id="095f6-142">currentValue</span><span class="sxs-lookup"><span data-stu-id="095f6-142">currentValue</span></span>|<span data-ttu-id="095f6-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="095f6-143">String</span></span>|<span data-ttu-id="095f6-144">Aktueller Wert der Einstellung auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="095f6-144">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="095f6-145">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="095f6-145">Relationships</span></span>
<span data-ttu-id="095f6-146">Keine</span><span class="sxs-lookup"><span data-stu-id="095f6-146">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="095f6-147">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="095f6-147">JSON Representation</span></span>
<span data-ttu-id="095f6-148">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="095f6-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingState",
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



