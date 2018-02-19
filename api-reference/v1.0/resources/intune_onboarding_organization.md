# <a name="organization-resource-type"></a><span data-ttu-id="39150-101">organization-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="39150-101">organization resource type</span></span>

> <span data-ttu-id="39150-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="39150-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39150-103">Die organization-Ressource stellt eine Instanz der globalen Einstellungen und Ressourcen dar, die auf Mandantenebene ausgeführt und bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="39150-103">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="39150-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="39150-104">Methods</span></span>
|<span data-ttu-id="39150-105">Methode</span><span class="sxs-lookup"><span data-stu-id="39150-105">Method</span></span>|<span data-ttu-id="39150-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="39150-106">Return Type</span></span>|<span data-ttu-id="39150-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="39150-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="39150-108">Organisationen auflisten</span><span class="sxs-lookup"><span data-stu-id="39150-108">List organizations</span></span>](../api/intune_onboarding_organization_list.md)|<span data-ttu-id="39150-109">[organization](../resources/intune_onboarding_organization.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="39150-109">[organization](../resources/intune_onboarding_organization.md) collection</span></span>|<span data-ttu-id="39150-110">Auflisten von Eigenschaften und Beziehungen der [organization](../resources/intune_onboarding_organization.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="39150-110">List properties and relationships of the [organization](../resources/intune_onboarding_organization.md) objects.</span></span>|
|[<span data-ttu-id="39150-111">Organisation abrufen</span><span class="sxs-lookup"><span data-stu-id="39150-111">Get organization</span></span>](../api/intune_onboarding_organization_get.md)|[<span data-ttu-id="39150-112">organization</span><span class="sxs-lookup"><span data-stu-id="39150-112">organization</span></span>](../resources/intune_onboarding_organization.md)|<span data-ttu-id="39150-113">Dient zum Lesen der Eigenschaften und Beziehungen des [organization](../resources/intune_onboarding_organization.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="39150-113">Read properties and relationships of organization object.</span></span>|
|[<span data-ttu-id="39150-114">Organisation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="39150-114">Update organization</span></span>](../api/intune_onboarding_organization_update.md)|[<span data-ttu-id="39150-115">organization</span><span class="sxs-lookup"><span data-stu-id="39150-115">organization</span></span>](../resources/intune_onboarding_organization.md)|<span data-ttu-id="39150-116">Aktualisieren der Eigenschaften eines [organization](../resources/intune_onboarding_organization.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="39150-116">Update the properties of a [calendar](../resources/intune_onboarding_organization.md) object.</span></span>|
|[<span data-ttu-id="39150-117">setMobileDeviceManagementAuthority-Aktion</span><span class="sxs-lookup"><span data-stu-id="39150-117">setMobileDeviceManagementAuthority action</span></span>](../api/intune_onboarding_organization_setmobiledevicemanagementauthority.md)|<span data-ttu-id="39150-118">Int32</span><span class="sxs-lookup"><span data-stu-id="39150-118">Int32</span></span>|<span data-ttu-id="39150-119">Autorität für die Verwaltung mobiler Geräte festlegen</span><span class="sxs-lookup"><span data-stu-id="39150-119">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="39150-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="39150-120">Properties</span></span>
|<span data-ttu-id="39150-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="39150-121">Property</span></span>|<span data-ttu-id="39150-122">Typ</span><span class="sxs-lookup"><span data-stu-id="39150-122">Type</span></span>|<span data-ttu-id="39150-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="39150-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39150-124">id</span><span class="sxs-lookup"><span data-stu-id="39150-124">id</span></span>|<span data-ttu-id="39150-125">String</span><span class="sxs-lookup"><span data-stu-id="39150-125">String</span></span>|<span data-ttu-id="39150-126">Die GUID für das Objekt.</span><span class="sxs-lookup"><span data-stu-id="39150-126">The resource GUID for the security object is not valid.</span></span>|
|<span data-ttu-id="39150-127">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="39150-127">mobileDeviceManagementAuthority</span></span>|<span data-ttu-id="39150-128">String</span><span class="sxs-lookup"><span data-stu-id="39150-128">String</span></span>|<span data-ttu-id="39150-129">Autorität für die Verwaltung mobiler Geräte.</span><span class="sxs-lookup"><span data-stu-id="39150-129">Mobile device management authority.</span></span> <span data-ttu-id="39150-130">Mögliche Werte: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="39150-130">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39150-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="39150-131">Relationships</span></span>
<span data-ttu-id="39150-132">Keine</span><span class="sxs-lookup"><span data-stu-id="39150-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="39150-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="39150-133">JSON Representation</span></span>
<span data-ttu-id="39150-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="39150-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organization",
  "id": "String (identifier)",
  "mobileDeviceManagementAuthority": "String"
}
```



