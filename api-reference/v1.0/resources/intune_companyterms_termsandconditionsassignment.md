# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="c29c7-101">termsAndConditionsAssignment-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c29c7-101">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="c29c7-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c29c7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c29c7-103">Eine TermsAndConditionsAssignment-Entität steht für die Zuweisung einer bestimmten Richtlinie der Nutzungsbedingungen (Terms and Conditions, T&C) zu einer bestimmten Gruppe.</span><span class="sxs-lookup"><span data-stu-id="c29c7-103">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="c29c7-104">Benutzer in der Gruppe müssen die Nutzungsbedingungen annehmen, um Geräte in Intune registrieren zu lassen.</span><span class="sxs-lookup"><span data-stu-id="c29c7-104">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="c29c7-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="c29c7-105">Methods</span></span>
|<span data-ttu-id="c29c7-106">Methode</span><span class="sxs-lookup"><span data-stu-id="c29c7-106">Method</span></span>|<span data-ttu-id="c29c7-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="c29c7-107">Return Type</span></span>|<span data-ttu-id="c29c7-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c29c7-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c29c7-109">termsAndConditionsAssignments auflisten</span><span class="sxs-lookup"><span data-stu-id="c29c7-109">List termsAndConditionsAssignments</span></span>](../api/intune_companyterms_termsandconditionsassignment_list.md)|<span data-ttu-id="c29c7-110">[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c29c7-110">[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="c29c7-111">Auflisten von Eigenschaften und Beziehungen der [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="c29c7-111">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="c29c7-112">termsAndConditionsAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="c29c7-112">Get termsAndConditionsAssignment</span></span>](../api/intune_companyterms_termsandconditionsassignment_get.md)|[<span data-ttu-id="c29c7-113">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="c29c7-113">termsAndConditionsAssignment</span></span>](../resources/intune_companyterms_termsandconditionsassignment.md)|<span data-ttu-id="c29c7-114">Lesen von Eigenschaften und Beziehungen des [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c29c7-114">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="c29c7-115">termsAndConditionsAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="c29c7-115">Create termsAndConditionsAssignment</span></span>](../api/intune_companyterms_termsandconditionsassignment_create.md)|[<span data-ttu-id="c29c7-116">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="c29c7-116">termsAndConditionsAssignment</span></span>](../resources/intune_companyterms_termsandconditionsassignment.md)|<span data-ttu-id="c29c7-117">Erstellen eines neuen [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c29c7-117">Create a new [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="c29c7-118">termsAndConditionsAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="c29c7-118">Delete termsAndConditionsAssignment</span></span>](../api/intune_companyterms_termsandconditionsassignment_delete.md)|<span data-ttu-id="c29c7-119">Keine</span><span class="sxs-lookup"><span data-stu-id="c29c7-119">None</span></span>|<span data-ttu-id="c29c7-120">Löscht ein [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c29c7-120">Deletes a [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="c29c7-121">termsAndConditionsAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c29c7-121">Update termsAndConditionsAssignment</span></span>](../api/intune_companyterms_termsandconditionsassignment_update.md)|[<span data-ttu-id="c29c7-122">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="c29c7-122">termsAndConditionsAssignment</span></span>](../resources/intune_companyterms_termsandconditionsassignment.md)|<span data-ttu-id="c29c7-123">Aktualisieren der Eigenschaften eines [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c29c7-123">Update the properties of a [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c29c7-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c29c7-124">Properties</span></span>
|<span data-ttu-id="c29c7-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c29c7-125">Property</span></span>|<span data-ttu-id="c29c7-126">Typ</span><span class="sxs-lookup"><span data-stu-id="c29c7-126">Type</span></span>|<span data-ttu-id="c29c7-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c29c7-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c29c7-128">ID</span><span class="sxs-lookup"><span data-stu-id="c29c7-128">id</span></span>|<span data-ttu-id="c29c7-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c29c7-129">String</span></span>|<span data-ttu-id="c29c7-130">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="c29c7-130">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="c29c7-131">Ziel</span><span class="sxs-lookup"><span data-stu-id="c29c7-131">target</span></span>|[<span data-ttu-id="c29c7-132">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c29c7-132">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c29c7-133">Zuweisungsziel, dem die Richtlinie der Nutzungsbedingungen zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="c29c7-133">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c29c7-134">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c29c7-134">Relationships</span></span>
<span data-ttu-id="c29c7-135">Keine</span><span class="sxs-lookup"><span data-stu-id="c29c7-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c29c7-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c29c7-136">JSON Representation</span></span>
<span data-ttu-id="c29c7-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c29c7-137">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```








