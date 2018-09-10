# <a name="managedappstatus-resource-type"></a><span data-ttu-id="8f358-101">managedAppStatus-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8f358-101">managedAppStatus resource type</span></span>

> <span data-ttu-id="8f358-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8f358-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f358-103">Stellt den App-Schutz und den Konfigurationsstatus für die Organisation dar.</span><span class="sxs-lookup"><span data-stu-id="8f358-103">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="8f358-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="8f358-104">Methods</span></span>
|<span data-ttu-id="8f358-105">Methode</span><span class="sxs-lookup"><span data-stu-id="8f358-105">Method</span></span>|<span data-ttu-id="8f358-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="8f358-106">Return Type</span></span>|<span data-ttu-id="8f358-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f358-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8f358-108">managedAppStatuses auflisten</span><span class="sxs-lookup"><span data-stu-id="8f358-108">List managedAppStatuses</span></span>](../api/intune_mam_managedappstatus_list.md)|<span data-ttu-id="8f358-109">[managedAppStatus](../resources/intune_mam_managedappstatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8f358-109">[managedAppStatus](../resources/intune_mam_managedappstatus.md) collection</span></span>|<span data-ttu-id="8f358-110">Auflisten von Eigenschaften und Beziehungen der [managedAppStatus](../resources/intune_mam_managedappstatus.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="8f358-110">List properties and relationships of the [managedAppStatus](../resources/intune_mam_managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="8f358-111">managedAppStatus abrufen</span><span class="sxs-lookup"><span data-stu-id="8f358-111">Get managedAppStatus</span></span>](../api/intune_mam_managedappstatus_get.md)|[<span data-ttu-id="8f358-112">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="8f358-112">managedAppStatus</span></span>](../resources/intune_mam_managedappstatus.md)|<span data-ttu-id="8f358-113">Lesen von Eigenschaften und Beziehungen des [managedAppStatus](../resources/intune_mam_managedappstatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8f358-113">Read properties and relationships of the [managedAppStatus](../resources/intune_mam_managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8f358-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8f358-114">Properties</span></span>
|<span data-ttu-id="8f358-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8f358-115">Property</span></span>|<span data-ttu-id="8f358-116">Typ</span><span class="sxs-lookup"><span data-stu-id="8f358-116">Type</span></span>|<span data-ttu-id="8f358-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f358-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f358-118">displayName</span><span class="sxs-lookup"><span data-stu-id="8f358-118">displayName</span></span>|<span data-ttu-id="8f358-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8f358-119">String</span></span>|<span data-ttu-id="8f358-120">Anzeigename des Statusberichts</span><span class="sxs-lookup"><span data-stu-id="8f358-120">Friendly name of the status report.</span></span>|
|<span data-ttu-id="8f358-121">id</span><span class="sxs-lookup"><span data-stu-id="8f358-121">id</span></span>|<span data-ttu-id="8f358-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8f358-122">String</span></span>|<span data-ttu-id="8f358-123">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8f358-123">Key of the entity.</span></span>|
|<span data-ttu-id="8f358-124">Version</span><span class="sxs-lookup"><span data-stu-id="8f358-124">version</span></span>|<span data-ttu-id="8f358-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8f358-125">String</span></span>|<span data-ttu-id="8f358-126">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="8f358-126">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f358-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8f358-127">Relationships</span></span>
<span data-ttu-id="8f358-128">Keine</span><span class="sxs-lookup"><span data-stu-id="8f358-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8f358-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8f358-129">JSON Representation</span></span>
<span data-ttu-id="8f358-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8f358-130">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatus"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```








