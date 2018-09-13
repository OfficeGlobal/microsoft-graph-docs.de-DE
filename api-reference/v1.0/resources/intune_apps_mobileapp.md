# <a name="mobileapp-resource-type"></a><span data-ttu-id="b4200-101">Ressourcentyp „mobileApp“</span><span class="sxs-lookup"><span data-stu-id="b4200-101">mobileApp resource type</span></span>

> <span data-ttu-id="b4200-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b4200-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4200-103">Eine abstrakte Klasse, die grundlegende Eigenschaften von mobilen Intune-Apps enthält</span><span class="sxs-lookup"><span data-stu-id="b4200-103">An abstract class containing the base properties for Intune mobile apps.</span></span>
## <a name="methods"></a><span data-ttu-id="b4200-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="b4200-104">Methods</span></span>
|<span data-ttu-id="b4200-105">Methode</span><span class="sxs-lookup"><span data-stu-id="b4200-105">Method</span></span>|<span data-ttu-id="b4200-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b4200-106">Return Type</span></span>|<span data-ttu-id="b4200-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4200-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b4200-108">Auflisten von „mobileApp“</span><span class="sxs-lookup"><span data-stu-id="b4200-108">List mobileApps</span></span>](../api/intune_apps_mobileapp_list.md)|<span data-ttu-id="b4200-109">Sammlung von Objekten des Typs [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4200-109">[mobileApp](../resources/intune_apps_mobileapp.md) collection</span></span>|<span data-ttu-id="b4200-110">Listet die Eigenschaften und Beziehungen von Objekten des Typs [mobileApp](../resources/intune_apps_mobileapp.md) auf.</span><span class="sxs-lookup"><span data-stu-id="b4200-110">List properties and relationships of the [mobileApp](../resources/intune_apps_mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="b4200-111">Abrufen von „mobileApp“</span><span class="sxs-lookup"><span data-stu-id="b4200-111">Get mobileApp</span></span>](../api/intune_apps_mobileapp_get.md)|[<span data-ttu-id="b4200-112">mobileApp</span><span class="sxs-lookup"><span data-stu-id="b4200-112">mobileApp</span></span>](../resources/intune_apps_mobileapp.md)|<span data-ttu-id="b4200-113">Liest die Eigenschaften und Beziehungen von Objekten des Typs [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4200-113">Read properties and relationships of the [mobileApp](../resources/intune_apps_mobileapp.md) object.</span></span>|
|[<span data-ttu-id="b4200-114">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="b4200-114">assign action</span></span>](../api/intune_apps_mobileapp_assign.md)|<span data-ttu-id="b4200-115">Keine</span><span class="sxs-lookup"><span data-stu-id="b4200-115">None</span></span>|<span data-ttu-id="b4200-116">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b4200-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="b4200-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b4200-117">Properties</span></span>
|<span data-ttu-id="b4200-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b4200-118">Property</span></span>|<span data-ttu-id="b4200-119">Typ</span><span class="sxs-lookup"><span data-stu-id="b4200-119">Type</span></span>|<span data-ttu-id="b4200-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4200-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4200-121">id</span><span class="sxs-lookup"><span data-stu-id="b4200-121">id</span></span>|<span data-ttu-id="b4200-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4200-122">String</span></span>|<span data-ttu-id="b4200-123">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b4200-123">Key of the entity.</span></span>|
|<span data-ttu-id="b4200-124">displayName</span><span class="sxs-lookup"><span data-stu-id="b4200-124">displayName</span></span>|<span data-ttu-id="b4200-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4200-125">String</span></span>|<span data-ttu-id="b4200-126">Titel der App (vom Administrator bereitgestellt oder importiert)</span><span class="sxs-lookup"><span data-stu-id="b4200-126">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="b4200-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4200-127">description</span></span>|<span data-ttu-id="b4200-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4200-128">String</span></span>|<span data-ttu-id="b4200-129">Beschreibung der App</span><span class="sxs-lookup"><span data-stu-id="b4200-129">The description of the app.</span></span>|
|<span data-ttu-id="b4200-130">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="b4200-130">publisher</span></span>|<span data-ttu-id="b4200-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4200-131">String</span></span>|<span data-ttu-id="b4200-132">Herausgeber der App</span><span class="sxs-lookup"><span data-stu-id="b4200-132">The publisher of the app.</span></span>|
|<span data-ttu-id="b4200-133">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b4200-133">largeIcon</span></span>|[<span data-ttu-id="b4200-134">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b4200-134">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="b4200-135">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll</span><span class="sxs-lookup"><span data-stu-id="b4200-135">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="b4200-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b4200-136">createdDateTime</span></span>|<span data-ttu-id="b4200-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4200-137">DateTimeOffset</span></span>|<span data-ttu-id="b4200-138">Datum und Uhrzeit der Erstellung der App</span><span class="sxs-lookup"><span data-stu-id="b4200-138">The date and time the app was created.</span></span>|
|<span data-ttu-id="b4200-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4200-139">lastModifiedDateTime</span></span>|<span data-ttu-id="b4200-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4200-140">DateTimeOffset</span></span>|<span data-ttu-id="b4200-141">Datum und Uhrzeit der letzten Änderung der App</span><span class="sxs-lookup"><span data-stu-id="b4200-141">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="b4200-142">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b4200-142">isFeatured</span></span>|<span data-ttu-id="b4200-143">boolesch</span><span class="sxs-lookup"><span data-stu-id="b4200-143">Boolean</span></span>|<span data-ttu-id="b4200-144">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde</span><span class="sxs-lookup"><span data-stu-id="b4200-144">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="b4200-145">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b4200-145">privacyInformationUrl</span></span>|<span data-ttu-id="b4200-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4200-146">String</span></span>|<span data-ttu-id="b4200-147">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="b4200-147">The privacy statement Url.</span></span>|
|<span data-ttu-id="b4200-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b4200-148">informationUrl</span></span>|<span data-ttu-id="b4200-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4200-149">String</span></span>|<span data-ttu-id="b4200-150">URL zur Seite mit weiteren Informationen</span><span class="sxs-lookup"><span data-stu-id="b4200-150">The more information Url.</span></span>|
|<span data-ttu-id="b4200-151">Besitzer</span><span class="sxs-lookup"><span data-stu-id="b4200-151">owner</span></span>|<span data-ttu-id="b4200-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4200-152">String</span></span>|<span data-ttu-id="b4200-153">Besitzer der App</span><span class="sxs-lookup"><span data-stu-id="b4200-153">The owner of the app.</span></span>|
|<span data-ttu-id="b4200-154">Entwickler</span><span class="sxs-lookup"><span data-stu-id="b4200-154">developer</span></span>|<span data-ttu-id="b4200-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4200-155">String</span></span>|<span data-ttu-id="b4200-156">Entwickler der App</span><span class="sxs-lookup"><span data-stu-id="b4200-156">The developer of the app.</span></span>|
|<span data-ttu-id="b4200-157">Notizen</span><span class="sxs-lookup"><span data-stu-id="b4200-157">notes</span></span>|<span data-ttu-id="b4200-158">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b4200-158">String</span></span>|<span data-ttu-id="b4200-159">Hinweise zur App</span><span class="sxs-lookup"><span data-stu-id="b4200-159">Notes for the app.</span></span>|
|<span data-ttu-id="b4200-160">publishingState</span><span class="sxs-lookup"><span data-stu-id="b4200-160">publishingState</span></span>|[<span data-ttu-id="b4200-161">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b4200-161">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="b4200-p101">Der Status der Veröffentlichung einer App. Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde. Mögliche Werte sind: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b4200-p101">The publishing state for the app. The app cannot be assigned unless the app is published. The possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4200-165">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b4200-165">Relationships</span></span>
|<span data-ttu-id="b4200-166">Beziehung</span><span class="sxs-lookup"><span data-stu-id="b4200-166">Relationship</span></span>|<span data-ttu-id="b4200-167">Typ</span><span class="sxs-lookup"><span data-stu-id="b4200-167">Type</span></span>|<span data-ttu-id="b4200-168">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4200-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4200-169">Kategorien</span><span class="sxs-lookup"><span data-stu-id="b4200-169">categories</span></span>|<span data-ttu-id="b4200-170">Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="b4200-170">[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) collection</span></span>|<span data-ttu-id="b4200-171">Liste der Kategorien, denen die App zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="b4200-171">The list of categories for this app.</span></span>|
|<span data-ttu-id="b4200-172">Aufgaben</span><span class="sxs-lookup"><span data-stu-id="b4200-172">assignments</span></span>|<span data-ttu-id="b4200-173">[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="b4200-173">[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) collection</span></span>|<span data-ttu-id="b4200-174">Liste der Gruppenzuweisungen für die mobile App</span><span class="sxs-lookup"><span data-stu-id="b4200-174">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b4200-175">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b4200-175">JSON Representation</span></span>
<span data-ttu-id="b4200-176">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b4200-176">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
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








