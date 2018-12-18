---
title: iosStoreApp erstellen
description: Erstellen eines neuen IosStoreApp-Objekts.
author: tfitzmac
ms.openlocfilehash: 0d46f8f8e123563f86a0475593f2699705f8fd5d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328798"
---
# <a name="create-iosstoreapp"></a><span data-ttu-id="1141f-103">iosStoreApp erstellen</span><span class="sxs-lookup"><span data-stu-id="1141f-103">Create iosStoreApp</span></span>

> <span data-ttu-id="1141f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1141f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1141f-105">Erstellen eines neuen [IosStoreApp](../resources/intune-apps-iosstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1141f-105">Create a new [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1141f-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1141f-106">Prerequisites</span></span>
<span data-ttu-id="1141f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1141f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1141f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1141f-109">Permission type</span></span>|<span data-ttu-id="1141f-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1141f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1141f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1141f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1141f-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1141f-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1141f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1141f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1141f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1141f-114">Not supported.</span></span>|
|<span data-ttu-id="1141f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1141f-115">Application</span></span>|<span data-ttu-id="1141f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1141f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1141f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1141f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1141f-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1141f-118">Request headers</span></span>
|<span data-ttu-id="1141f-119">Header</span><span class="sxs-lookup"><span data-stu-id="1141f-119">Header</span></span>|<span data-ttu-id="1141f-120">Wert</span><span class="sxs-lookup"><span data-stu-id="1141f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1141f-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1141f-121">Authorization</span></span>|<span data-ttu-id="1141f-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1141f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1141f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1141f-123">Accept</span></span>|<span data-ttu-id="1141f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1141f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1141f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1141f-125">Request body</span></span>
<span data-ttu-id="1141f-126">Geben Sie im Anforderungstext eine JSON-Darstellung des iosStoreApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="1141f-126">In the request body, supply a JSON representation for the iosStoreApp object.</span></span>

<span data-ttu-id="1141f-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosStoreApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="1141f-127">The following table shows the properties that are required when you create the iosStoreApp.</span></span>

|<span data-ttu-id="1141f-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1141f-128">Property</span></span>|<span data-ttu-id="1141f-129">Typ</span><span class="sxs-lookup"><span data-stu-id="1141f-129">Type</span></span>|<span data-ttu-id="1141f-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1141f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1141f-131">id</span><span class="sxs-lookup"><span data-stu-id="1141f-131">id</span></span>|<span data-ttu-id="1141f-132">String</span><span class="sxs-lookup"><span data-stu-id="1141f-132">String</span></span>|<span data-ttu-id="1141f-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1141f-133">Key of the entity.</span></span> <span data-ttu-id="1141f-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1141f-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1141f-135">displayName</span><span class="sxs-lookup"><span data-stu-id="1141f-135">displayName</span></span>|<span data-ttu-id="1141f-136">String</span><span class="sxs-lookup"><span data-stu-id="1141f-136">String</span></span>|<span data-ttu-id="1141f-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="1141f-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1141f-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1141f-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1141f-139">description</span><span class="sxs-lookup"><span data-stu-id="1141f-139">description</span></span>|<span data-ttu-id="1141f-140">String</span><span class="sxs-lookup"><span data-stu-id="1141f-140">String</span></span>|<span data-ttu-id="1141f-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="1141f-141">The description of the app.</span></span> <span data-ttu-id="1141f-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1141f-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1141f-143">publisher</span><span class="sxs-lookup"><span data-stu-id="1141f-143">publisher</span></span>|<span data-ttu-id="1141f-144">String</span><span class="sxs-lookup"><span data-stu-id="1141f-144">String</span></span>|<span data-ttu-id="1141f-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="1141f-145">The publisher of the app.</span></span> <span data-ttu-id="1141f-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1141f-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1141f-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1141f-147">largeIcon</span></span>|[<span data-ttu-id="1141f-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1141f-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1141f-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="1141f-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1141f-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1141f-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1141f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1141f-151">createdDateTime</span></span>|<span data-ttu-id="1141f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1141f-152">DateTimeOffset</span></span>|<span data-ttu-id="1141f-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="1141f-153">The date and time the app was created.</span></span> <span data-ttu-id="1141f-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1141f-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1141f-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1141f-155">lastModifiedDateTime</span></span>|<span data-ttu-id="1141f-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1141f-156">DateTimeOffset</span></span>|<span data-ttu-id="1141f-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="1141f-157">The date and time the app was last modified.</span></span> <span data-ttu-id="1141f-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1141f-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1141f-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1141f-159">isFeatured</span></span>|<span data-ttu-id="1141f-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1141f-160">Boolean</span></span>|<span data-ttu-id="1141f-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1141f-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1141f-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1141f-162">privacyInformationUrl</span></span>|<span data-ttu-id="1141f-163">String</span><span class="sxs-lookup"><span data-stu-id="1141f-163">String</span></span>|<span data-ttu-id="1141f-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="1141f-164">The privacy statement Url.</span></span> <span data-ttu-id="1141f-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1141f-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1141f-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1141f-166">informationUrl</span></span>|<span data-ttu-id="1141f-167">String</span><span class="sxs-lookup"><span data-stu-id="1141f-167">String</span></span>|<span data-ttu-id="1141f-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="1141f-168">The more information Url.</span></span> <span data-ttu-id="1141f-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1141f-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1141f-170">owner</span><span class="sxs-lookup"><span data-stu-id="1141f-170">owner</span></span>|<span data-ttu-id="1141f-171">String</span><span class="sxs-lookup"><span data-stu-id="1141f-171">String</span></span>|<span data-ttu-id="1141f-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="1141f-172">The owner of the app.</span></span> <span data-ttu-id="1141f-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1141f-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1141f-174">developer</span><span class="sxs-lookup"><span data-stu-id="1141f-174">developer</span></span>|<span data-ttu-id="1141f-175">String</span><span class="sxs-lookup"><span data-stu-id="1141f-175">String</span></span>|<span data-ttu-id="1141f-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="1141f-176">The developer of the app.</span></span> <span data-ttu-id="1141f-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1141f-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1141f-178">notes</span><span class="sxs-lookup"><span data-stu-id="1141f-178">notes</span></span>|<span data-ttu-id="1141f-179">String</span><span class="sxs-lookup"><span data-stu-id="1141f-179">String</span></span>|<span data-ttu-id="1141f-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="1141f-180">Notes for the app.</span></span> <span data-ttu-id="1141f-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1141f-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1141f-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="1141f-182">publishingState</span></span>|[<span data-ttu-id="1141f-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1141f-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1141f-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="1141f-184">The publishing state for the app.</span></span> <span data-ttu-id="1141f-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="1141f-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1141f-186">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1141f-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="1141f-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="1141f-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1141f-188">bundleId</span><span class="sxs-lookup"><span data-stu-id="1141f-188">bundleId</span></span>|<span data-ttu-id="1141f-189">String</span><span class="sxs-lookup"><span data-stu-id="1141f-189">String</span></span>|<span data-ttu-id="1141f-190">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="1141f-190">The Identity Name.</span></span>|
|<span data-ttu-id="1141f-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="1141f-191">appStoreUrl</span></span>|<span data-ttu-id="1141f-192">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1141f-192">String</span></span>|<span data-ttu-id="1141f-193">URL des Apple-App-Stores</span><span class="sxs-lookup"><span data-stu-id="1141f-193">The Apple App Store URL</span></span>|
|<span data-ttu-id="1141f-194">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="1141f-194">applicableDeviceType</span></span>|[<span data-ttu-id="1141f-195">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="1141f-195">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="1141f-196">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="1141f-196">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="1141f-197">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1141f-197">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1141f-198">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1141f-198">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="1141f-199">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="1141f-199">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="1141f-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="1141f-200">Response</span></span>
<span data-ttu-id="1141f-201">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosStoreApp](../resources/intune-apps-iosstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1141f-201">If successful, this method returns a `201 Created` response code and a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1141f-202">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1141f-202">Example</span></span>
### <a name="request"></a><span data-ttu-id="1141f-203">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1141f-203">Request</span></span>
<span data-ttu-id="1141f-204">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1141f-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1006

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="1141f-205">Antwort</span><span class="sxs-lookup"><span data-stu-id="1141f-205">Response</span></span>
<span data-ttu-id="1141f-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1141f-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1178

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```



