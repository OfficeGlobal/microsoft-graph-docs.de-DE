---
title: Erstellen von „androidStoreApp“
description: Diese Methode erstellt ein neues Objekt des Typs androidStoreApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3a7145cc1fb8219e88195a0a951110b91afd18fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894488"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="c1ca3-103">Erstellen von „androidStoreApp“</span><span class="sxs-lookup"><span data-stu-id="c1ca3-103">Create androidStoreApp</span></span>

> <span data-ttu-id="c1ca3-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c1ca3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1ca3-105">Diese Methode erstellt ein neues Objekt des Typs [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1ca3-105">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c1ca3-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c1ca3-106">Prerequisites</span></span>
<span data-ttu-id="c1ca3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1ca3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1ca3-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c1ca3-109">Permission type</span></span>|<span data-ttu-id="c1ca3-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c1ca3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1ca3-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c1ca3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c1ca3-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1ca3-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c1ca3-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c1ca3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1ca3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1ca3-114">Not supported.</span></span>|
|<span data-ttu-id="c1ca3-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c1ca3-115">Application</span></span>|<span data-ttu-id="c1ca3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1ca3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1ca3-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1ca3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c1ca3-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c1ca3-118">Request headers</span></span>
|<span data-ttu-id="c1ca3-119">Header</span><span class="sxs-lookup"><span data-stu-id="c1ca3-119">Header</span></span>|<span data-ttu-id="c1ca3-120">Wert</span><span class="sxs-lookup"><span data-stu-id="c1ca3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1ca3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1ca3-121">Authorization</span></span>|<span data-ttu-id="c1ca3-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c1ca3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1ca3-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c1ca3-123">Accept</span></span>|<span data-ttu-id="c1ca3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c1ca3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1ca3-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c1ca3-125">Request body</span></span>
<span data-ttu-id="c1ca3-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „androidStoreApp“ an.</span><span class="sxs-lookup"><span data-stu-id="c1ca3-126">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="c1ca3-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „androidStoreApp“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="c1ca3-127">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="c1ca3-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c1ca3-128">Property</span></span>|<span data-ttu-id="c1ca3-129">Typ</span><span class="sxs-lookup"><span data-stu-id="c1ca3-129">Type</span></span>|<span data-ttu-id="c1ca3-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1ca3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1ca3-131">id</span><span class="sxs-lookup"><span data-stu-id="c1ca3-131">id</span></span>|<span data-ttu-id="c1ca3-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1ca3-132">String</span></span>|<span data-ttu-id="c1ca3-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c1ca3-133">Key of the entity.</span></span> <span data-ttu-id="c1ca3-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1ca3-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ca3-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c1ca3-135">displayName</span></span>|<span data-ttu-id="c1ca3-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1ca3-136">String</span></span>|<span data-ttu-id="c1ca3-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="c1ca3-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c1ca3-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1ca3-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ca3-139">description</span><span class="sxs-lookup"><span data-stu-id="c1ca3-139">description</span></span>|<span data-ttu-id="c1ca3-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1ca3-140">String</span></span>|<span data-ttu-id="c1ca3-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="c1ca3-141">The description of the app.</span></span> <span data-ttu-id="c1ca3-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1ca3-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ca3-143">publisher</span><span class="sxs-lookup"><span data-stu-id="c1ca3-143">publisher</span></span>|<span data-ttu-id="c1ca3-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1ca3-144">String</span></span>|<span data-ttu-id="c1ca3-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="c1ca3-145">The publisher of the app.</span></span> <span data-ttu-id="c1ca3-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1ca3-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ca3-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c1ca3-147">largeIcon</span></span>|[<span data-ttu-id="c1ca3-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c1ca3-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c1ca3-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1ca3-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c1ca3-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1ca3-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ca3-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c1ca3-151">createdDateTime</span></span>|<span data-ttu-id="c1ca3-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1ca3-152">DateTimeOffset</span></span>|<span data-ttu-id="c1ca3-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="c1ca3-153">The date and time the app was created.</span></span> <span data-ttu-id="c1ca3-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1ca3-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ca3-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1ca3-155">lastModifiedDateTime</span></span>|<span data-ttu-id="c1ca3-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1ca3-156">DateTimeOffset</span></span>|<span data-ttu-id="c1ca3-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="c1ca3-157">The date and time the app was last modified.</span></span> <span data-ttu-id="c1ca3-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1ca3-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ca3-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c1ca3-159">isFeatured</span></span>|<span data-ttu-id="c1ca3-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c1ca3-160">Boolean</span></span>|<span data-ttu-id="c1ca3-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1ca3-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ca3-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c1ca3-162">privacyInformationUrl</span></span>|<span data-ttu-id="c1ca3-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1ca3-163">String</span></span>|<span data-ttu-id="c1ca3-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="c1ca3-164">The privacy statement Url.</span></span> <span data-ttu-id="c1ca3-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1ca3-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ca3-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c1ca3-166">informationUrl</span></span>|<span data-ttu-id="c1ca3-167">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1ca3-167">String</span></span>|<span data-ttu-id="c1ca3-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="c1ca3-168">The more information Url.</span></span> <span data-ttu-id="c1ca3-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1ca3-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ca3-170">owner</span><span class="sxs-lookup"><span data-stu-id="c1ca3-170">owner</span></span>|<span data-ttu-id="c1ca3-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1ca3-171">String</span></span>|<span data-ttu-id="c1ca3-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="c1ca3-172">The owner of the app.</span></span> <span data-ttu-id="c1ca3-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1ca3-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ca3-174">developer</span><span class="sxs-lookup"><span data-stu-id="c1ca3-174">developer</span></span>|<span data-ttu-id="c1ca3-175">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1ca3-175">String</span></span>|<span data-ttu-id="c1ca3-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="c1ca3-176">The developer of the app.</span></span> <span data-ttu-id="c1ca3-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1ca3-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ca3-178">notes</span><span class="sxs-lookup"><span data-stu-id="c1ca3-178">notes</span></span>|<span data-ttu-id="c1ca3-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1ca3-179">String</span></span>|<span data-ttu-id="c1ca3-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="c1ca3-180">Notes for the app.</span></span> <span data-ttu-id="c1ca3-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1ca3-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1ca3-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="c1ca3-182">publishingState</span></span>|[<span data-ttu-id="c1ca3-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c1ca3-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c1ca3-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="c1ca3-184">The publishing state for the app.</span></span> <span data-ttu-id="c1ca3-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="c1ca3-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c1ca3-186">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1ca3-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c1ca3-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="c1ca3-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c1ca3-188">packageId</span><span class="sxs-lookup"><span data-stu-id="c1ca3-188">packageId</span></span>|<span data-ttu-id="c1ca3-189">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1ca3-189">String</span></span>|<span data-ttu-id="c1ca3-190">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="c1ca3-190">The package identifier.</span></span>|
|<span data-ttu-id="c1ca3-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="c1ca3-191">appStoreUrl</span></span>|<span data-ttu-id="c1ca3-192">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1ca3-192">String</span></span>|<span data-ttu-id="c1ca3-193">URL zum App-Store von Android</span><span class="sxs-lookup"><span data-stu-id="c1ca3-193">The Android app store URL.</span></span>|
|<span data-ttu-id="c1ca3-194">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c1ca3-194">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c1ca3-195">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c1ca3-195">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="c1ca3-196">Wert, der angibt, welche Betriebssystemversion mindestens erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="c1ca3-196">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="c1ca3-197">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1ca3-197">Response</span></span>
<span data-ttu-id="c1ca3-198">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [androidStoreApp](../resources/intune-apps-androidstoreapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c1ca3-198">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1ca3-199">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1ca3-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="c1ca3-200">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1ca3-200">Request</span></span>
<span data-ttu-id="c1ca3-201">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c1ca3-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 938

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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

### <a name="response"></a><span data-ttu-id="c1ca3-202">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1ca3-202">Response</span></span>
<span data-ttu-id="c1ca3-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1ca3-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1110

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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



