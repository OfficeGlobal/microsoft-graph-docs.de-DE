---
title: managedAndroidStoreApp erstellen
description: Erstellen eines neuen ManagedAndroidStoreApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49c9db2905a6e72107a298743ffa2a7ffbf39027
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140068"
---
# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="c2ac5-103">managedAndroidStoreApp erstellen</span><span class="sxs-lookup"><span data-stu-id="c2ac5-103">Create managedAndroidStoreApp</span></span>

> <span data-ttu-id="c2ac5-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2ac5-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2ac5-106">Erstellen eines neuen [ManagedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-106">Create a new [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2ac5-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c2ac5-107">Prerequisites</span></span>
<span data-ttu-id="c2ac5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c2ac5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c2ac5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c2ac5-110">Permission type</span></span>|<span data-ttu-id="c2ac5-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c2ac5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2ac5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c2ac5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c2ac5-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2ac5-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c2ac5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c2ac5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2ac5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c2ac5-115">Not supported.</span></span>|
|<span data-ttu-id="c2ac5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c2ac5-116">Application</span></span>|<span data-ttu-id="c2ac5-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c2ac5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2ac5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c2ac5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c2ac5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c2ac5-119">Request headers</span></span>
|<span data-ttu-id="c2ac5-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c2ac5-120">Header</span></span>|<span data-ttu-id="c2ac5-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c2ac5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2ac5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2ac5-122">Authorization</span></span>|<span data-ttu-id="c2ac5-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c2ac5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2ac5-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c2ac5-124">Accept</span></span>|<span data-ttu-id="c2ac5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c2ac5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2ac5-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c2ac5-126">Request body</span></span>
<span data-ttu-id="c2ac5-127">Geben Sie im Anforderungstext eine JSON-Darstellung des managedAndroidStoreApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-127">In the request body, supply a JSON representation for the managedAndroidStoreApp object.</span></span>

<span data-ttu-id="c2ac5-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managedAndroidStoreApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-128">The following table shows the properties that are required when you create the managedAndroidStoreApp.</span></span>

|<span data-ttu-id="c2ac5-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c2ac5-129">Property</span></span>|<span data-ttu-id="c2ac5-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c2ac5-130">Type</span></span>|<span data-ttu-id="c2ac5-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c2ac5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2ac5-132">id</span><span class="sxs-lookup"><span data-stu-id="c2ac5-132">id</span></span>|<span data-ttu-id="c2ac5-133">string</span><span class="sxs-lookup"><span data-stu-id="c2ac5-133">String</span></span>|<span data-ttu-id="c2ac5-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c2ac5-134">Key of the entity.</span></span> <span data-ttu-id="c2ac5-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c2ac5-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2ac5-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c2ac5-136">displayName</span></span>|<span data-ttu-id="c2ac5-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c2ac5-137">String</span></span>|<span data-ttu-id="c2ac5-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c2ac5-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c2ac5-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2ac5-140">description</span><span class="sxs-lookup"><span data-stu-id="c2ac5-140">description</span></span>|<span data-ttu-id="c2ac5-141">String</span><span class="sxs-lookup"><span data-stu-id="c2ac5-141">String</span></span>|<span data-ttu-id="c2ac5-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-142">The description of the app.</span></span> <span data-ttu-id="c2ac5-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c2ac5-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2ac5-144">publisher</span><span class="sxs-lookup"><span data-stu-id="c2ac5-144">publisher</span></span>|<span data-ttu-id="c2ac5-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c2ac5-145">String</span></span>|<span data-ttu-id="c2ac5-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-146">The publisher of the app.</span></span> <span data-ttu-id="c2ac5-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c2ac5-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2ac5-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c2ac5-148">largeIcon</span></span>|[<span data-ttu-id="c2ac5-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c2ac5-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c2ac5-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c2ac5-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c2ac5-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2ac5-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c2ac5-152">createdDateTime</span></span>|<span data-ttu-id="c2ac5-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2ac5-153">DateTimeOffset</span></span>|<span data-ttu-id="c2ac5-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-154">The date and time the app was created.</span></span> <span data-ttu-id="c2ac5-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c2ac5-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2ac5-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2ac5-156">lastModifiedDateTime</span></span>|<span data-ttu-id="c2ac5-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2ac5-157">DateTimeOffset</span></span>|<span data-ttu-id="c2ac5-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-158">The date and time the app was last modified.</span></span> <span data-ttu-id="c2ac5-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c2ac5-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2ac5-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c2ac5-160">isFeatured</span></span>|<span data-ttu-id="c2ac5-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c2ac5-161">Boolean</span></span>|<span data-ttu-id="c2ac5-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c2ac5-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2ac5-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c2ac5-163">privacyInformationUrl</span></span>|<span data-ttu-id="c2ac5-164">String</span><span class="sxs-lookup"><span data-stu-id="c2ac5-164">String</span></span>|<span data-ttu-id="c2ac5-165">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-165">The privacy statement Url.</span></span> <span data-ttu-id="c2ac5-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c2ac5-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2ac5-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c2ac5-167">informationUrl</span></span>|<span data-ttu-id="c2ac5-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c2ac5-168">String</span></span>|<span data-ttu-id="c2ac5-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-169">The more information Url.</span></span> <span data-ttu-id="c2ac5-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c2ac5-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2ac5-171">owner</span><span class="sxs-lookup"><span data-stu-id="c2ac5-171">owner</span></span>|<span data-ttu-id="c2ac5-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c2ac5-172">String</span></span>|<span data-ttu-id="c2ac5-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-173">The owner of the app.</span></span> <span data-ttu-id="c2ac5-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c2ac5-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2ac5-175">developer</span><span class="sxs-lookup"><span data-stu-id="c2ac5-175">developer</span></span>|<span data-ttu-id="c2ac5-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c2ac5-176">String</span></span>|<span data-ttu-id="c2ac5-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-177">The developer of the app.</span></span> <span data-ttu-id="c2ac5-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c2ac5-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2ac5-179">notes</span><span class="sxs-lookup"><span data-stu-id="c2ac5-179">notes</span></span>|<span data-ttu-id="c2ac5-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c2ac5-180">String</span></span>|<span data-ttu-id="c2ac5-181">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-181">Notes for the app.</span></span> <span data-ttu-id="c2ac5-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c2ac5-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2ac5-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="c2ac5-183">uploadState</span></span>|<span data-ttu-id="c2ac5-184">Int32</span><span class="sxs-lookup"><span data-stu-id="c2ac5-184">Int32</span></span>|<span data-ttu-id="c2ac5-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-185">The upload state.</span></span> <span data-ttu-id="c2ac5-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c2ac5-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2ac5-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="c2ac5-187">publishingState</span></span>|[<span data-ttu-id="c2ac5-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c2ac5-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c2ac5-189">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-189">The publishing state for the app.</span></span> <span data-ttu-id="c2ac5-190">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c2ac5-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c2ac5-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c2ac5-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c2ac5-193">isAssigned</span></span>|<span data-ttu-id="c2ac5-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2ac5-194">Boolean</span></span>|<span data-ttu-id="c2ac5-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="c2ac5-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c2ac5-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2ac5-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="c2ac5-197">roleScopeTagIds</span></span>|<span data-ttu-id="c2ac5-198">String collection</span><span class="sxs-lookup"><span data-stu-id="c2ac5-198">String collection</span></span>|<span data-ttu-id="c2ac5-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="c2ac5-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c2ac5-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c2ac5-201">appAvailability</span><span class="sxs-lookup"><span data-stu-id="c2ac5-201">appAvailability</span></span>|[<span data-ttu-id="c2ac5-202">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="c2ac5-202">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="c2ac5-203">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-203">The Application's availability.</span></span> <span data-ttu-id="c2ac5-204">Von [ManagedApp](../resources/intune-apps-managedapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-204">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="c2ac5-205">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-205">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="c2ac5-206">version</span><span class="sxs-lookup"><span data-stu-id="c2ac5-206">version</span></span>|<span data-ttu-id="c2ac5-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c2ac5-207">String</span></span>|<span data-ttu-id="c2ac5-208">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-208">The Application's version.</span></span> <span data-ttu-id="c2ac5-209">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="c2ac5-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="c2ac5-210">packageId</span><span class="sxs-lookup"><span data-stu-id="c2ac5-210">packageId</span></span>|<span data-ttu-id="c2ac5-211">String</span><span class="sxs-lookup"><span data-stu-id="c2ac5-211">String</span></span>|<span data-ttu-id="c2ac5-212">Die Paket-ID der App.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-212">The app's package ID.</span></span>|
|<span data-ttu-id="c2ac5-213">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="c2ac5-213">appStoreUrl</span></span>|<span data-ttu-id="c2ac5-214">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c2ac5-214">String</span></span>|<span data-ttu-id="c2ac5-215">Die URL des Android-App-Stores.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-215">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="c2ac5-216">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c2ac5-216">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c2ac5-217">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c2ac5-217">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="c2ac5-218">Der Wert für die Mindestversion des unterstützten Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-218">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="c2ac5-219">Antwort</span><span class="sxs-lookup"><span data-stu-id="c2ac5-219">Response</span></span>
<span data-ttu-id="c2ac5-220">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-220">If successful, this method returns a `201 Created` response code and a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2ac5-221">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c2ac5-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2ac5-222">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c2ac5-222">Request</span></span>
<span data-ttu-id="c2ac5-223">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1237

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="c2ac5-224">Antwort</span><span class="sxs-lookup"><span data-stu-id="c2ac5-224">Response</span></span>
<span data-ttu-id="c2ac5-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c2ac5-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1409

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```




