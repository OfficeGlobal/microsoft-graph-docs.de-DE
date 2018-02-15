# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="61d03-101">deviceAppManagement-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="61d03-101">deviceAppManagement resource type</span></span>

> <span data-ttu-id="61d03-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="61d03-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61d03-103">Singleton-Entität, die als Container für alle Geräte-App-Verwaltungsfunktionen dient.</span><span class="sxs-lookup"><span data-stu-id="61d03-103">Singleton entity that acts as a container for all device app management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="61d03-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="61d03-104">Methods</span></span>
|<span data-ttu-id="61d03-105">Methode</span><span class="sxs-lookup"><span data-stu-id="61d03-105">Method</span></span>|<span data-ttu-id="61d03-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="61d03-106">Return Type</span></span>|<span data-ttu-id="61d03-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61d03-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="61d03-108">deviceAppManagement abrufen</span><span class="sxs-lookup"><span data-stu-id="61d03-108">Get deviceAppManagement</span></span>](../api/intune_books_deviceappmanagement_get.md)|[<span data-ttu-id="61d03-109">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="61d03-109">deviceAppManagement</span></span>](../resources/intune_books_deviceappmanagement.md)|<span data-ttu-id="61d03-110">Lesen von Eigenschaften und Beziehungen des [deviceAppManagement](../resources/intune_books_deviceappmanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="61d03-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_books_deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="61d03-111">deviceAppManagement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="61d03-111">Update deviceAppManagement</span></span>](../api/intune_books_deviceappmanagement_update.md)|[<span data-ttu-id="61d03-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="61d03-112">deviceAppManagement</span></span>](../resources/intune_books_deviceappmanagement.md)|<span data-ttu-id="61d03-113">Aktualisieren der Eigenschaften eines [deviceAppManagement](../resources/intune_books_deviceappmanagement.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="61d03-113">Update the properties of a [calendar](../resources/intune_books_deviceappmanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="61d03-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="61d03-114">Properties</span></span>
|<span data-ttu-id="61d03-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="61d03-115">Property</span></span>|<span data-ttu-id="61d03-116">Typ</span><span class="sxs-lookup"><span data-stu-id="61d03-116">Type</span></span>|<span data-ttu-id="61d03-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61d03-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61d03-118">id</span><span class="sxs-lookup"><span data-stu-id="61d03-118">id</span></span>|<span data-ttu-id="61d03-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="61d03-119">String</span></span>|<span data-ttu-id="61d03-120">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="61d03-120">Key of the setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61d03-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="61d03-121">Relationships</span></span>
|<span data-ttu-id="61d03-122">Beziehung</span><span class="sxs-lookup"><span data-stu-id="61d03-122">Relationship</span></span>|<span data-ttu-id="61d03-123">Typ</span><span class="sxs-lookup"><span data-stu-id="61d03-123">Type</span></span>|<span data-ttu-id="61d03-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61d03-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61d03-125">managedEBooks</span><span class="sxs-lookup"><span data-stu-id="61d03-125">managedEBooks</span></span>|<span data-ttu-id="61d03-126">[managedEBook](../resources/intune_books_managedebook.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="61d03-126">[managedEBook](../resources/intune_books_managedebook.md) collection</span></span>|<span data-ttu-id="61d03-127">Das verwaltete E-Book</span><span class="sxs-lookup"><span data-stu-id="61d03-127">The Managed eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="61d03-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="61d03-128">JSON Representation</span></span>
<span data-ttu-id="61d03-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="61d03-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```



