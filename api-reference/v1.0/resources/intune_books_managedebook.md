# <a name="managedebook-resource-type"></a><span data-ttu-id="91e87-101">managedEBook-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="91e87-101">managedEBook resource type</span></span>

> <span data-ttu-id="91e87-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="91e87-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91e87-103">Eine abstrakte Klasse, die die grundlegenden Eigenschaften des verwalteten eBooks enthält</span><span class="sxs-lookup"><span data-stu-id="91e87-103">An abstract class containing the base properties for Managed eBook.</span></span>
## <a name="methods"></a><span data-ttu-id="91e87-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="91e87-104">Methods</span></span>
|<span data-ttu-id="91e87-105">Methode</span><span class="sxs-lookup"><span data-stu-id="91e87-105">Method</span></span>|<span data-ttu-id="91e87-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="91e87-106">Return Type</span></span>|<span data-ttu-id="91e87-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91e87-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="91e87-108">managedEBooks auflisten</span><span class="sxs-lookup"><span data-stu-id="91e87-108">List managedEBooks</span></span>](../api/intune_books_managedebook_list.md)|<span data-ttu-id="91e87-109">[managedEBook](../resources/intune_books_managedebook.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="91e87-109">[managedEBook](../resources/intune_books_managedebook.md) collection</span></span>|<span data-ttu-id="91e87-110">Auflisten von Eigenschaften und Beziehungen der [managedEBook](../resources/intune_books_managedebook.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="91e87-110">List properties and relationships of the [managedEBook](../resources/intune_books_managedebook.md) objects.</span></span>|
|[<span data-ttu-id="91e87-111">managedEBook abrufen</span><span class="sxs-lookup"><span data-stu-id="91e87-111">Get managedEBook</span></span>](../api/intune_books_managedebook_get.md)|[<span data-ttu-id="91e87-112">managedEBook</span><span class="sxs-lookup"><span data-stu-id="91e87-112">managedEBook</span></span>](../resources/intune_books_managedebook.md)|<span data-ttu-id="91e87-113">Lesen von Eigenschaften und Beziehungen des [managedEBook](../resources/intune_books_managedebook.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="91e87-113">Read properties and relationships of the [managedEBook](../resources/intune_books_managedebook.md) object.</span></span>|
|[<span data-ttu-id="91e87-114">Aktion zuweisen</span><span class="sxs-lookup"><span data-stu-id="91e87-114">assign action</span></span>](../api/intune_books_managedebook_assign.md)|<span data-ttu-id="91e87-115">Keine</span><span class="sxs-lookup"><span data-stu-id="91e87-115">None</span></span>|<span data-ttu-id="91e87-116">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="91e87-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="91e87-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="91e87-117">Properties</span></span>
|<span data-ttu-id="91e87-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="91e87-118">Property</span></span>|<span data-ttu-id="91e87-119">Typ</span><span class="sxs-lookup"><span data-stu-id="91e87-119">Type</span></span>|<span data-ttu-id="91e87-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91e87-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91e87-121">id</span><span class="sxs-lookup"><span data-stu-id="91e87-121">id</span></span>|<span data-ttu-id="91e87-122">String</span><span class="sxs-lookup"><span data-stu-id="91e87-122">String</span></span>|<span data-ttu-id="91e87-123">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="91e87-123">Key of the entity.</span></span>|
|<span data-ttu-id="91e87-124">displayName</span><span class="sxs-lookup"><span data-stu-id="91e87-124">displayName</span></span>|<span data-ttu-id="91e87-125">String</span><span class="sxs-lookup"><span data-stu-id="91e87-125">String</span></span>|<span data-ttu-id="91e87-126">Name des E-Books</span><span class="sxs-lookup"><span data-stu-id="91e87-126">Name of the eBook.</span></span>|
|<span data-ttu-id="91e87-127">description</span><span class="sxs-lookup"><span data-stu-id="91e87-127">description</span></span>|<span data-ttu-id="91e87-128">String</span><span class="sxs-lookup"><span data-stu-id="91e87-128">String</span></span>|<span data-ttu-id="91e87-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91e87-129">Description.</span></span>|
|<span data-ttu-id="91e87-130">publisher</span><span class="sxs-lookup"><span data-stu-id="91e87-130">publisher</span></span>|<span data-ttu-id="91e87-131">String</span><span class="sxs-lookup"><span data-stu-id="91e87-131">String</span></span>|<span data-ttu-id="91e87-132">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="91e87-132">Publisher.</span></span>|
|<span data-ttu-id="91e87-133">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="91e87-133">publishedDateTime</span></span>|<span data-ttu-id="91e87-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91e87-134">DateTimeOffset</span></span>|<span data-ttu-id="91e87-135">Datum und Uhrzeit der Veröffentlichung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="91e87-135">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="91e87-136">largeCover</span><span class="sxs-lookup"><span data-stu-id="91e87-136">largeCover</span></span>|[<span data-ttu-id="91e87-137">mimeContent</span><span class="sxs-lookup"><span data-stu-id="91e87-137">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="91e87-138">Umschlagbild des Buchs</span><span class="sxs-lookup"><span data-stu-id="91e87-138">Book cover.</span></span>|
|<span data-ttu-id="91e87-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="91e87-139">createdDateTime</span></span>|<span data-ttu-id="91e87-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91e87-140">DateTimeOffset</span></span>|<span data-ttu-id="91e87-141">Datum und Uhrzeit der Erstellung der E-Book-Datei.</span><span class="sxs-lookup"><span data-stu-id="91e87-141">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="91e87-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="91e87-142">lastModifiedDateTime</span></span>|<span data-ttu-id="91e87-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91e87-143">DateTimeOffset</span></span>|<span data-ttu-id="91e87-144">Datum und Uhrzeit der letzten Änderung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="91e87-144">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="91e87-145">informationUrl</span><span class="sxs-lookup"><span data-stu-id="91e87-145">informationUrl</span></span>|<span data-ttu-id="91e87-146">String</span><span class="sxs-lookup"><span data-stu-id="91e87-146">String</span></span>|<span data-ttu-id="91e87-147">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="91e87-147">The more information Url.</span></span>|
|<span data-ttu-id="91e87-148">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="91e87-148">privacyInformationUrl</span></span>|<span data-ttu-id="91e87-149">String</span><span class="sxs-lookup"><span data-stu-id="91e87-149">String</span></span>|<span data-ttu-id="91e87-150">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="91e87-150">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91e87-151">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="91e87-151">Relationships</span></span>
|<span data-ttu-id="91e87-152">Beziehung</span><span class="sxs-lookup"><span data-stu-id="91e87-152">Relationship</span></span>|<span data-ttu-id="91e87-153">Typ</span><span class="sxs-lookup"><span data-stu-id="91e87-153">Type</span></span>|<span data-ttu-id="91e87-154">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91e87-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91e87-155">assignments</span><span class="sxs-lookup"><span data-stu-id="91e87-155">assignments</span></span>|<span data-ttu-id="91e87-156">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="91e87-156">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) collection</span></span>|<span data-ttu-id="91e87-157">Die Liste der Zuweisungen für dieses E-Book.</span><span class="sxs-lookup"><span data-stu-id="91e87-157">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="91e87-158">installSummary</span><span class="sxs-lookup"><span data-stu-id="91e87-158">installSummary</span></span>|[<span data-ttu-id="91e87-159">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="91e87-159">eBookInstallSummary</span></span>](../resources/intune_books_ebookinstallsummary.md)|<span data-ttu-id="91e87-160">Die Installationszusammenfassung für die mobile App.</span><span class="sxs-lookup"><span data-stu-id="91e87-160">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="91e87-161">deviceStates</span><span class="sxs-lookup"><span data-stu-id="91e87-161">deviceStates</span></span>|<span data-ttu-id="91e87-162">[deviceInstallState](../resources/intune_books_deviceinstallstate.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="91e87-162">[deviceInstallState](../resources/intune_books_deviceinstallstate.md) collection</span></span>|<span data-ttu-id="91e87-163">Die Liste der Installationsstatus für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="91e87-163">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="91e87-164">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="91e87-164">userStateSummary</span></span>|<span data-ttu-id="91e87-165">[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="91e87-165">[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="91e87-166">Die Liste der Installationsstatus für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="91e87-166">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="91e87-167">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="91e87-167">JSON Representation</span></span>
<span data-ttu-id="91e87-168">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="91e87-168">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```



