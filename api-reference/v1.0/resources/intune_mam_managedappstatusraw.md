# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="5e215-101">managedAppStatusRaw-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5e215-101">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="5e215-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5e215-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e215-103">Stellt einen nicht typisierten Statusbericht über App-Schutz und -Konfiguration der Organisation dar.</span><span class="sxs-lookup"><span data-stu-id="5e215-103">Represents an un-typed status report about organizations app protection and configuration.</span></span>

<span data-ttu-id="5e215-104">Erbt von [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="5e215-104">Inherits from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="5e215-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="5e215-105">Methods</span></span>
|<span data-ttu-id="5e215-106">Methode</span><span class="sxs-lookup"><span data-stu-id="5e215-106">Method</span></span>|<span data-ttu-id="5e215-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="5e215-107">Return Type</span></span>|<span data-ttu-id="5e215-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5e215-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5e215-109">managedAppStatusRaws auflisten</span><span class="sxs-lookup"><span data-stu-id="5e215-109">List managedAppStatusRaws</span></span>](../api/intune_mam_managedappstatusraw_list.md)|<span data-ttu-id="5e215-110">[managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="5e215-110">[managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) collection</span></span>|<span data-ttu-id="5e215-111">Auflisten von Eigenschaften und Beziehungen der [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="5e215-111">List properties and relationships of the [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="5e215-112">ManagedAppStatusRaw abrufen</span><span class="sxs-lookup"><span data-stu-id="5e215-112">Get managedAppStatusRaw</span></span>](../api/intune_mam_managedappstatusraw_get.md)|[<span data-ttu-id="5e215-113">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="5e215-113">managedAppStatusRaw</span></span>](../resources/intune_mam_managedappstatusraw.md)|<span data-ttu-id="5e215-114">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="5e215-114">Read properties and relationships of the [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5e215-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5e215-115">Properties</span></span>
|<span data-ttu-id="5e215-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5e215-116">Property</span></span>|<span data-ttu-id="5e215-117">Typ</span><span class="sxs-lookup"><span data-stu-id="5e215-117">Type</span></span>|<span data-ttu-id="5e215-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5e215-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e215-119">displayName</span><span class="sxs-lookup"><span data-stu-id="5e215-119">displayName</span></span>|<span data-ttu-id="5e215-120">String</span><span class="sxs-lookup"><span data-stu-id="5e215-120">String</span></span>|<span data-ttu-id="5e215-121">Anzeigename des Statusberichts.</span><span class="sxs-lookup"><span data-stu-id="5e215-121">Friendly name of the status report.</span></span> <span data-ttu-id="5e215-122">Geerbt von [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="5e215-122">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="5e215-123">id</span><span class="sxs-lookup"><span data-stu-id="5e215-123">id</span></span>|<span data-ttu-id="5e215-124">String</span><span class="sxs-lookup"><span data-stu-id="5e215-124">String</span></span>|<span data-ttu-id="5e215-125">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="5e215-125">Key of the entity.</span></span> <span data-ttu-id="5e215-126">Geerbt von [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="5e215-126">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="5e215-127">version</span><span class="sxs-lookup"><span data-stu-id="5e215-127">version</span></span>|<span data-ttu-id="5e215-128">String</span><span class="sxs-lookup"><span data-stu-id="5e215-128">String</span></span>|<span data-ttu-id="5e215-129">Version der Entität.</span><span class="sxs-lookup"><span data-stu-id="5e215-129">Version of the entity.</span></span> <span data-ttu-id="5e215-130">Geerbt von [managedAppStatus](../resources/intune_mam_managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="5e215-130">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="5e215-131">content</span><span class="sxs-lookup"><span data-stu-id="5e215-131">content</span></span>|[<span data-ttu-id="5e215-132">Json</span><span class="sxs-lookup"><span data-stu-id="5e215-132">Json</span></span>](../resources/intune_mam_json.md)|<span data-ttu-id="5e215-133">Inhalt des Statusberichts.</span><span class="sxs-lookup"><span data-stu-id="5e215-133">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e215-134">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5e215-134">Relationships</span></span>
<span data-ttu-id="5e215-135">Keine</span><span class="sxs-lookup"><span data-stu-id="5e215-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5e215-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5e215-136">JSON Representation</span></span>
<span data-ttu-id="5e215-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5e215-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatusRaw"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```



