---
title: mobileLobApp-Ressourcentyp
description: Eine abstrakte Basisklasse mit Eigenschaften für alle mobilen branchenspezifischen Apps.
ms.openlocfilehash: cbfa3d69431f0113e263981053dbeeb176126204
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017858"
---
# <a name="mobilelobapp-resource-type"></a><span data-ttu-id="edf38-103">mobileLobApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="edf38-103">mobileLobApp resource type</span></span>

> <span data-ttu-id="edf38-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="edf38-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="edf38-105">Eine abstrakte Basisklasse mit Eigenschaften für alle mobilen branchenspezifischen Apps.</span><span class="sxs-lookup"><span data-stu-id="edf38-105">An abstract base class containing properties for all mobile line of business apps.</span></span>

<span data-ttu-id="edf38-106">Sie erbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="edf38-106">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="edf38-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="edf38-107">Methods</span></span>
|<span data-ttu-id="edf38-108">Methode</span><span class="sxs-lookup"><span data-stu-id="edf38-108">Method</span></span>|<span data-ttu-id="edf38-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="edf38-109">Return Type</span></span>|<span data-ttu-id="edf38-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="edf38-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="edf38-111">MobileLobApps auflisten</span><span class="sxs-lookup"><span data-stu-id="edf38-111">List mobileLobApps</span></span>](../api/intune-apps-mobilelobapp-list.md)|<span data-ttu-id="edf38-112">[mobileLobApp](../resources/intune-apps-mobilelobapp.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="edf38-112">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) collection</span></span>|<span data-ttu-id="edf38-113">Listet die Eigenschaften und Beziehungen von Objekten des Typs [mobileLobApp](../resources/intune-apps-mobilelobapp.md) auf.</span><span class="sxs-lookup"><span data-stu-id="edf38-113">List properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) objects.</span></span>|
|[<span data-ttu-id="edf38-114">MobileLobApp abrufen</span><span class="sxs-lookup"><span data-stu-id="edf38-114">Get mobileLobApp</span></span>](../api/intune-apps-mobilelobapp-get.md)|[<span data-ttu-id="edf38-115">mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="edf38-115">mobileLobApp</span></span>](../resources/intune-apps-mobilelobapp.md)|<span data-ttu-id="edf38-116">Liest die Eigenschaften und Beziehungen von Objekten des [mobileLobApp](../resources/intune-apps-mobilelobapp.md)-Objekts auf.</span><span class="sxs-lookup"><span data-stu-id="edf38-116">Read properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="edf38-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="edf38-117">Properties</span></span>
|<span data-ttu-id="edf38-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="edf38-118">Property</span></span>|<span data-ttu-id="edf38-119">Typ</span><span class="sxs-lookup"><span data-stu-id="edf38-119">Type</span></span>|<span data-ttu-id="edf38-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="edf38-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edf38-121">id</span><span class="sxs-lookup"><span data-stu-id="edf38-121">id</span></span>|<span data-ttu-id="edf38-122">String</span><span class="sxs-lookup"><span data-stu-id="edf38-122">String</span></span>|<span data-ttu-id="edf38-123">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="edf38-123">Key of the entity.</span></span> <span data-ttu-id="edf38-124">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="edf38-124">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="edf38-125">displayName</span><span class="sxs-lookup"><span data-stu-id="edf38-125">displayName</span></span>|<span data-ttu-id="edf38-126">String</span><span class="sxs-lookup"><span data-stu-id="edf38-126">String</span></span>|<span data-ttu-id="edf38-127">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="edf38-127">The admin provided or imported title of the app.</span></span> <span data-ttu-id="edf38-128">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="edf38-128">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="edf38-129">description</span><span class="sxs-lookup"><span data-stu-id="edf38-129">description</span></span>|<span data-ttu-id="edf38-130">String</span><span class="sxs-lookup"><span data-stu-id="edf38-130">String</span></span>|<span data-ttu-id="edf38-131">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="edf38-131">The description of the app.</span></span> <span data-ttu-id="edf38-132">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="edf38-132">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="edf38-133">publisher</span><span class="sxs-lookup"><span data-stu-id="edf38-133">publisher</span></span>|<span data-ttu-id="edf38-134">String</span><span class="sxs-lookup"><span data-stu-id="edf38-134">String</span></span>|<span data-ttu-id="edf38-135">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="edf38-135">The publisher of the app.</span></span> <span data-ttu-id="edf38-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="edf38-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="edf38-137">largeIcon</span><span class="sxs-lookup"><span data-stu-id="edf38-137">largeIcon</span></span>|[<span data-ttu-id="edf38-138">mimeContent</span><span class="sxs-lookup"><span data-stu-id="edf38-138">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="edf38-139">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="edf38-139">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="edf38-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="edf38-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="edf38-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="edf38-141">createdDateTime</span></span>|<span data-ttu-id="edf38-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edf38-142">DateTimeOffset</span></span>|<span data-ttu-id="edf38-143">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="edf38-143">The date and time the app was created.</span></span> <span data-ttu-id="edf38-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="edf38-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="edf38-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="edf38-145">lastModifiedDateTime</span></span>|<span data-ttu-id="edf38-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edf38-146">DateTimeOffset</span></span>|<span data-ttu-id="edf38-147">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="edf38-147">The date and time the app was last modified.</span></span> <span data-ttu-id="edf38-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="edf38-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="edf38-149">isFeatured</span><span class="sxs-lookup"><span data-stu-id="edf38-149">isFeatured</span></span>|<span data-ttu-id="edf38-150">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="edf38-150">Boolean</span></span>|<span data-ttu-id="edf38-151">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="edf38-151">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="edf38-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="edf38-152">privacyInformationUrl</span></span>|<span data-ttu-id="edf38-153">String</span><span class="sxs-lookup"><span data-stu-id="edf38-153">String</span></span>|<span data-ttu-id="edf38-154">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="edf38-154">The privacy statement Url.</span></span> <span data-ttu-id="edf38-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="edf38-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="edf38-156">informationUrl</span><span class="sxs-lookup"><span data-stu-id="edf38-156">informationUrl</span></span>|<span data-ttu-id="edf38-157">String</span><span class="sxs-lookup"><span data-stu-id="edf38-157">String</span></span>|<span data-ttu-id="edf38-158">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="edf38-158">The more information Url.</span></span> <span data-ttu-id="edf38-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="edf38-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="edf38-160">owner</span><span class="sxs-lookup"><span data-stu-id="edf38-160">owner</span></span>|<span data-ttu-id="edf38-161">String</span><span class="sxs-lookup"><span data-stu-id="edf38-161">String</span></span>|<span data-ttu-id="edf38-162">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="edf38-162">The owner of the app.</span></span> <span data-ttu-id="edf38-163">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="edf38-163">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="edf38-164">developer</span><span class="sxs-lookup"><span data-stu-id="edf38-164">developer</span></span>|<span data-ttu-id="edf38-165">String</span><span class="sxs-lookup"><span data-stu-id="edf38-165">String</span></span>|<span data-ttu-id="edf38-166">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="edf38-166">The developer of the app.</span></span> <span data-ttu-id="edf38-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="edf38-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="edf38-168">notes</span><span class="sxs-lookup"><span data-stu-id="edf38-168">notes</span></span>|<span data-ttu-id="edf38-169">String</span><span class="sxs-lookup"><span data-stu-id="edf38-169">String</span></span>|<span data-ttu-id="edf38-170">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="edf38-170">Notes for the app.</span></span> <span data-ttu-id="edf38-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="edf38-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="edf38-172">publishingState</span><span class="sxs-lookup"><span data-stu-id="edf38-172">publishingState</span></span>|[<span data-ttu-id="edf38-173">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="edf38-173">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="edf38-174">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="edf38-174">The publishing state for the app.</span></span> <span data-ttu-id="edf38-175">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="edf38-175">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="edf38-176">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="edf38-176">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="edf38-177">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="edf38-177">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="edf38-178">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="edf38-178">committedContentVersion</span></span>|<span data-ttu-id="edf38-179">String</span><span class="sxs-lookup"><span data-stu-id="edf38-179">String</span></span>|<span data-ttu-id="edf38-180">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="edf38-180">The internal committed content version.</span></span>|
|<span data-ttu-id="edf38-181">fileName</span><span class="sxs-lookup"><span data-stu-id="edf38-181">fileName</span></span>|<span data-ttu-id="edf38-182">String</span><span class="sxs-lookup"><span data-stu-id="edf38-182">String</span></span>|<span data-ttu-id="edf38-183">Der Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="edf38-183">The name of the main Lob application file.</span></span>|
|<span data-ttu-id="edf38-184">size</span><span class="sxs-lookup"><span data-stu-id="edf38-184">size</span></span>|<span data-ttu-id="edf38-185">Int64</span><span class="sxs-lookup"><span data-stu-id="edf38-185">Int64</span></span>|<span data-ttu-id="edf38-186">Die Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="edf38-186">The total size, including all uploaded files.</span></span>|

## <a name="relationships"></a><span data-ttu-id="edf38-187">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="edf38-187">Relationships</span></span>
|<span data-ttu-id="edf38-188">Beziehung</span><span class="sxs-lookup"><span data-stu-id="edf38-188">Relationship</span></span>|<span data-ttu-id="edf38-189">Typ</span><span class="sxs-lookup"><span data-stu-id="edf38-189">Type</span></span>|<span data-ttu-id="edf38-190">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="edf38-190">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edf38-191">categories</span><span class="sxs-lookup"><span data-stu-id="edf38-191">categories</span></span>|<span data-ttu-id="edf38-192">Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="edf38-192">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="edf38-193">Die Liste der Kategorien für diese App.</span><span class="sxs-lookup"><span data-stu-id="edf38-193">The list of categories for this app.</span></span> <span data-ttu-id="edf38-194">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="edf38-194">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="edf38-195">assignments</span><span class="sxs-lookup"><span data-stu-id="edf38-195">assignments</span></span>|<span data-ttu-id="edf38-196">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="edf38-196">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="edf38-197">Die Liste von Gruppenzuweisungen für diese mobile App.</span><span class="sxs-lookup"><span data-stu-id="edf38-197">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="edf38-198">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="edf38-198">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="edf38-199">contentVersions</span><span class="sxs-lookup"><span data-stu-id="edf38-199">contentVersions</span></span>|<span data-ttu-id="edf38-200">Sammlung von Objekten des Typs [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="edf38-200">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="edf38-201">Die Liste der Inhaltsversionen für diese App.</span><span class="sxs-lookup"><span data-stu-id="edf38-201">The list of content versions for this app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="edf38-202">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="edf38-202">JSON Representation</span></span>
<span data-ttu-id="edf38-203">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="edf38-203">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileLobApp",
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
  "publishingState": "String",
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024
}
```


