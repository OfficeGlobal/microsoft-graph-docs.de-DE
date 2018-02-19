# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="2ca74-101">deviceCompliancePolicySettingState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2ca74-101">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="2ca74-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2ca74-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ca74-103">Zustand der Gerätekonformitätsrichtlinien-Einstellung für ein bestimmtes Gerät.</span><span class="sxs-lookup"><span data-stu-id="2ca74-103">Device Compilance Policy Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="2ca74-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2ca74-104">Properties</span></span>
|<span data-ttu-id="2ca74-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2ca74-105">Property</span></span>|<span data-ttu-id="2ca74-106">Typ</span><span class="sxs-lookup"><span data-stu-id="2ca74-106">Type</span></span>|<span data-ttu-id="2ca74-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2ca74-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ca74-108">setting</span><span class="sxs-lookup"><span data-stu-id="2ca74-108">setting</span></span>|<span data-ttu-id="2ca74-109">String</span><span class="sxs-lookup"><span data-stu-id="2ca74-109">String</span></span>|<span data-ttu-id="2ca74-110">Die gemeldete Einstellung</span><span class="sxs-lookup"><span data-stu-id="2ca74-110">The setting that is being reported</span></span>|
|<span data-ttu-id="2ca74-111">settingName</span><span class="sxs-lookup"><span data-stu-id="2ca74-111">settingName</span></span>|<span data-ttu-id="2ca74-112">String</span><span class="sxs-lookup"><span data-stu-id="2ca74-112">String</span></span>|<span data-ttu-id="2ca74-113">Lokalisierter/benutzerfreundlicher Name der Einstellung, die gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="2ca74-113">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="2ca74-114">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="2ca74-114">instanceDisplayName</span></span>|<span data-ttu-id="2ca74-115">String</span><span class="sxs-lookup"><span data-stu-id="2ca74-115">String</span></span>|<span data-ttu-id="2ca74-116">Name der Einstellungsinstanz, die gemeldet wird.</span><span class="sxs-lookup"><span data-stu-id="2ca74-116">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="2ca74-117">state</span><span class="sxs-lookup"><span data-stu-id="2ca74-117">state</span></span>|<span data-ttu-id="2ca74-118">String</span><span class="sxs-lookup"><span data-stu-id="2ca74-118">String</span></span>|<span data-ttu-id="2ca74-119">Der Konformitätsstatus der Einstellung. Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="2ca74-119">The compliance state of the setting Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="2ca74-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="2ca74-120">errorCode</span></span>|<span data-ttu-id="2ca74-121">Int64</span><span class="sxs-lookup"><span data-stu-id="2ca74-121">Int64</span></span>|<span data-ttu-id="2ca74-122">Fehlercode für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="2ca74-122">Error code for the setting</span></span>|
|<span data-ttu-id="2ca74-123">errorDescription</span><span class="sxs-lookup"><span data-stu-id="2ca74-123">error_description</span></span>|<span data-ttu-id="2ca74-124">String</span><span class="sxs-lookup"><span data-stu-id="2ca74-124">String</span></span>|<span data-ttu-id="2ca74-125">Fehlerbeschreibung</span><span class="sxs-lookup"><span data-stu-id="2ca74-125">Error Description</span></span>|
|<span data-ttu-id="2ca74-126">userId</span><span class="sxs-lookup"><span data-stu-id="2ca74-126">userID</span></span>|<span data-ttu-id="2ca74-127">String</span><span class="sxs-lookup"><span data-stu-id="2ca74-127">String</span></span>|<span data-ttu-id="2ca74-128">UserId</span><span class="sxs-lookup"><span data-stu-id="2ca74-128">UserId</span></span>|
|<span data-ttu-id="2ca74-129">userName</span><span class="sxs-lookup"><span data-stu-id="2ca74-129">UserName</span></span>|<span data-ttu-id="2ca74-130">String</span><span class="sxs-lookup"><span data-stu-id="2ca74-130">String</span></span>|<span data-ttu-id="2ca74-131">UserName</span><span class="sxs-lookup"><span data-stu-id="2ca74-131">UserName</span></span>|
|<span data-ttu-id="2ca74-132">userEmail</span><span class="sxs-lookup"><span data-stu-id="2ca74-132">userEmail</span></span>|<span data-ttu-id="2ca74-133">String</span><span class="sxs-lookup"><span data-stu-id="2ca74-133">String</span></span>|<span data-ttu-id="2ca74-134">UserEmail</span><span class="sxs-lookup"><span data-stu-id="2ca74-134">UserEmail Element</span></span>|
|<span data-ttu-id="2ca74-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2ca74-135">userPrincipalName</span></span>|<span data-ttu-id="2ca74-136">String</span><span class="sxs-lookup"><span data-stu-id="2ca74-136">String</span></span>|<span data-ttu-id="2ca74-137">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="2ca74-137">userPrincipalName</span></span>|
|<span data-ttu-id="2ca74-138">sources</span><span class="sxs-lookup"><span data-stu-id="2ca74-138">Sources</span></span>|<span data-ttu-id="2ca74-139">[settingSource](../resources/intune_deviceconfig_settingsource.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="2ca74-139">[settingSource](../resources/intune_deviceconfig_settingsource.md) collection</span></span>|<span data-ttu-id="2ca74-140">Beitragende Richtlinien</span><span class="sxs-lookup"><span data-stu-id="2ca74-140">Contributing policies</span></span>|
|<span data-ttu-id="2ca74-141">currentValue</span><span class="sxs-lookup"><span data-stu-id="2ca74-141">currentValue</span></span>|<span data-ttu-id="2ca74-142">String</span><span class="sxs-lookup"><span data-stu-id="2ca74-142">String</span></span>|<span data-ttu-id="2ca74-143">Aktueller Wert der Einstellung auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="2ca74-143">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ca74-144">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2ca74-144">Relationships</span></span>
<span data-ttu-id="2ca74-145">Keine</span><span class="sxs-lookup"><span data-stu-id="2ca74-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2ca74-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2ca74-146">JSON Representation</span></span>
<span data-ttu-id="2ca74-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2ca74-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



