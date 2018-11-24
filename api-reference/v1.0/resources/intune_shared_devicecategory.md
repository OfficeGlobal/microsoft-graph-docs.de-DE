# <a name="devicecategory-resource-type"></a><span data-ttu-id="1445a-101">deviceCategory-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1445a-101">deviceCategory resource type</span></span>

> <span data-ttu-id="1445a-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1445a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1445a-103">Gerätekategorien bieten eine Möglichkeit zum Organisieren Ihrer Geräte.</span><span class="sxs-lookup"><span data-stu-id="1445a-103">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="1445a-104">Mithilfe von Gerätekategorien können Unternehmensadministratoren eigene Kategorien definieren, die für ihr Unternehmen sinnvoll sind.</span><span class="sxs-lookup"><span data-stu-id="1445a-104">Using device categories, company administrators can define their own categories that make sense to their company.</span></span><span data-ttu-id="1445a-105">Diese Kategorien können dann in der Intune Azure-Konsole auf ein Gerät angewendet oder bei der Geräteregistrierung von einem Benutzer ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="1445a-105"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="1445a-106">Sie können basierend auf Gerätekategorien Berichte filtern und dynamische Azure Active Directory-Gerätegruppen erstellen.</span><span class="sxs-lookup"><span data-stu-id="1445a-106">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="1445a-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="1445a-107">Methods</span></span>
|<span data-ttu-id="1445a-108">Methode</span><span class="sxs-lookup"><span data-stu-id="1445a-108">Method</span></span>|<span data-ttu-id="1445a-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="1445a-109">Return Type</span></span>|<span data-ttu-id="1445a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1445a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1445a-111">[Liste DeviceCategories](../api/intune_shared_devicecategory_list.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="1445a-111">[List deviceCategories](../api/intune_shared_devicecategory_list.md) collection</span></span>|<span data-ttu-id="1445a-112">Auflisten von Eigenschaften und Beziehungen der [deviceCategory](../resources/intune_shared_devicecategory.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="1445a-112">List properties and relationships of the [deviceCategory](../resources/intune_shared_devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="1445a-113">deviceCategory abrufen</span><span class="sxs-lookup"><span data-stu-id="1445a-113">Get deviceCategory</span></span>](../api/intune_shared_devicecategory_get.md)|<span data-ttu-id="1445a-114">Lesen von Eigenschaften und Beziehungen des [deviceCategory](../resources/intune_shared_devicecategory.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1445a-114">Read properties and relationships of the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>|
|[<span data-ttu-id="1445a-115">deviceCategory erstellen</span><span class="sxs-lookup"><span data-stu-id="1445a-115">Create deviceCategory</span></span>](../api/intune_shared_devicecategory_create.md)|<span data-ttu-id="1445a-116">Erstellen eines neuen [deviceCategory](../resources/intune_shared_devicecategory.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1445a-116">Create a new [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>|
|<span data-ttu-id="1445a-117">[DeviceCategory löschen](../api/intune_shared_devicecategory_delete.md).</span><span class="sxs-lookup"><span data-stu-id="1445a-117">[Delete deviceCategory](../api/intune_shared_devicecategory_delete.md).</span></span>|
|[<span data-ttu-id="1445a-118">deviceCategory aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1445a-118">Update deviceCategory</span></span>](../api/intune_shared_devicecategory_update.md)|<span data-ttu-id="1445a-119">Aktualisieren der Eigenschaften eines [deviceCategory](../resources/intune_shared_devicecategory.md)-Objekts</span><span class="sxs-lookup"><span data-stu-id="1445a-119">Update the properties of a [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1445a-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1445a-120">Properties</span></span>
|<span data-ttu-id="1445a-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1445a-121">Property</span></span>|<span data-ttu-id="1445a-122">Typ</span><span class="sxs-lookup"><span data-stu-id="1445a-122">Type</span></span>|<span data-ttu-id="1445a-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1445a-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1445a-124">id</span><span class="sxs-lookup"><span data-stu-id="1445a-124">id</span></span>|<span data-ttu-id="1445a-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1445a-125">String</span></span>|<span data-ttu-id="1445a-126">Eindeutiger Bezeichner für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="1445a-126">Unique identifier for the device category.</span></span> <span data-ttu-id="1445a-127">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1445a-127">Read-only.</span></span>|
|<span data-ttu-id="1445a-128">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="1445a-128">**Onboarding**</span></span>|
|<span data-ttu-id="1445a-129">displayName</span><span class="sxs-lookup"><span data-stu-id="1445a-129">displayName</span></span>|<span data-ttu-id="1445a-130">String</span><span class="sxs-lookup"><span data-stu-id="1445a-130">String</span></span>|<span data-ttu-id="1445a-131">Der Anzeigename für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="1445a-131">Display name for the device category.</span></span>|
|<span data-ttu-id="1445a-132">description</span><span class="sxs-lookup"><span data-stu-id="1445a-132">description</span></span>|<span data-ttu-id="1445a-133">String</span><span class="sxs-lookup"><span data-stu-id="1445a-133">String</span></span>|<span data-ttu-id="1445a-134">Optionale Beschreibung für die Gerätekategorie.</span><span class="sxs-lookup"><span data-stu-id="1445a-134">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1445a-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1445a-135">Relationships</span></span>
<span data-ttu-id="1445a-136">Keine</span><span class="sxs-lookup"><span data-stu-id="1445a-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1445a-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1445a-137">JSON Representation</span></span>
<span data-ttu-id="1445a-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1445a-138">Here is a JSON representation of the resource.</span></span>
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



