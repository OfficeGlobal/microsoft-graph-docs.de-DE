---
title: managedAndroidStoreApp aktualisieren
description: Aktualisieren der Eigenschaften eines managedAndroidStoreApp-Objekts.
author: tfitzmac
ms.openlocfilehash: c592238c7c48939b47dfc772a93dea4f07f7bf06
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327643"
---
# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="8994d-103">managedAndroidStoreApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8994d-103">Update managedAndroidStoreApp</span></span>

> <span data-ttu-id="8994d-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8994d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8994d-105">Aktualisieren der Eigenschaften eines [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8994d-105">Update the properties of a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8994d-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8994d-106">Prerequisites</span></span>
<span data-ttu-id="8994d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8994d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8994d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8994d-109">Permission type</span></span>|<span data-ttu-id="8994d-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8994d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8994d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8994d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8994d-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8994d-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8994d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8994d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8994d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8994d-114">Not supported.</span></span>|
|<span data-ttu-id="8994d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8994d-115">Application</span></span>|<span data-ttu-id="8994d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8994d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8994d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8994d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="8994d-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8994d-118">Request headers</span></span>
|<span data-ttu-id="8994d-119">Header</span><span class="sxs-lookup"><span data-stu-id="8994d-119">Header</span></span>|<span data-ttu-id="8994d-120">Wert</span><span class="sxs-lookup"><span data-stu-id="8994d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8994d-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="8994d-121">Authorization</span></span>|<span data-ttu-id="8994d-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8994d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8994d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8994d-123">Accept</span></span>|<span data-ttu-id="8994d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8994d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8994d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8994d-125">Request body</span></span>
<span data-ttu-id="8994d-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="8994d-126">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="8994d-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8994d-127">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="8994d-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8994d-128">Property</span></span>|<span data-ttu-id="8994d-129">Typ</span><span class="sxs-lookup"><span data-stu-id="8994d-129">Type</span></span>|<span data-ttu-id="8994d-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8994d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8994d-131">id</span><span class="sxs-lookup"><span data-stu-id="8994d-131">id</span></span>|<span data-ttu-id="8994d-132">String</span><span class="sxs-lookup"><span data-stu-id="8994d-132">String</span></span>|<span data-ttu-id="8994d-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8994d-133">Key of the entity.</span></span> <span data-ttu-id="8994d-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8994d-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8994d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="8994d-135">displayName</span></span>|<span data-ttu-id="8994d-136">String</span><span class="sxs-lookup"><span data-stu-id="8994d-136">String</span></span>|<span data-ttu-id="8994d-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="8994d-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8994d-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8994d-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8994d-139">description</span><span class="sxs-lookup"><span data-stu-id="8994d-139">description</span></span>|<span data-ttu-id="8994d-140">String</span><span class="sxs-lookup"><span data-stu-id="8994d-140">String</span></span>|<span data-ttu-id="8994d-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="8994d-141">The description of the app.</span></span> <span data-ttu-id="8994d-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8994d-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8994d-143">publisher</span><span class="sxs-lookup"><span data-stu-id="8994d-143">publisher</span></span>|<span data-ttu-id="8994d-144">String</span><span class="sxs-lookup"><span data-stu-id="8994d-144">String</span></span>|<span data-ttu-id="8994d-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="8994d-145">The publisher of the app.</span></span> <span data-ttu-id="8994d-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8994d-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8994d-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8994d-147">largeIcon</span></span>|[<span data-ttu-id="8994d-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8994d-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8994d-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="8994d-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8994d-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8994d-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8994d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8994d-151">createdDateTime</span></span>|<span data-ttu-id="8994d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8994d-152">DateTimeOffset</span></span>|<span data-ttu-id="8994d-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="8994d-153">The date and time the app was created.</span></span> <span data-ttu-id="8994d-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8994d-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8994d-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8994d-155">lastModifiedDateTime</span></span>|<span data-ttu-id="8994d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8994d-156">DateTimeOffset</span></span>|<span data-ttu-id="8994d-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="8994d-157">The date and time the app was last modified.</span></span> <span data-ttu-id="8994d-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8994d-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8994d-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8994d-159">isFeatured</span></span>|<span data-ttu-id="8994d-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8994d-160">Boolean</span></span>|<span data-ttu-id="8994d-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8994d-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8994d-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8994d-162">privacyInformationUrl</span></span>|<span data-ttu-id="8994d-163">String</span><span class="sxs-lookup"><span data-stu-id="8994d-163">String</span></span>|<span data-ttu-id="8994d-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="8994d-164">The privacy statement Url.</span></span> <span data-ttu-id="8994d-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8994d-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8994d-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8994d-166">informationUrl</span></span>|<span data-ttu-id="8994d-167">String</span><span class="sxs-lookup"><span data-stu-id="8994d-167">String</span></span>|<span data-ttu-id="8994d-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="8994d-168">The more information Url.</span></span> <span data-ttu-id="8994d-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8994d-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8994d-170">owner</span><span class="sxs-lookup"><span data-stu-id="8994d-170">owner</span></span>|<span data-ttu-id="8994d-171">String</span><span class="sxs-lookup"><span data-stu-id="8994d-171">String</span></span>|<span data-ttu-id="8994d-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="8994d-172">The owner of the app.</span></span> <span data-ttu-id="8994d-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8994d-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8994d-174">developer</span><span class="sxs-lookup"><span data-stu-id="8994d-174">developer</span></span>|<span data-ttu-id="8994d-175">String</span><span class="sxs-lookup"><span data-stu-id="8994d-175">String</span></span>|<span data-ttu-id="8994d-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="8994d-176">The developer of the app.</span></span> <span data-ttu-id="8994d-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8994d-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8994d-178">notes</span><span class="sxs-lookup"><span data-stu-id="8994d-178">notes</span></span>|<span data-ttu-id="8994d-179">String</span><span class="sxs-lookup"><span data-stu-id="8994d-179">String</span></span>|<span data-ttu-id="8994d-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="8994d-180">Notes for the app.</span></span> <span data-ttu-id="8994d-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8994d-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8994d-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="8994d-182">publishingState</span></span>|[<span data-ttu-id="8994d-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8994d-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8994d-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="8994d-184">The publishing state for the app.</span></span> <span data-ttu-id="8994d-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="8994d-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8994d-186">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8994d-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="8994d-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="8994d-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8994d-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="8994d-188">appAvailability</span></span>|[<span data-ttu-id="8994d-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="8994d-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="8994d-190">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="8994d-190">The Application's availability.</span></span> <span data-ttu-id="8994d-191">Geerbt von [ManagedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="8994d-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="8994d-192">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="8994d-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="8994d-193">version</span><span class="sxs-lookup"><span data-stu-id="8994d-193">version</span></span>|<span data-ttu-id="8994d-194">String</span><span class="sxs-lookup"><span data-stu-id="8994d-194">String</span></span>|<span data-ttu-id="8994d-195">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="8994d-195">The Application's version.</span></span> <span data-ttu-id="8994d-196">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="8994d-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="8994d-197">packageId</span><span class="sxs-lookup"><span data-stu-id="8994d-197">packageId</span></span>|<span data-ttu-id="8994d-198">String</span><span class="sxs-lookup"><span data-stu-id="8994d-198">String</span></span>|<span data-ttu-id="8994d-199">Die Paket-ID der App.</span><span class="sxs-lookup"><span data-stu-id="8994d-199">The app's package ID.</span></span>|
|<span data-ttu-id="8994d-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="8994d-200">appStoreUrl</span></span>|<span data-ttu-id="8994d-201">String</span><span class="sxs-lookup"><span data-stu-id="8994d-201">String</span></span>|<span data-ttu-id="8994d-202">Die URL des Android-App-Stores.</span><span class="sxs-lookup"><span data-stu-id="8994d-202">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="8994d-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8994d-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="8994d-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8994d-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="8994d-205">Der Wert für die Mindestversion des unterstützten Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="8994d-205">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="8994d-206">Antwort</span><span class="sxs-lookup"><span data-stu-id="8994d-206">Response</span></span>
<span data-ttu-id="8994d-207">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8994d-207">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8994d-208">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8994d-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="8994d-209">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8994d-209">Request</span></span>
<span data-ttu-id="8994d-210">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8994d-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1016

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
  "publishingState": "processing",
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
    "v5_1": true
  }
}
```

### <a name="response"></a><span data-ttu-id="8994d-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="8994d-211">Response</span></span>
<span data-ttu-id="8994d-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8994d-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1188

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
  "publishingState": "processing",
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
    "v5_1": true
  }
}
```



