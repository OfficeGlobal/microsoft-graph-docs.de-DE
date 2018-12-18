---
title: managedIOSStoreApp erstellen
description: Erstellen eines neuen managedIOSStoreApp-Objekts.
author: tfitzmac
ms.openlocfilehash: 392d7fee5685afe1804c8832bdd1fcb72ff6d3a9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319467"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="cb5d2-103">managedIOSStoreApp erstellen</span><span class="sxs-lookup"><span data-stu-id="cb5d2-103">Create managedIOSStoreApp</span></span>

> <span data-ttu-id="cb5d2-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb5d2-105">Erstellen eines neuen [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-105">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cb5d2-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cb5d2-106">Prerequisites</span></span>
<span data-ttu-id="cb5d2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb5d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb5d2-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cb5d2-109">Permission type</span></span>|<span data-ttu-id="cb5d2-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cb5d2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb5d2-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cb5d2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cb5d2-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb5d2-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cb5d2-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cb5d2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb5d2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cb5d2-114">Not supported.</span></span>|
|<span data-ttu-id="cb5d2-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cb5d2-115">Application</span></span>|<span data-ttu-id="cb5d2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cb5d2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb5d2-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cb5d2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="cb5d2-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cb5d2-118">Request headers</span></span>
|<span data-ttu-id="cb5d2-119">Header</span><span class="sxs-lookup"><span data-stu-id="cb5d2-119">Header</span></span>|<span data-ttu-id="cb5d2-120">Wert</span><span class="sxs-lookup"><span data-stu-id="cb5d2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb5d2-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="cb5d2-121">Authorization</span></span>|<span data-ttu-id="cb5d2-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cb5d2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb5d2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cb5d2-123">Accept</span></span>|<span data-ttu-id="cb5d2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cb5d2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb5d2-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cb5d2-125">Request body</span></span>
<span data-ttu-id="cb5d2-126">Geben Sie im Anforderungstext eine JSON-Darstellung des managedIOSStoreApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-126">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="cb5d2-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managedIOSStoreApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-127">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="cb5d2-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cb5d2-128">Property</span></span>|<span data-ttu-id="cb5d2-129">Typ</span><span class="sxs-lookup"><span data-stu-id="cb5d2-129">Type</span></span>|<span data-ttu-id="cb5d2-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb5d2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb5d2-131">id</span><span class="sxs-lookup"><span data-stu-id="cb5d2-131">id</span></span>|<span data-ttu-id="cb5d2-132">String</span><span class="sxs-lookup"><span data-stu-id="cb5d2-132">String</span></span>|<span data-ttu-id="cb5d2-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="cb5d2-133">Key of the entity.</span></span> <span data-ttu-id="cb5d2-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb5d2-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb5d2-135">displayName</span><span class="sxs-lookup"><span data-stu-id="cb5d2-135">displayName</span></span>|<span data-ttu-id="cb5d2-136">String</span><span class="sxs-lookup"><span data-stu-id="cb5d2-136">String</span></span>|<span data-ttu-id="cb5d2-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cb5d2-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb5d2-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb5d2-139">description</span><span class="sxs-lookup"><span data-stu-id="cb5d2-139">description</span></span>|<span data-ttu-id="cb5d2-140">String</span><span class="sxs-lookup"><span data-stu-id="cb5d2-140">String</span></span>|<span data-ttu-id="cb5d2-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-141">The description of the app.</span></span> <span data-ttu-id="cb5d2-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb5d2-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb5d2-143">publisher</span><span class="sxs-lookup"><span data-stu-id="cb5d2-143">publisher</span></span>|<span data-ttu-id="cb5d2-144">String</span><span class="sxs-lookup"><span data-stu-id="cb5d2-144">String</span></span>|<span data-ttu-id="cb5d2-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-145">The publisher of the app.</span></span> <span data-ttu-id="cb5d2-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb5d2-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb5d2-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cb5d2-147">largeIcon</span></span>|[<span data-ttu-id="cb5d2-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cb5d2-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cb5d2-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cb5d2-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb5d2-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb5d2-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb5d2-151">createdDateTime</span></span>|<span data-ttu-id="cb5d2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb5d2-152">DateTimeOffset</span></span>|<span data-ttu-id="cb5d2-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-153">The date and time the app was created.</span></span> <span data-ttu-id="cb5d2-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb5d2-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb5d2-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb5d2-155">lastModifiedDateTime</span></span>|<span data-ttu-id="cb5d2-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb5d2-156">DateTimeOffset</span></span>|<span data-ttu-id="cb5d2-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-157">The date and time the app was last modified.</span></span> <span data-ttu-id="cb5d2-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb5d2-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb5d2-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cb5d2-159">isFeatured</span></span>|<span data-ttu-id="cb5d2-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="cb5d2-160">Boolean</span></span>|<span data-ttu-id="cb5d2-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb5d2-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb5d2-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cb5d2-162">privacyInformationUrl</span></span>|<span data-ttu-id="cb5d2-163">String</span><span class="sxs-lookup"><span data-stu-id="cb5d2-163">String</span></span>|<span data-ttu-id="cb5d2-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-164">The privacy statement Url.</span></span> <span data-ttu-id="cb5d2-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb5d2-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb5d2-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cb5d2-166">informationUrl</span></span>|<span data-ttu-id="cb5d2-167">String</span><span class="sxs-lookup"><span data-stu-id="cb5d2-167">String</span></span>|<span data-ttu-id="cb5d2-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-168">The more information Url.</span></span> <span data-ttu-id="cb5d2-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb5d2-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb5d2-170">owner</span><span class="sxs-lookup"><span data-stu-id="cb5d2-170">owner</span></span>|<span data-ttu-id="cb5d2-171">String</span><span class="sxs-lookup"><span data-stu-id="cb5d2-171">String</span></span>|<span data-ttu-id="cb5d2-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-172">The owner of the app.</span></span> <span data-ttu-id="cb5d2-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb5d2-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb5d2-174">developer</span><span class="sxs-lookup"><span data-stu-id="cb5d2-174">developer</span></span>|<span data-ttu-id="cb5d2-175">String</span><span class="sxs-lookup"><span data-stu-id="cb5d2-175">String</span></span>|<span data-ttu-id="cb5d2-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-176">The developer of the app.</span></span> <span data-ttu-id="cb5d2-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb5d2-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb5d2-178">notes</span><span class="sxs-lookup"><span data-stu-id="cb5d2-178">notes</span></span>|<span data-ttu-id="cb5d2-179">String</span><span class="sxs-lookup"><span data-stu-id="cb5d2-179">String</span></span>|<span data-ttu-id="cb5d2-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-180">Notes for the app.</span></span> <span data-ttu-id="cb5d2-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb5d2-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb5d2-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="cb5d2-182">publishingState</span></span>|[<span data-ttu-id="cb5d2-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="cb5d2-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="cb5d2-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-184">The publishing state for the app.</span></span> <span data-ttu-id="cb5d2-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cb5d2-186">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb5d2-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="cb5d2-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cb5d2-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="cb5d2-188">appAvailability</span></span>|[<span data-ttu-id="cb5d2-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="cb5d2-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="cb5d2-190">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-190">The Application's availability.</span></span> <span data-ttu-id="cb5d2-191">Geerbt von [ManagedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="cb5d2-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="cb5d2-192">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="cb5d2-193">version</span><span class="sxs-lookup"><span data-stu-id="cb5d2-193">version</span></span>|<span data-ttu-id="cb5d2-194">String</span><span class="sxs-lookup"><span data-stu-id="cb5d2-194">String</span></span>|<span data-ttu-id="cb5d2-195">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-195">The Application's version.</span></span> <span data-ttu-id="cb5d2-196">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb5d2-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="cb5d2-197">bundleId</span><span class="sxs-lookup"><span data-stu-id="cb5d2-197">bundleId</span></span>|<span data-ttu-id="cb5d2-198">String</span><span class="sxs-lookup"><span data-stu-id="cb5d2-198">String</span></span>|<span data-ttu-id="cb5d2-199">Die Bundle-ID einer App.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-199">The app's Bundle ID.</span></span>|
|<span data-ttu-id="cb5d2-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="cb5d2-200">appStoreUrl</span></span>|<span data-ttu-id="cb5d2-201">String</span><span class="sxs-lookup"><span data-stu-id="cb5d2-201">String</span></span>|<span data-ttu-id="cb5d2-202">Die URL des Apple-App-Stores.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-202">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="cb5d2-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="cb5d2-203">applicableDeviceType</span></span>|[<span data-ttu-id="cb5d2-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="cb5d2-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="cb5d2-205">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-205">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="cb5d2-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cb5d2-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="cb5d2-207">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cb5d2-207">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="cb5d2-208">Der Wert für die Mindestversion des unterstützten Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-208">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="cb5d2-209">Antwort</span><span class="sxs-lookup"><span data-stu-id="cb5d2-209">Response</span></span>
<span data-ttu-id="cb5d2-210">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-210">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb5d2-211">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cb5d2-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="cb5d2-212">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cb5d2-212">Request</span></span>
<span data-ttu-id="cb5d2-213">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-213">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1084

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
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

### <a name="response"></a><span data-ttu-id="cb5d2-214">Antwort</span><span class="sxs-lookup"><span data-stu-id="cb5d2-214">Response</span></span>
<span data-ttu-id="cb5d2-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cb5d2-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1256

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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



