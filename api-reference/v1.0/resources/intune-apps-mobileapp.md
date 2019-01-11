---
title: Ressourcentyp „mobileApp“
description: Eine abstrakte Klasse, die grundlegende Eigenschaften von mobilen Intune-Apps enthält
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aac7045bb446956b4df415a96e5c4a7b9cbbbbae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806615"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="63431-103">Ressourcentyp „mobileApp“</span><span class="sxs-lookup"><span data-stu-id="63431-103">mobileApp resource type</span></span>

> <span data-ttu-id="63431-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="63431-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63431-105">Eine abstrakte Klasse, die grundlegende Eigenschaften von mobilen Intune-Apps enthält</span><span class="sxs-lookup"><span data-stu-id="63431-105">An abstract class containing the base properties for Intune mobile apps.</span></span>
## <a name="methods"></a><span data-ttu-id="63431-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="63431-106">Methods</span></span>
|<span data-ttu-id="63431-107">Methode</span><span class="sxs-lookup"><span data-stu-id="63431-107">Method</span></span>|<span data-ttu-id="63431-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="63431-108">Return Type</span></span>|<span data-ttu-id="63431-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="63431-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="63431-110">Auflisten von „mobileApp“</span><span class="sxs-lookup"><span data-stu-id="63431-110">List mobileApps</span></span>](../api/intune-apps-mobileapp-list.md)|<span data-ttu-id="63431-111">Sammlung von Objekten des Typs [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="63431-111">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="63431-112">Listet die Eigenschaften und Beziehungen von Objekten des Typs [mobileApp](../resources/intune-apps-mobileapp.md) auf.</span><span class="sxs-lookup"><span data-stu-id="63431-112">List properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="63431-113">Abrufen von „mobileApp“</span><span class="sxs-lookup"><span data-stu-id="63431-113">Get mobileApp</span></span>](../api/intune-apps-mobileapp-get.md)|[<span data-ttu-id="63431-114">mobileApp</span><span class="sxs-lookup"><span data-stu-id="63431-114">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="63431-115">Liest die Eigenschaften und Beziehungen von Objekten des Typs [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="63431-115">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>|
|[<span data-ttu-id="63431-116">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="63431-116">assign action</span></span>](../api/intune-apps-mobileapp-assign.md)|<span data-ttu-id="63431-117">Keine</span><span class="sxs-lookup"><span data-stu-id="63431-117">None</span></span>|<span data-ttu-id="63431-118">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="63431-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="63431-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="63431-119">Properties</span></span>
|<span data-ttu-id="63431-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="63431-120">Property</span></span>|<span data-ttu-id="63431-121">Typ</span><span class="sxs-lookup"><span data-stu-id="63431-121">Type</span></span>|<span data-ttu-id="63431-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="63431-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63431-123">id</span><span class="sxs-lookup"><span data-stu-id="63431-123">id</span></span>|<span data-ttu-id="63431-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="63431-124">String</span></span>|<span data-ttu-id="63431-125">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="63431-125">Key of the entity.</span></span>|
|<span data-ttu-id="63431-126">displayName</span><span class="sxs-lookup"><span data-stu-id="63431-126">displayName</span></span>|<span data-ttu-id="63431-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="63431-127">String</span></span>|<span data-ttu-id="63431-128">Titel der App (vom Administrator bereitgestellt oder importiert)</span><span class="sxs-lookup"><span data-stu-id="63431-128">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="63431-129">description</span><span class="sxs-lookup"><span data-stu-id="63431-129">description</span></span>|<span data-ttu-id="63431-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="63431-130">String</span></span>|<span data-ttu-id="63431-131">Beschreibung der App</span><span class="sxs-lookup"><span data-stu-id="63431-131">The description of the app.</span></span>|
|<span data-ttu-id="63431-132">publisher</span><span class="sxs-lookup"><span data-stu-id="63431-132">publisher</span></span>|<span data-ttu-id="63431-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="63431-133">String</span></span>|<span data-ttu-id="63431-134">Herausgeber der App</span><span class="sxs-lookup"><span data-stu-id="63431-134">The publisher of the app.</span></span>|
|<span data-ttu-id="63431-135">largeIcon</span><span class="sxs-lookup"><span data-stu-id="63431-135">largeIcon</span></span>|[<span data-ttu-id="63431-136">mimeContent</span><span class="sxs-lookup"><span data-stu-id="63431-136">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="63431-137">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll</span><span class="sxs-lookup"><span data-stu-id="63431-137">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="63431-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="63431-138">createdDateTime</span></span>|<span data-ttu-id="63431-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63431-139">DateTimeOffset</span></span>|<span data-ttu-id="63431-140">Datum und Uhrzeit der Erstellung der App</span><span class="sxs-lookup"><span data-stu-id="63431-140">The date and time the app was created.</span></span>|
|<span data-ttu-id="63431-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="63431-141">lastModifiedDateTime</span></span>|<span data-ttu-id="63431-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63431-142">DateTimeOffset</span></span>|<span data-ttu-id="63431-143">Datum und Uhrzeit der letzten Änderung der App</span><span class="sxs-lookup"><span data-stu-id="63431-143">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="63431-144">isFeatured</span><span class="sxs-lookup"><span data-stu-id="63431-144">isFeatured</span></span>|<span data-ttu-id="63431-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="63431-145">Boolean</span></span>|<span data-ttu-id="63431-146">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde</span><span class="sxs-lookup"><span data-stu-id="63431-146">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="63431-147">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="63431-147">privacyInformationUrl</span></span>|<span data-ttu-id="63431-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="63431-148">String</span></span>|<span data-ttu-id="63431-149">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="63431-149">The privacy statement Url.</span></span>|
|<span data-ttu-id="63431-150">informationUrl</span><span class="sxs-lookup"><span data-stu-id="63431-150">informationUrl</span></span>|<span data-ttu-id="63431-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="63431-151">String</span></span>|<span data-ttu-id="63431-152">URL zur Seite mit weiteren Informationen</span><span class="sxs-lookup"><span data-stu-id="63431-152">The more information Url.</span></span>|
|<span data-ttu-id="63431-153">owner</span><span class="sxs-lookup"><span data-stu-id="63431-153">owner</span></span>|<span data-ttu-id="63431-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="63431-154">String</span></span>|<span data-ttu-id="63431-155">Besitzer der App</span><span class="sxs-lookup"><span data-stu-id="63431-155">The owner of the app.</span></span>|
|<span data-ttu-id="63431-156">developer</span><span class="sxs-lookup"><span data-stu-id="63431-156">developer</span></span>|<span data-ttu-id="63431-157">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="63431-157">String</span></span>|<span data-ttu-id="63431-158">Entwickler der App</span><span class="sxs-lookup"><span data-stu-id="63431-158">The developer of the app.</span></span>|
|<span data-ttu-id="63431-159">notes</span><span class="sxs-lookup"><span data-stu-id="63431-159">notes</span></span>|<span data-ttu-id="63431-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="63431-160">String</span></span>|<span data-ttu-id="63431-161">Hinweise zur App</span><span class="sxs-lookup"><span data-stu-id="63431-161">Notes for the app.</span></span>|
|<span data-ttu-id="63431-162">publishingState</span><span class="sxs-lookup"><span data-stu-id="63431-162">publishingState</span></span>|[<span data-ttu-id="63431-163">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="63431-163">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="63431-164">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="63431-164">The publishing state for the app.</span></span> <span data-ttu-id="63431-165">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="63431-165">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="63431-166">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="63431-166">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63431-167">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="63431-167">Relationships</span></span>
|<span data-ttu-id="63431-168">Beziehung</span><span class="sxs-lookup"><span data-stu-id="63431-168">Relationship</span></span>|<span data-ttu-id="63431-169">Typ</span><span class="sxs-lookup"><span data-stu-id="63431-169">Type</span></span>|<span data-ttu-id="63431-170">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="63431-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63431-171">categories</span><span class="sxs-lookup"><span data-stu-id="63431-171">categories</span></span>|<span data-ttu-id="63431-172">Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="63431-172">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="63431-173">Liste der Kategorien, denen die App zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="63431-173">The list of categories for this app.</span></span>|
|<span data-ttu-id="63431-174">assignments</span><span class="sxs-lookup"><span data-stu-id="63431-174">assignments</span></span>|<span data-ttu-id="63431-175">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="63431-175">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="63431-176">Liste der Gruppenzuweisungen für die mobile App</span><span class="sxs-lookup"><span data-stu-id="63431-176">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="63431-177">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="63431-177">JSON Representation</span></span>
<span data-ttu-id="63431-178">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="63431-178">Here is a JSON representation of the resource.</span></span>
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



