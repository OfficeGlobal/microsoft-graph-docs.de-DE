# <a name="mobileapp-resource-type"></a><span data-ttu-id="aaecb-101">Ressourcentyp „mobileApp“</span><span class="sxs-lookup"><span data-stu-id="aaecb-101">mobileApp resource type</span></span>

> <span data-ttu-id="aaecb-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="aaecb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aaecb-103">Eine abstrakte Klasse, die grundlegende Eigenschaften von mobilen Intune-Apps enthält</span><span class="sxs-lookup"><span data-stu-id="aaecb-103">An abstract class containing the base properties for Intune mobile apps.</span></span>
## <a name="methods"></a><span data-ttu-id="aaecb-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="aaecb-104">Methods</span></span>
|<span data-ttu-id="aaecb-105">Methode</span><span class="sxs-lookup"><span data-stu-id="aaecb-105">Method</span></span>|<span data-ttu-id="aaecb-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="aaecb-106">Return Type</span></span>|<span data-ttu-id="aaecb-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aaecb-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aaecb-108">Auflisten von „mobileApp“</span><span class="sxs-lookup"><span data-stu-id="aaecb-108">List mobileApps</span></span>](../api/intune_apps_mobileapp_list.md)|<span data-ttu-id="aaecb-109">Sammlung von Objekten des Typs [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="aaecb-109">[mobileApp](../resources/intune_apps_mobileapp.md) collection</span></span>|<span data-ttu-id="aaecb-110">Listet die Eigenschaften und Beziehungen von Objekten des Typs [mobileApp](../resources/intune_apps_mobileapp.md) auf.</span><span class="sxs-lookup"><span data-stu-id="aaecb-110">List properties and relationships of the [mobileApp](../resources/intune_apps_mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="aaecb-111">Abrufen von „mobileApp“</span><span class="sxs-lookup"><span data-stu-id="aaecb-111">Get mobileApp</span></span>](../api/intune_apps_mobileapp_get.md)|[<span data-ttu-id="aaecb-112">mobileApp</span><span class="sxs-lookup"><span data-stu-id="aaecb-112">mobileApp</span></span>](../resources/intune_apps_mobileapp.md)|<span data-ttu-id="aaecb-113">Liest die Eigenschaften und Beziehungen von Objekten des Typs [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="aaecb-113">Read properties and relationships of the [mobileApp](../resources/intune_apps_mobileapp.md) object.</span></span>|
|[<span data-ttu-id="aaecb-114">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="aaecb-114">assign action</span></span>](../api/intune_apps_mobileapp_assign.md)|<span data-ttu-id="aaecb-115">Keiner</span><span class="sxs-lookup"><span data-stu-id="aaecb-115">None</span></span>|<span data-ttu-id="aaecb-116">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="aaecb-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="aaecb-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="aaecb-117">Properties</span></span>
|<span data-ttu-id="aaecb-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aaecb-118">Property</span></span>|<span data-ttu-id="aaecb-119">Typ</span><span class="sxs-lookup"><span data-stu-id="aaecb-119">Type</span></span>|<span data-ttu-id="aaecb-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aaecb-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aaecb-121">id</span><span class="sxs-lookup"><span data-stu-id="aaecb-121">id</span></span>|<span data-ttu-id="aaecb-122">String</span><span class="sxs-lookup"><span data-stu-id="aaecb-122">String</span></span>|<span data-ttu-id="aaecb-123">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="aaecb-123">Key of the entity.</span></span>|
|<span data-ttu-id="aaecb-124">displayName</span><span class="sxs-lookup"><span data-stu-id="aaecb-124">displayName</span></span>|<span data-ttu-id="aaecb-125">String</span><span class="sxs-lookup"><span data-stu-id="aaecb-125">String</span></span>|<span data-ttu-id="aaecb-126">Titel der App (vom Administrator bereitgestellt oder importiert)</span><span class="sxs-lookup"><span data-stu-id="aaecb-126">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="aaecb-127">description</span><span class="sxs-lookup"><span data-stu-id="aaecb-127">description</span></span>|<span data-ttu-id="aaecb-128">String</span><span class="sxs-lookup"><span data-stu-id="aaecb-128">String</span></span>|<span data-ttu-id="aaecb-129">Beschreibung der App</span><span class="sxs-lookup"><span data-stu-id="aaecb-129">The description of the app.</span></span>|
|<span data-ttu-id="aaecb-130">publisher</span><span class="sxs-lookup"><span data-stu-id="aaecb-130">publisher</span></span>|<span data-ttu-id="aaecb-131">String</span><span class="sxs-lookup"><span data-stu-id="aaecb-131">String</span></span>|<span data-ttu-id="aaecb-132">Herausgeber der App</span><span class="sxs-lookup"><span data-stu-id="aaecb-132">The publisher of the app.</span></span>|
|<span data-ttu-id="aaecb-133">largeIcon</span><span class="sxs-lookup"><span data-stu-id="aaecb-133">largeIcon</span></span>|[<span data-ttu-id="aaecb-134">mimeContent</span><span class="sxs-lookup"><span data-stu-id="aaecb-134">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="aaecb-135">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll</span><span class="sxs-lookup"><span data-stu-id="aaecb-135">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="aaecb-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aaecb-136">createdDateTime</span></span>|<span data-ttu-id="aaecb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aaecb-137">DateTimeOffset</span></span>|<span data-ttu-id="aaecb-138">Datum und Uhrzeit der Erstellung der App</span><span class="sxs-lookup"><span data-stu-id="aaecb-138">The date and time the app was created.</span></span>|
|<span data-ttu-id="aaecb-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aaecb-139">lastModifiedDateTime</span></span>|<span data-ttu-id="aaecb-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aaecb-140">DateTimeOffset</span></span>|<span data-ttu-id="aaecb-141">Datum und Uhrzeit der letzten Änderung der App</span><span class="sxs-lookup"><span data-stu-id="aaecb-141">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="aaecb-142">isFeatured</span><span class="sxs-lookup"><span data-stu-id="aaecb-142">isFeatured</span></span>|<span data-ttu-id="aaecb-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="aaecb-143">Boolean</span></span>|<span data-ttu-id="aaecb-144">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde</span><span class="sxs-lookup"><span data-stu-id="aaecb-144">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="aaecb-145">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="aaecb-145">privacyInformationUrl</span></span>|<span data-ttu-id="aaecb-146">String</span><span class="sxs-lookup"><span data-stu-id="aaecb-146">String</span></span>|<span data-ttu-id="aaecb-147">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="aaecb-147">The privacy statement Url.</span></span>|
|<span data-ttu-id="aaecb-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="aaecb-148">informationUrl</span></span>|<span data-ttu-id="aaecb-149">String</span><span class="sxs-lookup"><span data-stu-id="aaecb-149">String</span></span>|<span data-ttu-id="aaecb-150">URL zur Seite mit weiteren Informationen</span><span class="sxs-lookup"><span data-stu-id="aaecb-150">The more information Url.</span></span>|
|<span data-ttu-id="aaecb-151">owner</span><span class="sxs-lookup"><span data-stu-id="aaecb-151">owner</span></span>|<span data-ttu-id="aaecb-152">String</span><span class="sxs-lookup"><span data-stu-id="aaecb-152">String</span></span>|<span data-ttu-id="aaecb-153">Besitzer der App</span><span class="sxs-lookup"><span data-stu-id="aaecb-153">The owner of the app.</span></span>|
|<span data-ttu-id="aaecb-154">developer</span><span class="sxs-lookup"><span data-stu-id="aaecb-154">developer</span></span>|<span data-ttu-id="aaecb-155">String</span><span class="sxs-lookup"><span data-stu-id="aaecb-155">String</span></span>|<span data-ttu-id="aaecb-156">Entwickler der App</span><span class="sxs-lookup"><span data-stu-id="aaecb-156">The developer of the app.</span></span>|
|<span data-ttu-id="aaecb-157">notes</span><span class="sxs-lookup"><span data-stu-id="aaecb-157">notes</span></span>|<span data-ttu-id="aaecb-158">String</span><span class="sxs-lookup"><span data-stu-id="aaecb-158">String</span></span>|<span data-ttu-id="aaecb-159">Hinweise zur App</span><span class="sxs-lookup"><span data-stu-id="aaecb-159">Notes for the app.</span></span>|
|<span data-ttu-id="aaecb-160">publishingState</span><span class="sxs-lookup"><span data-stu-id="aaecb-160">publishingState</span></span>|[<span data-ttu-id="aaecb-161">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="aaecb-161">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="aaecb-162">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="aaecb-162">The publishing state for the app.</span></span> <span data-ttu-id="aaecb-163">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="aaecb-163">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="aaecb-164">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="aaecb-164">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aaecb-165">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="aaecb-165">Relationships</span></span>
|<span data-ttu-id="aaecb-166">Beziehung</span><span class="sxs-lookup"><span data-stu-id="aaecb-166">Relationship</span></span>|<span data-ttu-id="aaecb-167">Typ</span><span class="sxs-lookup"><span data-stu-id="aaecb-167">Type</span></span>|<span data-ttu-id="aaecb-168">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aaecb-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aaecb-169">categories</span><span class="sxs-lookup"><span data-stu-id="aaecb-169">categories</span></span>|<span data-ttu-id="aaecb-170">Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="aaecb-170">[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) collection</span></span>|<span data-ttu-id="aaecb-171">Liste der Kategorien, denen die App zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="aaecb-171">The list of categories for this app.</span></span>|
|<span data-ttu-id="aaecb-172">assignments</span><span class="sxs-lookup"><span data-stu-id="aaecb-172">assignments</span></span>|<span data-ttu-id="aaecb-173">Sammlung von Objekten des Typs [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="aaecb-173">[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) collection</span></span>|<span data-ttu-id="aaecb-174">Liste der Gruppenzuweisungen für die mobile App</span><span class="sxs-lookup"><span data-stu-id="aaecb-174">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aaecb-175">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="aaecb-175">JSON Representation</span></span>
<span data-ttu-id="aaecb-176">Unten sehen Sie eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="aaecb-176">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "publishingState": "String"
}
```



