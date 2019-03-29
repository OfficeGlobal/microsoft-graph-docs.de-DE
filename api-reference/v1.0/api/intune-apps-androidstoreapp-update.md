---
title: androidStoreApp aktualisieren
description: Aktualisieren der Eigenschaften eines androidStoreApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0408720fc5f8140e11728d7f367f738ca7636aa3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962106"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="37ad8-103">androidStoreApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="37ad8-103">Update androidStoreApp</span></span>

> <span data-ttu-id="37ad8-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="37ad8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37ad8-105">Aktualisieren der Eigenschaften eines [androidStoreApp](../resources/intune-apps-androidstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="37ad8-105">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37ad8-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="37ad8-106">Prerequisites</span></span>
<span data-ttu-id="37ad8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37ad8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37ad8-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="37ad8-109">Permission type</span></span>|<span data-ttu-id="37ad8-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="37ad8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37ad8-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="37ad8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="37ad8-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37ad8-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="37ad8-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="37ad8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37ad8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="37ad8-114">Not supported.</span></span>|
|<span data-ttu-id="37ad8-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="37ad8-115">Application</span></span>|<span data-ttu-id="37ad8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="37ad8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37ad8-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="37ad8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="37ad8-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="37ad8-118">Request headers</span></span>
|<span data-ttu-id="37ad8-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="37ad8-119">Header</span></span>|<span data-ttu-id="37ad8-120">Wert</span><span class="sxs-lookup"><span data-stu-id="37ad8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37ad8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="37ad8-121">Authorization</span></span>|<span data-ttu-id="37ad8-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="37ad8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37ad8-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="37ad8-123">Accept</span></span>|<span data-ttu-id="37ad8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="37ad8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37ad8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="37ad8-125">Request body</span></span>
<span data-ttu-id="37ad8-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [androidStoreApp](../resources/intune-apps-androidstoreapp.md) an.</span><span class="sxs-lookup"><span data-stu-id="37ad8-126">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="37ad8-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [androidStoreApp](../resources/intune-apps-androidstoreapp.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="37ad8-127">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="37ad8-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="37ad8-128">Property</span></span>|<span data-ttu-id="37ad8-129">Typ</span><span class="sxs-lookup"><span data-stu-id="37ad8-129">Type</span></span>|<span data-ttu-id="37ad8-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="37ad8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37ad8-131">id</span><span class="sxs-lookup"><span data-stu-id="37ad8-131">id</span></span>|<span data-ttu-id="37ad8-132">String</span><span class="sxs-lookup"><span data-stu-id="37ad8-132">String</span></span>|<span data-ttu-id="37ad8-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="37ad8-133">Key of the entity.</span></span> <span data-ttu-id="37ad8-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37ad8-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37ad8-135">displayName</span><span class="sxs-lookup"><span data-stu-id="37ad8-135">displayName</span></span>|<span data-ttu-id="37ad8-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="37ad8-136">String</span></span>|<span data-ttu-id="37ad8-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="37ad8-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="37ad8-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37ad8-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37ad8-139">description</span><span class="sxs-lookup"><span data-stu-id="37ad8-139">description</span></span>|<span data-ttu-id="37ad8-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="37ad8-140">String</span></span>|<span data-ttu-id="37ad8-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="37ad8-141">The description of the app.</span></span> <span data-ttu-id="37ad8-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37ad8-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37ad8-143">publisher</span><span class="sxs-lookup"><span data-stu-id="37ad8-143">publisher</span></span>|<span data-ttu-id="37ad8-144">String</span><span class="sxs-lookup"><span data-stu-id="37ad8-144">String</span></span>|<span data-ttu-id="37ad8-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="37ad8-145">The publisher of the app.</span></span> <span data-ttu-id="37ad8-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37ad8-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37ad8-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="37ad8-147">largeIcon</span></span>|[<span data-ttu-id="37ad8-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="37ad8-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="37ad8-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="37ad8-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="37ad8-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37ad8-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37ad8-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="37ad8-151">createdDateTime</span></span>|<span data-ttu-id="37ad8-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37ad8-152">DateTimeOffset</span></span>|<span data-ttu-id="37ad8-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="37ad8-153">The date and time the app was created.</span></span> <span data-ttu-id="37ad8-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37ad8-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37ad8-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="37ad8-155">lastModifiedDateTime</span></span>|<span data-ttu-id="37ad8-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37ad8-156">DateTimeOffset</span></span>|<span data-ttu-id="37ad8-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="37ad8-157">The date and time the app was last modified.</span></span> <span data-ttu-id="37ad8-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37ad8-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37ad8-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="37ad8-159">isFeatured</span></span>|<span data-ttu-id="37ad8-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="37ad8-160">Boolean</span></span>|<span data-ttu-id="37ad8-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37ad8-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37ad8-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="37ad8-162">privacyInformationUrl</span></span>|<span data-ttu-id="37ad8-163">String</span><span class="sxs-lookup"><span data-stu-id="37ad8-163">String</span></span>|<span data-ttu-id="37ad8-164">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="37ad8-164">The privacy statement Url.</span></span> <span data-ttu-id="37ad8-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37ad8-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37ad8-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="37ad8-166">informationUrl</span></span>|<span data-ttu-id="37ad8-167">String</span><span class="sxs-lookup"><span data-stu-id="37ad8-167">String</span></span>|<span data-ttu-id="37ad8-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="37ad8-168">The more information Url.</span></span> <span data-ttu-id="37ad8-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37ad8-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37ad8-170">owner</span><span class="sxs-lookup"><span data-stu-id="37ad8-170">owner</span></span>|<span data-ttu-id="37ad8-171">String</span><span class="sxs-lookup"><span data-stu-id="37ad8-171">String</span></span>|<span data-ttu-id="37ad8-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="37ad8-172">The owner of the app.</span></span> <span data-ttu-id="37ad8-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37ad8-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37ad8-174">developer</span><span class="sxs-lookup"><span data-stu-id="37ad8-174">developer</span></span>|<span data-ttu-id="37ad8-175">String</span><span class="sxs-lookup"><span data-stu-id="37ad8-175">String</span></span>|<span data-ttu-id="37ad8-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="37ad8-176">The developer of the app.</span></span> <span data-ttu-id="37ad8-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37ad8-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37ad8-178">notes</span><span class="sxs-lookup"><span data-stu-id="37ad8-178">notes</span></span>|<span data-ttu-id="37ad8-179">String</span><span class="sxs-lookup"><span data-stu-id="37ad8-179">String</span></span>|<span data-ttu-id="37ad8-180">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="37ad8-180">Notes for the app.</span></span> <span data-ttu-id="37ad8-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37ad8-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37ad8-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="37ad8-182">publishingState</span></span>|[<span data-ttu-id="37ad8-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="37ad8-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="37ad8-184">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="37ad8-184">The publishing state for the app.</span></span> <span data-ttu-id="37ad8-185">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="37ad8-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="37ad8-186">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="37ad8-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="37ad8-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="37ad8-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="37ad8-188">packageId</span><span class="sxs-lookup"><span data-stu-id="37ad8-188">packageId</span></span>|<span data-ttu-id="37ad8-189">String</span><span class="sxs-lookup"><span data-stu-id="37ad8-189">String</span></span>|<span data-ttu-id="37ad8-190">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="37ad8-190">The package identifier.</span></span>|
|<span data-ttu-id="37ad8-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="37ad8-191">appStoreUrl</span></span>|<span data-ttu-id="37ad8-192">String</span><span class="sxs-lookup"><span data-stu-id="37ad8-192">String</span></span>|<span data-ttu-id="37ad8-193">URL zum App-Store von Android</span><span class="sxs-lookup"><span data-stu-id="37ad8-193">The Android app store URL.</span></span>|
|<span data-ttu-id="37ad8-194">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="37ad8-194">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="37ad8-195">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="37ad8-195">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="37ad8-196">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="37ad8-196">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="37ad8-197">Antwort</span><span class="sxs-lookup"><span data-stu-id="37ad8-197">Response</span></span>
<span data-ttu-id="37ad8-198">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [androidStoreApp](../resources/intune-apps-androidstoreapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="37ad8-198">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37ad8-199">Beispiel</span><span class="sxs-lookup"><span data-stu-id="37ad8-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="37ad8-200">Anforderung</span><span class="sxs-lookup"><span data-stu-id="37ad8-200">Request</span></span>
<span data-ttu-id="37ad8-201">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="37ad8-201">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="37ad8-202">Antwort</span><span class="sxs-lookup"><span data-stu-id="37ad8-202">Response</span></span>
<span data-ttu-id="37ad8-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="37ad8-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



