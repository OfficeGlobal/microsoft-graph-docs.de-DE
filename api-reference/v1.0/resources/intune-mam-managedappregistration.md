---
title: Ressourcentyp „managedAppRegistration“
description: ManagedAppEntity ist der Basisentitätstyp für alle anderen Entitätstypen im App-Verwaltungsworkflow.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8a954c3465ba4bb4d2f7372ee544a00fcd8c2af7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937089"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="9415e-103">Ressourcentyp „managedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="9415e-103">managedAppRegistration resource type</span></span>

> <span data-ttu-id="9415e-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9415e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9415e-105">Der Entitätstyp „ManagedAppEntity“ ist der Basisentitätstyp für alle anderen Entitätstypen im Workflow für die App-Verwaltung.</span><span class="sxs-lookup"><span data-stu-id="9415e-105">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="9415e-106">Die Ressource „managedAppRegistration“ repräsentiert die Details einer verwalteten App, die von einem Mitglied der Organisation verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="9415e-106">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="9415e-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="9415e-107">Methods</span></span>
|<span data-ttu-id="9415e-108">Methode</span><span class="sxs-lookup"><span data-stu-id="9415e-108">Method</span></span>|<span data-ttu-id="9415e-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9415e-109">Return Type</span></span>|<span data-ttu-id="9415e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9415e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9415e-111">Auflisten von „managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="9415e-111">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="9415e-112">Sammlung von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span><span class="sxs-lookup"><span data-stu-id="9415e-112">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="9415e-113">Listet die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="9415e-113">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="9415e-114">Abrufen von „managedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="9415e-114">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="9415e-115">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="9415e-115">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="9415e-116">Liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppRegistration](../resources/intune-mam-managedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="9415e-116">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="9415e-117">Funktion „getUserIdsWithFlaggedAppRegistration“</span><span class="sxs-lookup"><span data-stu-id="9415e-117">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="9415e-118">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="9415e-118">String collection</span></span>|<span data-ttu-id="9415e-119">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="9415e-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9415e-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9415e-120">Properties</span></span>
|<span data-ttu-id="9415e-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9415e-121">Property</span></span>|<span data-ttu-id="9415e-122">Typ</span><span class="sxs-lookup"><span data-stu-id="9415e-122">Type</span></span>|<span data-ttu-id="9415e-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9415e-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9415e-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9415e-124">createdDateTime</span></span>|<span data-ttu-id="9415e-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9415e-125">DateTimeOffset</span></span>|<span data-ttu-id="9415e-126">Datum und Uhrzeit der Erstellung</span><span class="sxs-lookup"><span data-stu-id="9415e-126">Date and time of creation</span></span>|
|<span data-ttu-id="9415e-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9415e-127">lastSyncDateTime</span></span>|<span data-ttu-id="9415e-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9415e-128">DateTimeOffset</span></span>|<span data-ttu-id="9415e-129">Datum und Uhrzeit der letzten Synchronisierung der App mit dem Verwaltungsdienst</span><span class="sxs-lookup"><span data-stu-id="9415e-129">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="9415e-130">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="9415e-130">applicationVersion</span></span>|<span data-ttu-id="9415e-131">String</span><span class="sxs-lookup"><span data-stu-id="9415e-131">String</span></span>|<span data-ttu-id="9415e-132">Version der App</span><span class="sxs-lookup"><span data-stu-id="9415e-132">App version</span></span>|
|<span data-ttu-id="9415e-133">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="9415e-133">managementSdkVersion</span></span>|<span data-ttu-id="9415e-134">String</span><span class="sxs-lookup"><span data-stu-id="9415e-134">String</span></span>|<span data-ttu-id="9415e-135">Version des App-Verwaltungs-SDK</span><span class="sxs-lookup"><span data-stu-id="9415e-135">App management SDK version</span></span>|
|<span data-ttu-id="9415e-136">platformVersion</span><span class="sxs-lookup"><span data-stu-id="9415e-136">platformVersion</span></span>|<span data-ttu-id="9415e-137">String</span><span class="sxs-lookup"><span data-stu-id="9415e-137">String</span></span>|<span data-ttu-id="9415e-138">Version des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="9415e-138">Operating System version</span></span>|
|<span data-ttu-id="9415e-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="9415e-139">deviceType</span></span>|<span data-ttu-id="9415e-140">String</span><span class="sxs-lookup"><span data-stu-id="9415e-140">String</span></span>|<span data-ttu-id="9415e-141">Gerätetyp des Hostgeräts</span><span class="sxs-lookup"><span data-stu-id="9415e-141">Host device type</span></span>|
|<span data-ttu-id="9415e-142">deviceTag</span><span class="sxs-lookup"><span data-stu-id="9415e-142">deviceTag</span></span>|<span data-ttu-id="9415e-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9415e-143">String</span></span>|<span data-ttu-id="9415e-144">Vom App-Verwaltungs-SDK generiertes Tag, das bei der Zuordnung von Apps hilft, die auf demselben Gerät gehostet werden.</span><span class="sxs-lookup"><span data-stu-id="9415e-144">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="9415e-145">Es ist nicht garantiert, dass die App-Zuordnung unter allen Bedingungen funktioniert.</span><span class="sxs-lookup"><span data-stu-id="9415e-145">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="9415e-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="9415e-146">deviceName</span></span>|<span data-ttu-id="9415e-147">String</span><span class="sxs-lookup"><span data-stu-id="9415e-147">String</span></span>|<span data-ttu-id="9415e-148">Gerätename des Hostgeräts</span><span class="sxs-lookup"><span data-stu-id="9415e-148">Host device name</span></span>|
|<span data-ttu-id="9415e-149">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="9415e-149">flaggedReasons</span></span>|<span data-ttu-id="9415e-150">[ManagedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="9415e-150">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="9415e-151">Gründe (0 oder mehr), aus denen eine App-Registrierung gekennzeichnet wurde.</span><span class="sxs-lookup"><span data-stu-id="9415e-151">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="9415e-152">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="9415e-152">E.g.</span></span> <span data-ttu-id="9415e-153">Die App wird auf einem gerooteten Gerät ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="9415e-153">app running on rooted device</span></span>|
|<span data-ttu-id="9415e-154">userId</span><span class="sxs-lookup"><span data-stu-id="9415e-154">userId</span></span>|<span data-ttu-id="9415e-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9415e-155">String</span></span>|<span data-ttu-id="9415e-156">Benutzer-ID, zu der die App-Registrierung gehört</span><span class="sxs-lookup"><span data-stu-id="9415e-156">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="9415e-157">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="9415e-157">appIdentifier</span></span>|[<span data-ttu-id="9415e-158">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9415e-158">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="9415e-159">Bezeichner des App-Pakets</span><span class="sxs-lookup"><span data-stu-id="9415e-159">The app package Identifier</span></span>|
|<span data-ttu-id="9415e-160">id</span><span class="sxs-lookup"><span data-stu-id="9415e-160">id</span></span>|<span data-ttu-id="9415e-161">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9415e-161">String</span></span>|<span data-ttu-id="9415e-162">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9415e-162">Key of the entity.</span></span>|
|<span data-ttu-id="9415e-163">Version</span><span class="sxs-lookup"><span data-stu-id="9415e-163">version</span></span>|<span data-ttu-id="9415e-164">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9415e-164">String</span></span>|<span data-ttu-id="9415e-165">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="9415e-165">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9415e-166">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9415e-166">Relationships</span></span>
|<span data-ttu-id="9415e-167">Beziehung</span><span class="sxs-lookup"><span data-stu-id="9415e-167">Relationship</span></span>|<span data-ttu-id="9415e-168">Typ</span><span class="sxs-lookup"><span data-stu-id="9415e-168">Type</span></span>|<span data-ttu-id="9415e-169">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9415e-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9415e-170">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="9415e-170">appliedPolicies</span></span>|<span data-ttu-id="9415e-171">Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9415e-171">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="9415e-172">Richtlinien (0 oder mehr), die bereits auf die registrierte App angewendet wurden, als sie letztmals mit dem Verwaltungsdienst synchronisiert wurde</span><span class="sxs-lookup"><span data-stu-id="9415e-172">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="9415e-173">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="9415e-173">intendedPolicies</span></span>|<span data-ttu-id="9415e-174">Sammlung von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9415e-174">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="9415e-175">Richtlinien (0 oder mehr), die der Administrator bisher für die App vorgesehen hat</span><span class="sxs-lookup"><span data-stu-id="9415e-175">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="9415e-176">operations</span><span class="sxs-lookup"><span data-stu-id="9415e-176">operations</span></span>|<span data-ttu-id="9415e-177">Sammlung von Objekten des Typs [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="9415e-177">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="9415e-178">Operationen (0 oder mehr) mit langer Ausführungszeit, die bei der App-Registrierung ausgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="9415e-178">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9415e-179">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9415e-179">JSON Representation</span></span>
<span data-ttu-id="9415e-180">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9415e-180">Here is a JSON representation of the resource.</span></span>
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
