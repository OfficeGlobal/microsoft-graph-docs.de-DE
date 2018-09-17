# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="a0abe-101">deviceConfigurationSettingState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a0abe-101">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="a0abe-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a0abe-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0abe-103">Status der Konfigurationseinstellungen für ein bestimmtes Gerät</span><span class="sxs-lookup"><span data-stu-id="a0abe-103">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="a0abe-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a0abe-104">Properties</span></span>
|<span data-ttu-id="a0abe-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a0abe-105">Property</span></span>|<span data-ttu-id="a0abe-106">Typ</span><span class="sxs-lookup"><span data-stu-id="a0abe-106">Type</span></span>|<span data-ttu-id="a0abe-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a0abe-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0abe-108">Einstellung</span><span class="sxs-lookup"><span data-stu-id="a0abe-108">setting</span></span>|<span data-ttu-id="a0abe-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a0abe-109">String</span></span>|<span data-ttu-id="a0abe-110">Die gemeldete Einstellung</span><span class="sxs-lookup"><span data-stu-id="a0abe-110">The setting that is being reported</span></span>|
|<span data-ttu-id="a0abe-111">settingName</span><span class="sxs-lookup"><span data-stu-id="a0abe-111">settingName</span></span>|<span data-ttu-id="a0abe-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a0abe-112">String</span></span>|<span data-ttu-id="a0abe-113">Lokalisierter/benutzerfreundlicher Name der Einstellung, die gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="a0abe-113">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="a0abe-114">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a0abe-114">instanceDisplayName</span></span>|<span data-ttu-id="a0abe-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a0abe-115">String</span></span>|<span data-ttu-id="a0abe-116">Name der Einstellungsinstanz, die gemeldet wird.</span><span class="sxs-lookup"><span data-stu-id="a0abe-116">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="a0abe-117">Zustand</span><span class="sxs-lookup"><span data-stu-id="a0abe-117">state</span></span>|[<span data-ttu-id="a0abe-118">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="a0abe-118">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="a0abe-p101">Der Compliance-Zustand der Einstellung. Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="a0abe-p101">The compliance state of the setting Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="a0abe-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="a0abe-121">errorCode</span></span>|<span data-ttu-id="a0abe-122">Int64</span><span class="sxs-lookup"><span data-stu-id="a0abe-122">Int64</span></span>|<span data-ttu-id="a0abe-123">Fehlercode für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="a0abe-123">Error code for the setting</span></span>|
|<span data-ttu-id="a0abe-124">errorDescription</span><span class="sxs-lookup"><span data-stu-id="a0abe-124">errorDescription</span></span>|<span data-ttu-id="a0abe-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a0abe-125">String</span></span>|<span data-ttu-id="a0abe-126">Fehlerbeschreibung</span><span class="sxs-lookup"><span data-stu-id="a0abe-126">Error description</span></span>|
|<span data-ttu-id="a0abe-127">userId</span><span class="sxs-lookup"><span data-stu-id="a0abe-127">userId</span></span>|<span data-ttu-id="a0abe-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a0abe-128">String</span></span>|<span data-ttu-id="a0abe-129">UserId</span><span class="sxs-lookup"><span data-stu-id="a0abe-129">UserId</span></span>|
|<span data-ttu-id="a0abe-130">userName</span><span class="sxs-lookup"><span data-stu-id="a0abe-130">userName</span></span>|<span data-ttu-id="a0abe-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a0abe-131">String</span></span>|<span data-ttu-id="a0abe-132">UserName</span><span class="sxs-lookup"><span data-stu-id="a0abe-132">UserName</span></span>|
|<span data-ttu-id="a0abe-133">userEmail</span><span class="sxs-lookup"><span data-stu-id="a0abe-133">userEmail</span></span>|<span data-ttu-id="a0abe-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a0abe-134">String</span></span>|<span data-ttu-id="a0abe-135">UserEmail</span><span class="sxs-lookup"><span data-stu-id="a0abe-135">UserEmail</span></span>|
|<span data-ttu-id="a0abe-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a0abe-136">userPrincipalName</span></span>|<span data-ttu-id="a0abe-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a0abe-137">String</span></span>|<span data-ttu-id="a0abe-138">Benutzer-Prinzipalname</span><span class="sxs-lookup"><span data-stu-id="a0abe-138">UserPrincipalName.</span></span>|
|<span data-ttu-id="a0abe-139">Datenquellen</span><span class="sxs-lookup"><span data-stu-id="a0abe-139">sources</span></span>|<span data-ttu-id="a0abe-140">[settingSource](../resources/intune_deviceconfig_settingsource.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a0abe-140">[settingSource](../resources/intune_deviceconfig_settingsource.md) collection</span></span>|<span data-ttu-id="a0abe-141">Beitragende Richtlinien</span><span class="sxs-lookup"><span data-stu-id="a0abe-141">Contributing policies</span></span>|
|<span data-ttu-id="a0abe-142">currentValue</span><span class="sxs-lookup"><span data-stu-id="a0abe-142">currentValue</span></span>|<span data-ttu-id="a0abe-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a0abe-143">String</span></span>|<span data-ttu-id="a0abe-144">Aktueller Wert der Einstellung auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="a0abe-144">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0abe-145">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a0abe-145">Relationships</span></span>
<span data-ttu-id="a0abe-146">Keine</span><span class="sxs-lookup"><span data-stu-id="a0abe-146">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a0abe-147">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a0abe-147">JSON Representation</span></span>
<span data-ttu-id="a0abe-148">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a0abe-148">Here is a JSON representation of the resource.</span></span>
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








