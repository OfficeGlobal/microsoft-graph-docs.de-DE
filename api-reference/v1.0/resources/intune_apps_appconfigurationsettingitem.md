# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="a7d81-101">appConfigurationSettingItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a7d81-101">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="a7d81-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a7d81-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7d81-103">Enthält die Eigenschaften für ein App-Konfigurationseinstellungselement.</span><span class="sxs-lookup"><span data-stu-id="a7d81-103">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="a7d81-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a7d81-104">Properties</span></span>
|<span data-ttu-id="a7d81-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a7d81-105">Property</span></span>|<span data-ttu-id="a7d81-106">Typ</span><span class="sxs-lookup"><span data-stu-id="a7d81-106">Type</span></span>|<span data-ttu-id="a7d81-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a7d81-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7d81-108">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="a7d81-108">appConfigKey</span></span>|<span data-ttu-id="a7d81-109">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a7d81-109">String</span></span>|<span data-ttu-id="a7d81-110">App-Konfigurationsschlüssel</span><span class="sxs-lookup"><span data-stu-id="a7d81-110">app configuration key.</span></span>|
|<span data-ttu-id="a7d81-111">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="a7d81-111">appConfigKeyType</span></span>|[<span data-ttu-id="a7d81-112">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="a7d81-112">mdmAppConfigKeyType</span></span>](../resources/intune_apps_mdmappconfigkeytype.md)|<span data-ttu-id="a7d81-113">Typs des App-Konfigurationsschlüssels.</span><span class="sxs-lookup"><span data-stu-id="a7d81-113">app configuration key type.</span></span> <span data-ttu-id="a7d81-114">Mögliche Werte: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span><span class="sxs-lookup"><span data-stu-id="a7d81-114">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="a7d81-115">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="a7d81-115">appConfigKeyValue</span></span>|<span data-ttu-id="a7d81-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a7d81-116">String</span></span>|<span data-ttu-id="a7d81-117">Wert des App-Konfigurationsschlüssels</span><span class="sxs-lookup"><span data-stu-id="a7d81-117">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7d81-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a7d81-118">Relationships</span></span>
<span data-ttu-id="a7d81-119">Keine</span><span class="sxs-lookup"><span data-stu-id="a7d81-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a7d81-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a7d81-120">JSON Representation</span></span>
<span data-ttu-id="a7d81-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a7d81-121">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConfigurationSettingItem"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.appConfigurationSettingItem",
  "appConfigKey": "String",
  "appConfigKeyType": "String",
  "appConfigKeyValue": "String"
}
```








