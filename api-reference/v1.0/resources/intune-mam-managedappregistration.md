---
title: Ressourcentyp „managedAppRegistration“
description: Der Entitätstyp „ManagedAppEntity“ ist der Basisentitätstyp für alle anderen Entitätstypen im Workflow für die App-Verwaltung. Die Ressource „managedAppRegistration“ repräsentiert die Details einer verwalteten App, die von einem Mitglied der Organisation verwendet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc4754a190f19dab34ac417d2852ccc9e06ba9f4
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252238"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="e679f-104">Ressourcentyp „managedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="e679f-104">managedAppRegistration resource type</span></span>

> <span data-ttu-id="e679f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e679f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e679f-106">Der Entitätstyp „ManagedAppEntity“ ist der Basisentitätstyp für alle anderen Entitätstypen im Workflow für die App-Verwaltung.</span><span class="sxs-lookup"><span data-stu-id="e679f-106">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="e679f-107">Die Ressource „managedAppRegistration“ repräsentiert die Details einer verwalteten App, die von einem Mitglied der Organisation verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="e679f-107">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="e679f-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="e679f-108">Methods</span></span>
|<span data-ttu-id="e679f-109">Methode</span><span class="sxs-lookup"><span data-stu-id="e679f-109">Method</span></span>|<span data-ttu-id="e679f-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e679f-110">Return Type</span></span>|<span data-ttu-id="e679f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e679f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e679f-112">Auflisten von „managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="e679f-112">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="e679f-113">Sammlung von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="e679f-113">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="e679f-114">Listet die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="e679f-114">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="e679f-115">Abrufen von „managedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="e679f-115">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="e679f-116">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="e679f-116">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="e679f-117">Liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="e679f-117">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="e679f-118">Funktion „getUserIdsWithFlaggedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="e679f-118">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="e679f-119">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="e679f-119">String collection</span></span>|<span data-ttu-id="e679f-120">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e679f-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e679f-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e679f-121">Properties</span></span>
|<span data-ttu-id="e679f-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e679f-122">Property</span></span>|<span data-ttu-id="e679f-123">Typ</span><span class="sxs-lookup"><span data-stu-id="e679f-123">Type</span></span>|<span data-ttu-id="e679f-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e679f-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e679f-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e679f-125">createdDateTime</span></span>|<span data-ttu-id="e679f-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e679f-126">DateTimeOffset</span></span>|<span data-ttu-id="e679f-127">Datum und Uhrzeit der Erstellung</span><span class="sxs-lookup"><span data-stu-id="e679f-127">Date and time of creation</span></span>|
|<span data-ttu-id="e679f-128">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e679f-128">lastSyncDateTime</span></span>|<span data-ttu-id="e679f-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e679f-129">DateTimeOffset</span></span>|<span data-ttu-id="e679f-130">Datum und Uhrzeit der letzten Synchronisierung der App mit dem Verwaltungsdienst</span><span class="sxs-lookup"><span data-stu-id="e679f-130">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="e679f-131">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="e679f-131">applicationVersion</span></span>|<span data-ttu-id="e679f-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e679f-132">String</span></span>|<span data-ttu-id="e679f-133">Version der App</span><span class="sxs-lookup"><span data-stu-id="e679f-133">App version</span></span>|
|<span data-ttu-id="e679f-134">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="e679f-134">managementSdkVersion</span></span>|<span data-ttu-id="e679f-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e679f-135">String</span></span>|<span data-ttu-id="e679f-136">Version des App-Verwaltungs-SDK</span><span class="sxs-lookup"><span data-stu-id="e679f-136">App management SDK version</span></span>|
|<span data-ttu-id="e679f-137">platformVersion</span><span class="sxs-lookup"><span data-stu-id="e679f-137">platformVersion</span></span>|<span data-ttu-id="e679f-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e679f-138">String</span></span>|<span data-ttu-id="e679f-139">Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="e679f-139">Operating System version</span></span>|
|<span data-ttu-id="e679f-140">deviceType</span><span class="sxs-lookup"><span data-stu-id="e679f-140">deviceType</span></span>|<span data-ttu-id="e679f-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e679f-141">String</span></span>|<span data-ttu-id="e679f-142">Gerätetyp des Hostgeräts</span><span class="sxs-lookup"><span data-stu-id="e679f-142">Host device type</span></span>|
|<span data-ttu-id="e679f-143">deviceTag</span><span class="sxs-lookup"><span data-stu-id="e679f-143">deviceTag</span></span>|<span data-ttu-id="e679f-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e679f-144">String</span></span>|<span data-ttu-id="e679f-145">Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden.</span><span class="sxs-lookup"><span data-stu-id="e679f-145">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="e679f-146">Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert.</span><span class="sxs-lookup"><span data-stu-id="e679f-146">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="e679f-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="e679f-147">deviceName</span></span>|<span data-ttu-id="e679f-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e679f-148">String</span></span>|<span data-ttu-id="e679f-149">Gerätename des Hostgeräts</span><span class="sxs-lookup"><span data-stu-id="e679f-149">Host device name</span></span>|
|<span data-ttu-id="e679f-150">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="e679f-150">flaggedReasons</span></span>|<span data-ttu-id="e679f-151">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="e679f-151">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="e679f-152">Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="e679f-152">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="e679f-153">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="e679f-153">E.g.</span></span> <span data-ttu-id="e679f-154">Die App wird auf einem gerooteten Gerät ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="e679f-154">app running on rooted device</span></span>|
|<span data-ttu-id="e679f-155">userId</span><span class="sxs-lookup"><span data-stu-id="e679f-155">userId</span></span>|<span data-ttu-id="e679f-156">String</span><span class="sxs-lookup"><span data-stu-id="e679f-156">String</span></span>|<span data-ttu-id="e679f-157">Benutzer-ID, zu der die App-Registrierung gehört</span><span class="sxs-lookup"><span data-stu-id="e679f-157">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="e679f-158">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="e679f-158">appIdentifier</span></span>|[<span data-ttu-id="e679f-159">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="e679f-159">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="e679f-160">Bezeichner des App-Pakets</span><span class="sxs-lookup"><span data-stu-id="e679f-160">The app package Identifier</span></span>|
|<span data-ttu-id="e679f-161">id</span><span class="sxs-lookup"><span data-stu-id="e679f-161">id</span></span>|<span data-ttu-id="e679f-162">string</span><span class="sxs-lookup"><span data-stu-id="e679f-162">String</span></span>|<span data-ttu-id="e679f-163">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e679f-163">Key of the entity.</span></span>|
|<span data-ttu-id="e679f-164">Version</span><span class="sxs-lookup"><span data-stu-id="e679f-164">version</span></span>|<span data-ttu-id="e679f-165">String</span><span class="sxs-lookup"><span data-stu-id="e679f-165">String</span></span>|<span data-ttu-id="e679f-166">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="e679f-166">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e679f-167">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e679f-167">Relationships</span></span>
|<span data-ttu-id="e679f-168">Beziehung</span><span class="sxs-lookup"><span data-stu-id="e679f-168">Relationship</span></span>|<span data-ttu-id="e679f-169">Typ</span><span class="sxs-lookup"><span data-stu-id="e679f-169">Type</span></span>|<span data-ttu-id="e679f-170">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e679f-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e679f-171">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="e679f-171">appliedPolicies</span></span>|<span data-ttu-id="e679f-172">Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e679f-172">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="e679f-173">Richtlinien (0 oder mehr), die bereits auf die registrierte App angewendet wurden, als sie letztmals mit dem Verwaltungsdienst synchronisiert wurde</span><span class="sxs-lookup"><span data-stu-id="e679f-173">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="e679f-174">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="e679f-174">intendedPolicies</span></span>|<span data-ttu-id="e679f-175">Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e679f-175">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="e679f-176">Richtlinien (0 oder mehr), die der Administrator bisher für die App vorgesehen hat</span><span class="sxs-lookup"><span data-stu-id="e679f-176">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="e679f-177">operations</span><span class="sxs-lookup"><span data-stu-id="e679f-177">operations</span></span>|<span data-ttu-id="e679f-178">Sammlung von Objekten des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="e679f-178">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="e679f-179">Operationen (0 oder mehr) mit langer Ausführungszeit, die bei der App-Registrierung ausgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="e679f-179">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e679f-180">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e679f-180">JSON Representation</span></span>
<span data-ttu-id="e679f-181">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e679f-181">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppRegistration",
  "createdDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "applicationVersion": "String",
  "managementSdkVersion": "String",
  "platformVersion": "String",
  "deviceType": "String",
  "deviceTag": "String",
  "deviceName": "String",
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-managedappregistration.md/microsoft.graph.managedAppRegistration/flaggedReasons:
    Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->


