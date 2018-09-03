# <a name="mobileapp-resource-type"></a><span data-ttu-id="65870-101">Ressourcentyp „mobileApp“</span><span class="sxs-lookup"><span data-stu-id="65870-101">mobileApp resource type</span></span>

> <span data-ttu-id="65870-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="65870-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65870-103">Eine abstrakte Klasse, die grundlegende Eigenschaften von mobilen Intune-Apps enthält</span><span class="sxs-lookup"><span data-stu-id="65870-103">An abstract class containing the base properties for Intune mobile apps.</span></span>
## <a name="methods"></a><span data-ttu-id="65870-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="65870-104">Methods</span></span>
|<span data-ttu-id="65870-105">Methode</span><span class="sxs-lookup"><span data-stu-id="65870-105">Method</span></span>|<span data-ttu-id="65870-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="65870-106">Return Type</span></span>|<span data-ttu-id="65870-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65870-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="65870-108">Auflisten von „mobileApp“</span><span class="sxs-lookup"><span data-stu-id="65870-108">List mobileApps</span></span>](../api/intune_apps_mobileapp_list.md)|<span data-ttu-id="65870-109">Sammlung von Objekten des Typs [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="65870-109">[mobileApp](../resources/intune_apps_mobileapp.md) collection</span></span>|<span data-ttu-id="65870-110">Listet die Eigenschaften und Beziehungen von Objekten des Typs [mobileApp](../resources/intune_apps_mobileapp.md) auf.</span><span class="sxs-lookup"><span data-stu-id="65870-110">List properties and relationships of the [mobileApp](../resources/intune_apps_mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="65870-111">Abrufen von „mobileApp“</span><span class="sxs-lookup"><span data-stu-id="65870-111">Get mobileApp</span></span>](../api/intune_apps_mobileapp_get.md)|[<span data-ttu-id="65870-112">mobileApp</span><span class="sxs-lookup"><span data-stu-id="65870-112">mobileApp</span></span>](../resources/intune_apps_mobileapp.md)|<span data-ttu-id="65870-113">Liest die Eigenschaften und Beziehungen von Objekten des Typs [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="65870-113">Read properties and relationships of the [mobileApp](../resources/intune_apps_mobileapp.md) object.</span></span>|
|[<span data-ttu-id="65870-114">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="65870-114">assign action</span></span>](../api/intune_apps_mobileapp_assign.md)|<span data-ttu-id="65870-115">Keine</span><span class="sxs-lookup"><span data-stu-id="65870-115">None</span></span>|<span data-ttu-id="65870-116">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="65870-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="65870-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="65870-117">Properties</span></span>
|<span data-ttu-id="65870-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="65870-118">Property</span></span>|<span data-ttu-id="65870-119">Typ</span><span class="sxs-lookup"><span data-stu-id="65870-119">Type</span></span>|<span data-ttu-id="65870-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65870-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65870-121">id</span><span class="sxs-lookup"><span data-stu-id="65870-121">id</span></span>|<span data-ttu-id="65870-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="65870-122">String</span></span>|<span data-ttu-id="65870-123">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="65870-123">Key of the entity.</span></span>|
|<span data-ttu-id="65870-124">displayName</span><span class="sxs-lookup"><span data-stu-id="65870-124">displayName</span></span>|<span data-ttu-id="65870-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="65870-125">String</span></span>|<span data-ttu-id="65870-126">Titel der App (vom Administrator bereitgestellt oder importiert)</span><span class="sxs-lookup"><span data-stu-id="65870-126">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="65870-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65870-127">description</span></span>|<span data-ttu-id="65870-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="65870-128">String</span></span>|<span data-ttu-id="65870-129">Beschreibung der App</span><span class="sxs-lookup"><span data-stu-id="65870-129">The description of the app.</span></span>|
|<span data-ttu-id="65870-130">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="65870-130">publisher</span></span>|<span data-ttu-id="65870-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="65870-131">String</span></span>|<span data-ttu-id="65870-132">Herausgeber der App</span><span class="sxs-lookup"><span data-stu-id="65870-132">The publisher of the app.</span></span>|
|<span data-ttu-id="65870-133">largeIcon</span><span class="sxs-lookup"><span data-stu-id="65870-133">largeIcon</span></span>|[<span data-ttu-id="65870-134">mimeContent</span><span class="sxs-lookup"><span data-stu-id="65870-134">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="65870-135">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll</span><span class="sxs-lookup"><span data-stu-id="65870-135">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="65870-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="65870-136">createdDateTime</span></span>|<span data-ttu-id="65870-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65870-137">DateTimeOffset</span></span>|<span data-ttu-id="65870-138">Datum und Uhrzeit der Erstellung der App</span><span class="sxs-lookup"><span data-stu-id="65870-138">The date and time the app was created.</span></span>|
|<span data-ttu-id="65870-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="65870-139">lastModifiedDateTime</span></span>|<span data-ttu-id="65870-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65870-140">DateTimeOffset</span></span>|<span data-ttu-id="65870-141">Datum und Uhrzeit der letzten Änderung der App</span><span class="sxs-lookup"><span data-stu-id="65870-141">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="65870-142">isFeatured</span><span class="sxs-lookup"><span data-stu-id="65870-142">isFeatured</span></span>|<span data-ttu-id="65870-143">boolesch</span><span class="sxs-lookup"><span data-stu-id="65870-143">Boolean</span></span>|<span data-ttu-id="65870-144">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde</span><span class="sxs-lookup"><span data-stu-id="65870-144">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="65870-145">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="65870-145">privacyInformationUrl</span></span>|<span data-ttu-id="65870-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="65870-146">String</span></span>|<span data-ttu-id="65870-147">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="65870-147">The privacy statement Url.</span></span>|
|<span data-ttu-id="65870-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="65870-148">informationUrl</span></span>|<span data-ttu-id="65870-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="65870-149">String</span></span>|<span data-ttu-id="65870-150">URL zur Seite mit weiteren Informationen</span><span class="sxs-lookup"><span data-stu-id="65870-150">The more information Url.</span></span>|
|<span data-ttu-id="65870-151">Besitzer</span><span class="sxs-lookup"><span data-stu-id="65870-151">owner</span></span>|<span data-ttu-id="65870-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="65870-152">String</span></span>|<span data-ttu-id="65870-153">Besitzer der App</span><span class="sxs-lookup"><span data-stu-id="65870-153">The owner of the app.</span></span>|
|<span data-ttu-id="65870-154">Entwickler</span><span class="sxs-lookup"><span data-stu-id="65870-154">developer</span></span>|<span data-ttu-id="65870-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="65870-155">String</span></span>|<span data-ttu-id="65870-156">Entwickler der App</span><span class="sxs-lookup"><span data-stu-id="65870-156">The developer of the app.</span></span>|
|<span data-ttu-id="65870-157">Notizen</span><span class="sxs-lookup"><span data-stu-id="65870-157">notes</span></span>|<span data-ttu-id="65870-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="65870-158">String</span></span>|<span data-ttu-id="65870-159">Hinweise zur App</span><span class="sxs-lookup"><span data-stu-id="65870-159">Notes for the app.</span></span>|
|<span data-ttu-id="65870-160">publishingState</span><span class="sxs-lookup"><span data-stu-id="65870-160">publishingState</span></span>|[<span data-ttu-id="65870-161">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="65870-161">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="65870-162">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="65870-162">The publishing state for the app.</span></span> <span data-ttu-id="65870-163">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="65870-163">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="65870-164">Mögliche Werte sind:`notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="65870-164">The possible values are `notPublished`, `processing`, `published`, , , , , , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="65870-165">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="65870-165">Relationships</span></span>
|<span data-ttu-id="65870-166">Beziehung</span><span class="sxs-lookup"><span data-stu-id="65870-166">Relationship</span></span>|<span data-ttu-id="65870-167">Typ</span><span class="sxs-lookup"><span data-stu-id="65870-167">Type</span></span>|<span data-ttu-id="65870-168">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65870-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65870-169">Kategorien</span><span class="sxs-lookup"><span data-stu-id="65870-169">categories</span></span>|<span data-ttu-id="65870-170">Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="65870-170">[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) collection</span></span>|<span data-ttu-id="65870-171">Liste der Kategorien, denen die App zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="65870-171">The list of categories for this app.</span></span>|
|<span data-ttu-id="65870-172">Aufgaben</span><span class="sxs-lookup"><span data-stu-id="65870-172">assignments</span></span>|<span data-ttu-id="65870-173">[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="65870-173">[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) collection</span></span>|<span data-ttu-id="65870-174">Liste der Gruppenzuweisungen für die mobile App</span><span class="sxs-lookup"><span data-stu-id="65870-174">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65870-175">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="65870-175">JSON Representation</span></span>
<span data-ttu-id="65870-176">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="65870-176">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "abstract": true,
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.mobileApp"
}-->
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



