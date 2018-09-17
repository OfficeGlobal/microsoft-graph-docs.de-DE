# <a name="devicecategory-resource-type"></a><span data-ttu-id="258f6-101">deviceCategory-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="258f6-101">deviceCategory resource type</span></span>

> <span data-ttu-id="258f6-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="258f6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="258f6-103">Gerätekategorien bieten eine Möglichkeit zum Organisieren Ihrer Geräte.</span><span class="sxs-lookup"><span data-stu-id="258f6-103">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="258f6-104">Mithilfe von Gerätekategorien können Unternehmensadministratoren eigene Kategorien definieren, die für ihr Unternehmen sinnvoll sind.</span><span class="sxs-lookup"><span data-stu-id="258f6-104">Using device categories, company administrators can define their own categories that make sense to their company.</span></span> <span data-ttu-id="258f6-105">Diese Kategorien können dann in der Intune Azure-Konsole auf ein Gerät angewendet oder bei der Geräteregistrierung von einem Benutzer ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="258f6-105">These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="258f6-106">Sie können basierend auf Gerätekategorien Berichte filtern und dynamische Azure Active Directory-Gerätegruppen erstellen.</span><span class="sxs-lookup"><span data-stu-id="258f6-106">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="258f6-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="258f6-107">Methods</span></span>
|<span data-ttu-id="258f6-108">Methode</span><span class="sxs-lookup"><span data-stu-id="258f6-108">Method</span></span>|<span data-ttu-id="258f6-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="258f6-109">Return Type</span></span>|<span data-ttu-id="258f6-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="258f6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="258f6-111">[List deviceCategories](../api/intune_shared_devicecategory_list.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="258f6-111">[List deviceCategories](../api/intune_shared_devicecategory_list.md) objects.</span></span>|
|<span data-ttu-id="258f6-112">[Get deviceCategory](../api/intune_shared_devicecategory_get.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="258f6-112">[Get deviceCategory](../api/intune_shared_devicecategory_get.md) object.</span></span>|
|<span data-ttu-id="258f6-113">[Create deviceCategory](../api/intune_shared_devicecategory_create.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="258f6-113">Create a new [deviceCategory](../api/intune_shared_devicecategory_create.md) object.</span></span>|
|<span data-ttu-id="258f6-114">[Delete deviceCategory](../api/intune_shared_devicecategory_delete.md).</span><span class="sxs-lookup"><span data-stu-id="258f6-114">Delete deviceCategory</span></span>|
|<span data-ttu-id="258f6-115">[Update deviceCategory](../api/intune_shared_devicecategory_update.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="258f6-115">Update the properties of a [deviceCategory](../api/intune_shared_devicecategory_update.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="258f6-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="258f6-116">Properties</span></span>
|<span data-ttu-id="258f6-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="258f6-117">Property</span></span>|<span data-ttu-id="258f6-118">Typ</span><span class="sxs-lookup"><span data-stu-id="258f6-118">Type</span></span>|<span data-ttu-id="258f6-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="258f6-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="258f6-120">ID</span><span class="sxs-lookup"><span data-stu-id="258f6-120">id</span></span>|<span data-ttu-id="258f6-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="258f6-121">String</span></span>|<span data-ttu-id="258f6-122">Eindeutiger Bezeichner für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="258f6-122">Unique identifier for the device category.</span></span> <span data-ttu-id="258f6-123">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="258f6-123">Read-only.</span></span>|
|<span data-ttu-id="258f6-124">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="258f6-124">**On-boarding**</span></span>|
|<span data-ttu-id="258f6-125">displayName</span><span class="sxs-lookup"><span data-stu-id="258f6-125">displayName</span></span>|<span data-ttu-id="258f6-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="258f6-126">String</span></span>|<span data-ttu-id="258f6-127">Der Anzeigename für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="258f6-127">Display name for the device category.</span></span>|
|<span data-ttu-id="258f6-128">description</span><span class="sxs-lookup"><span data-stu-id="258f6-128">description</span></span>|<span data-ttu-id="258f6-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="258f6-129">String</span></span>|<span data-ttu-id="258f6-130">Optionale Beschreibung für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="258f6-130">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="258f6-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="258f6-131">Relationships</span></span>
<span data-ttu-id="258f6-132">Keine</span><span class="sxs-lookup"><span data-stu-id="258f6-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="258f6-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="258f6-133">JSON Representation</span></span>
<span data-ttu-id="258f6-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="258f6-134">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceCategory"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



