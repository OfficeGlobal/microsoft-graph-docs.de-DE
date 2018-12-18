---
title: Ressourcentyp „mobileApp“
description: Eine abstrakte Klasse, die grundlegende Eigenschaften von mobilen Intune-Apps enthält
author: tfitzmac
ms.openlocfilehash: 7d28205e532779504b5b9a846e835d4178fc94e9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301540"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="5093c-103">Ressourcentyp „mobileApp“</span><span class="sxs-lookup"><span data-stu-id="5093c-103">mobileApp resource type</span></span>

> <span data-ttu-id="5093c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5093c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5093c-105">Eine abstrakte Klasse, die grundlegende Eigenschaften von mobilen Intune-Apps enthält</span><span class="sxs-lookup"><span data-stu-id="5093c-105">An abstract class containing the base properties for Intune mobile apps.</span></span>
## <a name="methods"></a><span data-ttu-id="5093c-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="5093c-106">Methods</span></span>
|<span data-ttu-id="5093c-107">Methode</span><span class="sxs-lookup"><span data-stu-id="5093c-107">Method</span></span>|<span data-ttu-id="5093c-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="5093c-108">Return Type</span></span>|<span data-ttu-id="5093c-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5093c-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5093c-110">Auflisten von „mobileApp“</span><span class="sxs-lookup"><span data-stu-id="5093c-110">List mobileApps</span></span>](../api/intune-apps-mobileapp-list.md)|<span data-ttu-id="5093c-111">Sammlung von Objekten des Typs [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5093c-111">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="5093c-112">Listet die Eigenschaften und Beziehungen von Objekten des Typs [mobileApp](../resources/intune-apps-mobileapp.md) auf.</span><span class="sxs-lookup"><span data-stu-id="5093c-112">List properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="5093c-113">Abrufen von „mobileApp“</span><span class="sxs-lookup"><span data-stu-id="5093c-113">Get mobileApp</span></span>](../api/intune-apps-mobileapp-get.md)|[<span data-ttu-id="5093c-114">mobileApp</span><span class="sxs-lookup"><span data-stu-id="5093c-114">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="5093c-115">Liest die Eigenschaften und Beziehungen von Objekten des Typs [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5093c-115">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>|
|[<span data-ttu-id="5093c-116">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="5093c-116">assign action</span></span>](../api/intune-apps-mobileapp-assign.md)|<span data-ttu-id="5093c-117">Keine</span><span class="sxs-lookup"><span data-stu-id="5093c-117">None</span></span>|<span data-ttu-id="5093c-118">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="5093c-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5093c-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5093c-119">Properties</span></span>
|<span data-ttu-id="5093c-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5093c-120">Property</span></span>|<span data-ttu-id="5093c-121">Typ</span><span class="sxs-lookup"><span data-stu-id="5093c-121">Type</span></span>|<span data-ttu-id="5093c-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5093c-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5093c-123">id</span><span class="sxs-lookup"><span data-stu-id="5093c-123">id</span></span>|<span data-ttu-id="5093c-124">String</span><span class="sxs-lookup"><span data-stu-id="5093c-124">String</span></span>|<span data-ttu-id="5093c-125">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5093c-125">Key of the entity.</span></span>|
|<span data-ttu-id="5093c-126">displayName</span><span class="sxs-lookup"><span data-stu-id="5093c-126">displayName</span></span>|<span data-ttu-id="5093c-127">String</span><span class="sxs-lookup"><span data-stu-id="5093c-127">String</span></span>|<span data-ttu-id="5093c-128">Titel der App (vom Administrator bereitgestellt oder importiert)</span><span class="sxs-lookup"><span data-stu-id="5093c-128">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="5093c-129">description</span><span class="sxs-lookup"><span data-stu-id="5093c-129">description</span></span>|<span data-ttu-id="5093c-130">String</span><span class="sxs-lookup"><span data-stu-id="5093c-130">String</span></span>|<span data-ttu-id="5093c-131">Beschreibung der App</span><span class="sxs-lookup"><span data-stu-id="5093c-131">The description of the app.</span></span>|
|<span data-ttu-id="5093c-132">publisher</span><span class="sxs-lookup"><span data-stu-id="5093c-132">publisher</span></span>|<span data-ttu-id="5093c-133">String</span><span class="sxs-lookup"><span data-stu-id="5093c-133">String</span></span>|<span data-ttu-id="5093c-134">Herausgeber der App</span><span class="sxs-lookup"><span data-stu-id="5093c-134">The publisher of the app.</span></span>|
|<span data-ttu-id="5093c-135">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5093c-135">largeIcon</span></span>|[<span data-ttu-id="5093c-136">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5093c-136">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5093c-137">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll</span><span class="sxs-lookup"><span data-stu-id="5093c-137">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="5093c-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5093c-138">createdDateTime</span></span>|<span data-ttu-id="5093c-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5093c-139">DateTimeOffset</span></span>|<span data-ttu-id="5093c-140">Datum und Uhrzeit der Erstellung der App</span><span class="sxs-lookup"><span data-stu-id="5093c-140">The date and time the app was created.</span></span>|
|<span data-ttu-id="5093c-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5093c-141">lastModifiedDateTime</span></span>|<span data-ttu-id="5093c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5093c-142">DateTimeOffset</span></span>|<span data-ttu-id="5093c-143">Datum und Uhrzeit der letzten Änderung der App</span><span class="sxs-lookup"><span data-stu-id="5093c-143">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="5093c-144">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5093c-144">isFeatured</span></span>|<span data-ttu-id="5093c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="5093c-145">Boolean</span></span>|<span data-ttu-id="5093c-146">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde</span><span class="sxs-lookup"><span data-stu-id="5093c-146">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="5093c-147">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5093c-147">privacyInformationUrl</span></span>|<span data-ttu-id="5093c-148">String</span><span class="sxs-lookup"><span data-stu-id="5093c-148">String</span></span>|<span data-ttu-id="5093c-149">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="5093c-149">The privacy statement Url.</span></span>|
|<span data-ttu-id="5093c-150">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5093c-150">informationUrl</span></span>|<span data-ttu-id="5093c-151">String</span><span class="sxs-lookup"><span data-stu-id="5093c-151">String</span></span>|<span data-ttu-id="5093c-152">URL zur Seite mit weiteren Informationen</span><span class="sxs-lookup"><span data-stu-id="5093c-152">The more information Url.</span></span>|
|<span data-ttu-id="5093c-153">owner</span><span class="sxs-lookup"><span data-stu-id="5093c-153">owner</span></span>|<span data-ttu-id="5093c-154">String</span><span class="sxs-lookup"><span data-stu-id="5093c-154">String</span></span>|<span data-ttu-id="5093c-155">Besitzer der App</span><span class="sxs-lookup"><span data-stu-id="5093c-155">The owner of the app.</span></span>|
|<span data-ttu-id="5093c-156">developer</span><span class="sxs-lookup"><span data-stu-id="5093c-156">developer</span></span>|<span data-ttu-id="5093c-157">String</span><span class="sxs-lookup"><span data-stu-id="5093c-157">String</span></span>|<span data-ttu-id="5093c-158">Entwickler der App</span><span class="sxs-lookup"><span data-stu-id="5093c-158">The developer of the app.</span></span>|
|<span data-ttu-id="5093c-159">notes</span><span class="sxs-lookup"><span data-stu-id="5093c-159">notes</span></span>|<span data-ttu-id="5093c-160">String</span><span class="sxs-lookup"><span data-stu-id="5093c-160">String</span></span>|<span data-ttu-id="5093c-161">Hinweise zur App</span><span class="sxs-lookup"><span data-stu-id="5093c-161">Notes for the app.</span></span>|
|<span data-ttu-id="5093c-162">publishingState</span><span class="sxs-lookup"><span data-stu-id="5093c-162">publishingState</span></span>|[<span data-ttu-id="5093c-163">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="5093c-163">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="5093c-164">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="5093c-164">The publishing state for the app.</span></span> <span data-ttu-id="5093c-165">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="5093c-165">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5093c-166">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="5093c-166">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5093c-167">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5093c-167">Relationships</span></span>
|<span data-ttu-id="5093c-168">Beziehung</span><span class="sxs-lookup"><span data-stu-id="5093c-168">Relationship</span></span>|<span data-ttu-id="5093c-169">Typ</span><span class="sxs-lookup"><span data-stu-id="5093c-169">Type</span></span>|<span data-ttu-id="5093c-170">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5093c-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5093c-171">categories</span><span class="sxs-lookup"><span data-stu-id="5093c-171">categories</span></span>|<span data-ttu-id="5093c-172">Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="5093c-172">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="5093c-173">Liste der Kategorien, denen die App zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="5093c-173">The list of categories for this app.</span></span>|
|<span data-ttu-id="5093c-174">assignments</span><span class="sxs-lookup"><span data-stu-id="5093c-174">assignments</span></span>|<span data-ttu-id="5093c-175">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="5093c-175">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="5093c-176">Liste der Gruppenzuweisungen für die mobile App</span><span class="sxs-lookup"><span data-stu-id="5093c-176">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5093c-177">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5093c-177">JSON Representation</span></span>
<span data-ttu-id="5093c-178">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5093c-178">Here is a JSON representation of the resource.</span></span>
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



