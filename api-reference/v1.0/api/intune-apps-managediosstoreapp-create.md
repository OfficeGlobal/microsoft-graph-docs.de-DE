---
title: managedIOSStoreApp erstellen
description: Erstellen eines neuen managedIOSStoreApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e19fad95e363f3b92165eb3bd0dbc78b57ff7afd
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255507"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="bb0fb-103">managedIOSStoreApp erstellen</span><span class="sxs-lookup"><span data-stu-id="bb0fb-103">Create managedIOSStoreApp</span></span>

> <span data-ttu-id="bb0fb-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb0fb-105">Erstellen eines neuen [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-105">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb0fb-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bb0fb-106">Prerequisites</span></span>
<span data-ttu-id="bb0fb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bb0fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bb0fb-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bb0fb-109">Permission type</span></span>|<span data-ttu-id="bb0fb-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bb0fb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb0fb-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bb0fb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bb0fb-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb0fb-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bb0fb-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bb0fb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb0fb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bb0fb-114">Not supported.</span></span>|
|<span data-ttu-id="bb0fb-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bb0fb-115">Application</span></span>|<span data-ttu-id="bb0fb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bb0fb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb0fb-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bb0fb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="bb0fb-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bb0fb-118">Request headers</span></span>
|<span data-ttu-id="bb0fb-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bb0fb-119">Header</span></span>|<span data-ttu-id="bb0fb-120">Wert</span><span class="sxs-lookup"><span data-stu-id="bb0fb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb0fb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb0fb-121">Authorization</span></span>|<span data-ttu-id="bb0fb-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bb0fb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb0fb-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bb0fb-123">Accept</span></span>|<span data-ttu-id="bb0fb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bb0fb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb0fb-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bb0fb-125">Request body</span></span>
<span data-ttu-id="bb0fb-126">Geben Sie im Anforderungstext eine JSON-Darstellung des managedIOSStoreApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-126">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="bb0fb-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managedIOSStoreApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-127">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="bb0fb-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bb0fb-128">Property</span></span>|<span data-ttu-id="bb0fb-129">Typ</span><span class="sxs-lookup"><span data-stu-id="bb0fb-129">Type</span></span>|<span data-ttu-id="bb0fb-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb0fb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb0fb-131">id</span><span class="sxs-lookup"><span data-stu-id="bb0fb-131">id</span></span>|<span data-ttu-id="bb0fb-132">string</span><span class="sxs-lookup"><span data-stu-id="bb0fb-132">String</span></span>|<span data-ttu-id="bb0fb-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="bb0fb-133">Key of the entity.</span></span> <span data-ttu-id="bb0fb-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb0fb-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb0fb-135">displayName</span><span class="sxs-lookup"><span data-stu-id="bb0fb-135">displayName</span></span>|<span data-ttu-id="bb0fb-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bb0fb-136">String</span></span>|<span data-ttu-id="bb0fb-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="bb0fb-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb0fb-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb0fb-139">description</span><span class="sxs-lookup"><span data-stu-id="bb0fb-139">description</span></span>|<span data-ttu-id="bb0fb-140">String</span><span class="sxs-lookup"><span data-stu-id="bb0fb-140">String</span></span>|<span data-ttu-id="bb0fb-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-141">The description of the app.</span></span> <span data-ttu-id="bb0fb-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb0fb-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb0fb-143">publisher</span><span class="sxs-lookup"><span data-stu-id="bb0fb-143">publisher</span></span>|<span data-ttu-id="bb0fb-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bb0fb-144">String</span></span>|<span data-ttu-id="bb0fb-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-145">The publisher of the app.</span></span> <span data-ttu-id="bb0fb-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb0fb-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb0fb-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="bb0fb-147">largeIcon</span></span>|[<span data-ttu-id="bb0fb-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bb0fb-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="bb0fb-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="bb0fb-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb0fb-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb0fb-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb0fb-151">createdDateTime</span></span>|<span data-ttu-id="bb0fb-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb0fb-152">DateTimeOffset</span></span>|<span data-ttu-id="bb0fb-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-153">The date and time the app was created.</span></span> <span data-ttu-id="bb0fb-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb0fb-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb0fb-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb0fb-155">lastModifiedDateTime</span></span>|<span data-ttu-id="bb0fb-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb0fb-156">DateTimeOffset</span></span>|<span data-ttu-id="bb0fb-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-157">The date and time the app was last modified.</span></span> <span data-ttu-id="bb0fb-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb0fb-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb0fb-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="bb0fb-159">isFeatured</span></span>|<span data-ttu-id="bb0fb-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb0fb-160">Boolean</span></span>|<span data-ttu-id="bb0fb-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb0fb-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb0fb-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="bb0fb-162">privacyInformationUrl</span></span>|<span data-ttu-id="bb0fb-163">String</span><span class="sxs-lookup"><span data-stu-id="bb0fb-163">String</span></span>|<span data-ttu-id="bb0fb-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-164">The privacy statement Url.</span></span> <span data-ttu-id="bb0fb-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb0fb-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb0fb-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="bb0fb-166">informationUrl</span></span>|<span data-ttu-id="bb0fb-167">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bb0fb-167">String</span></span>|<span data-ttu-id="bb0fb-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-168">The more information Url.</span></span> <span data-ttu-id="bb0fb-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb0fb-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb0fb-170">owner</span><span class="sxs-lookup"><span data-stu-id="bb0fb-170">owner</span></span>|<span data-ttu-id="bb0fb-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bb0fb-171">String</span></span>|<span data-ttu-id="bb0fb-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-172">The owner of the app.</span></span> <span data-ttu-id="bb0fb-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb0fb-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb0fb-174">developer</span><span class="sxs-lookup"><span data-stu-id="bb0fb-174">developer</span></span>|<span data-ttu-id="bb0fb-175">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bb0fb-175">String</span></span>|<span data-ttu-id="bb0fb-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-176">The developer of the app.</span></span> <span data-ttu-id="bb0fb-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb0fb-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb0fb-178">notes</span><span class="sxs-lookup"><span data-stu-id="bb0fb-178">notes</span></span>|<span data-ttu-id="bb0fb-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bb0fb-179">String</span></span>|<span data-ttu-id="bb0fb-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-180">Notes for the app.</span></span> <span data-ttu-id="bb0fb-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb0fb-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb0fb-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="bb0fb-182">publishingState</span></span>|[<span data-ttu-id="bb0fb-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="bb0fb-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="bb0fb-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-184">The publishing state for the app.</span></span> <span data-ttu-id="bb0fb-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="bb0fb-186">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="bb0fb-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="bb0fb-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="bb0fb-188">appAvailability</span></span>|[<span data-ttu-id="bb0fb-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="bb0fb-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="bb0fb-190">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-190">The Application's availability.</span></span> <span data-ttu-id="bb0fb-191">Von [ManagedApp](../resources/intune-apps-managedapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="bb0fb-192">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="bb0fb-193">version</span><span class="sxs-lookup"><span data-stu-id="bb0fb-193">version</span></span>|<span data-ttu-id="bb0fb-194">String</span><span class="sxs-lookup"><span data-stu-id="bb0fb-194">String</span></span>|<span data-ttu-id="bb0fb-195">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-195">The Application's version.</span></span> <span data-ttu-id="bb0fb-196">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb0fb-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="bb0fb-197">bundleId</span><span class="sxs-lookup"><span data-stu-id="bb0fb-197">bundleId</span></span>|<span data-ttu-id="bb0fb-198">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bb0fb-198">String</span></span>|<span data-ttu-id="bb0fb-199">Die Bundle-ID einer App.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-199">The app's Bundle ID.</span></span>|
|<span data-ttu-id="bb0fb-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="bb0fb-200">appStoreUrl</span></span>|<span data-ttu-id="bb0fb-201">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bb0fb-201">String</span></span>|<span data-ttu-id="bb0fb-202">Die URL des Apple-App-Stores.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-202">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="bb0fb-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="bb0fb-203">applicableDeviceType</span></span>|[<span data-ttu-id="bb0fb-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="bb0fb-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="bb0fb-205">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-205">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="bb0fb-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bb0fb-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="bb0fb-207">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bb0fb-207">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="bb0fb-208">Der Wert für die Mindestversion des unterstützten Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-208">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="bb0fb-209">Antwort</span><span class="sxs-lookup"><span data-stu-id="bb0fb-209">Response</span></span>
<span data-ttu-id="bb0fb-210">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-210">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb0fb-211">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bb0fb-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb0fb-212">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bb0fb-212">Request</span></span>
<span data-ttu-id="bb0fb-213">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-213">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bb0fb-214">Antwort</span><span class="sxs-lookup"><span data-stu-id="bb0fb-214">Response</span></span>
<span data-ttu-id="bb0fb-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bb0fb-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



