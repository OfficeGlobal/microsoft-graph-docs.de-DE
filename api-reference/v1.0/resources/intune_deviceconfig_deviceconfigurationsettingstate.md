# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="932ca-101">deviceConfigurationSettingState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="932ca-101">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="932ca-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="932ca-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="932ca-103">Status der Konfigurationseinstellungen für ein bestimmtes Gerät</span><span class="sxs-lookup"><span data-stu-id="932ca-103">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="932ca-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="932ca-104">Properties</span></span>
|<span data-ttu-id="932ca-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="932ca-105">Property</span></span>|<span data-ttu-id="932ca-106">Typ</span><span class="sxs-lookup"><span data-stu-id="932ca-106">Type</span></span>|<span data-ttu-id="932ca-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="932ca-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="932ca-108">setting</span><span class="sxs-lookup"><span data-stu-id="932ca-108">setting</span></span>|<span data-ttu-id="932ca-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="932ca-109">String</span></span>|<span data-ttu-id="932ca-110">Die gemeldete Einstellung</span><span class="sxs-lookup"><span data-stu-id="932ca-110">The setting that is being reported</span></span>|
|<span data-ttu-id="932ca-111">settingName</span><span class="sxs-lookup"><span data-stu-id="932ca-111">settingName</span></span>|<span data-ttu-id="932ca-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="932ca-112">String</span></span>|<span data-ttu-id="932ca-113">Lokalisierter/benutzerfreundlicher Name der Einstellung, die gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="932ca-113">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="932ca-114">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="932ca-114">instanceDisplayName</span></span>|<span data-ttu-id="932ca-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="932ca-115">String</span></span>|<span data-ttu-id="932ca-116">Name der Einstellungsinstanz, die gemeldet wird</span><span class="sxs-lookup"><span data-stu-id="932ca-116">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="932ca-117">state</span><span class="sxs-lookup"><span data-stu-id="932ca-117">state</span></span>|<span data-ttu-id="932ca-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="932ca-118">String</span></span>|<span data-ttu-id="932ca-119">Der Konformitätsstatus der Einstellung. Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="932ca-119">The compliance state of the setting Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="932ca-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="932ca-120">errorCode</span></span>|<span data-ttu-id="932ca-121">Int64</span><span class="sxs-lookup"><span data-stu-id="932ca-121">Int64</span></span>|<span data-ttu-id="932ca-122">Fehlercode für die Einstellung</span><span class="sxs-lookup"><span data-stu-id="932ca-122">Error code for the setting</span></span>|
|<span data-ttu-id="932ca-123">errorDescription</span><span class="sxs-lookup"><span data-stu-id="932ca-123">error_description</span></span>|<span data-ttu-id="932ca-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="932ca-124">String</span></span>|<span data-ttu-id="932ca-125">Fehlerbeschreibung</span><span class="sxs-lookup"><span data-stu-id="932ca-125">Error Description</span></span>|
|<span data-ttu-id="932ca-126">userId</span><span class="sxs-lookup"><span data-stu-id="932ca-126">userID</span></span>|<span data-ttu-id="932ca-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="932ca-127">String</span></span>|<span data-ttu-id="932ca-128">Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="932ca-128">UserId</span></span>|
|<span data-ttu-id="932ca-129">userName</span><span class="sxs-lookup"><span data-stu-id="932ca-129">UserName</span></span>|<span data-ttu-id="932ca-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="932ca-130">String</span></span>|<span data-ttu-id="932ca-131">Benutzername</span><span class="sxs-lookup"><span data-stu-id="932ca-131">UserName</span></span>|
|<span data-ttu-id="932ca-132">userEmail</span><span class="sxs-lookup"><span data-stu-id="932ca-132">userEmail</span></span>|<span data-ttu-id="932ca-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="932ca-133">String</span></span>|<span data-ttu-id="932ca-134">E-Mail-Adresse des Benutzers</span><span class="sxs-lookup"><span data-stu-id="932ca-134">UserEmail Element</span></span>|
|<span data-ttu-id="932ca-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="932ca-135">userPrincipalName</span></span>|<span data-ttu-id="932ca-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="932ca-136">String</span></span>|<span data-ttu-id="932ca-137">Benutzer-Prinzipalname</span><span class="sxs-lookup"><span data-stu-id="932ca-137">userPrincipalName</span></span>|
|<span data-ttu-id="932ca-138">sources</span><span class="sxs-lookup"><span data-stu-id="932ca-138">Sources</span></span>|<span data-ttu-id="932ca-139">[settingSource](../resources/intune_deviceconfig_settingsource.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="932ca-139">[settingSource](../resources/intune_deviceconfig_settingsource.md) collection</span></span>|<span data-ttu-id="932ca-140">Beitragende Richtlinien</span><span class="sxs-lookup"><span data-stu-id="932ca-140">Contributing policies</span></span>|
|<span data-ttu-id="932ca-141">currentValue</span><span class="sxs-lookup"><span data-stu-id="932ca-141">currentValue</span></span>|<span data-ttu-id="932ca-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="932ca-142">String</span></span>|<span data-ttu-id="932ca-143">Aktueller Wert der Einstellung auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="932ca-143">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="932ca-144">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="932ca-144">Relationships</span></span>
<span data-ttu-id="932ca-145">Keine</span><span class="sxs-lookup"><span data-stu-id="932ca-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="932ca-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="932ca-146">JSON Representation</span></span>
<span data-ttu-id="932ca-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="932ca-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
}
-->
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



