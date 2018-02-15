# <a name="devicemanagement-resource-type"></a><span data-ttu-id="4c2b2-101">deviceManagement-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4c2b2-101">deviceManagement resource type</span></span>

> <span data-ttu-id="4c2b2-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4c2b2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c2b2-103">Singleton-Entität, die als Container für alle Geräteverwaltungsfunktionen dient.</span><span class="sxs-lookup"><span data-stu-id="4c2b2-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="4c2b2-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="4c2b2-104">Methods</span></span>
|<span data-ttu-id="4c2b2-105">Methode</span><span class="sxs-lookup"><span data-stu-id="4c2b2-105">Method</span></span>|<span data-ttu-id="4c2b2-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="4c2b2-106">Return Type</span></span>|<span data-ttu-id="4c2b2-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4c2b2-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4c2b2-108">deviceManagement abrufen</span><span class="sxs-lookup"><span data-stu-id="4c2b2-108">Get deviceManagement</span></span>](../api/intune_companyterms_devicemanagement_get.md)|[<span data-ttu-id="4c2b2-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="4c2b2-109">deviceManagement</span></span>](../resources/intune_companyterms_devicemanagement.md)|<span data-ttu-id="4c2b2-110">Lesen von Eigenschaften und Beziehungen des [deviceManagement](../resources/intune_companyterms_devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4c2b2-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_companyterms_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="4c2b2-111">deviceManagement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4c2b2-111">Update deviceManagement</span></span>](../api/intune_companyterms_devicemanagement_update.md)|[<span data-ttu-id="4c2b2-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="4c2b2-112">deviceManagement</span></span>](../resources/intune_companyterms_devicemanagement.md)|<span data-ttu-id="4c2b2-113">Aktualisieren der Eigenschaften eines [deviceManagement](../resources/intune_companyterms_devicemanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4c2b2-113">Update the properties of a [calendar](../resources/intune_companyterms_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4c2b2-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4c2b2-114">Properties</span></span>
|<span data-ttu-id="4c2b2-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4c2b2-115">Property</span></span>|<span data-ttu-id="4c2b2-116">Typ</span><span class="sxs-lookup"><span data-stu-id="4c2b2-116">Type</span></span>|<span data-ttu-id="4c2b2-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4c2b2-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c2b2-118">id</span><span class="sxs-lookup"><span data-stu-id="4c2b2-118">id</span></span>|<span data-ttu-id="4c2b2-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4c2b2-119">String</span></span>|<span data-ttu-id="4c2b2-120">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="4c2b2-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c2b2-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4c2b2-121">Relationships</span></span>
|<span data-ttu-id="4c2b2-122">Beziehung</span><span class="sxs-lookup"><span data-stu-id="4c2b2-122">Relationship</span></span>|<span data-ttu-id="4c2b2-123">Typ</span><span class="sxs-lookup"><span data-stu-id="4c2b2-123">Type</span></span>|<span data-ttu-id="4c2b2-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4c2b2-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c2b2-125">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="4c2b2-125">termsAndConditions</span></span>|<span data-ttu-id="4c2b2-126">[termsAndConditions](../resources/intune_companyterms_termsandconditions.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4c2b2-126">[termsAndConditions](../resources/intune_companyterms_termsandconditions.md) collection</span></span>|<span data-ttu-id="4c2b2-127">Die allgemeinen Geschäftsbedingungen für die Geräteverwaltung des Unternehmens.</span><span class="sxs-lookup"><span data-stu-id="4c2b2-127">The terms and conditions associated with device management of the company.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4c2b2-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4c2b2-128">JSON Representation</span></span>
<span data-ttu-id="4c2b2-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4c2b2-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



