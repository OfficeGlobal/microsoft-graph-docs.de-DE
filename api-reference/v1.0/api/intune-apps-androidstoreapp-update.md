---
title: androidStoreApp aktualisieren
description: Aktualisieren der Eigenschaften eines androidStoreApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d233792054166dcb88c2b8a29891ecad13a743de
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847292"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="5c67c-103">androidStoreApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5c67c-103">Update androidStoreApp</span></span>

> <span data-ttu-id="5c67c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5c67c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c67c-105">Aktualisieren der Eigenschaften eines [androidStoreApp](../resources/intune-apps-androidstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5c67c-105">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5c67c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5c67c-106">Prerequisites</span></span>
<span data-ttu-id="5c67c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c67c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c67c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5c67c-109">Permission type</span></span>|<span data-ttu-id="5c67c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5c67c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c67c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5c67c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5c67c-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c67c-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5c67c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5c67c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c67c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5c67c-114">Not supported.</span></span>|
|<span data-ttu-id="5c67c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5c67c-115">Application</span></span>|<span data-ttu-id="5c67c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5c67c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c67c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5c67c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="5c67c-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5c67c-118">Request headers</span></span>
|<span data-ttu-id="5c67c-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5c67c-119">Header</span></span>|<span data-ttu-id="5c67c-120">Wert</span><span class="sxs-lookup"><span data-stu-id="5c67c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c67c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c67c-121">Authorization</span></span>|<span data-ttu-id="5c67c-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5c67c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c67c-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5c67c-123">Accept</span></span>|<span data-ttu-id="5c67c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5c67c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c67c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5c67c-125">Request body</span></span>
<span data-ttu-id="5c67c-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [androidStoreApp](../resources/intune-apps-androidstoreapp.md) an.</span><span class="sxs-lookup"><span data-stu-id="5c67c-126">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="5c67c-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [androidStoreApp](../resources/intune-apps-androidstoreapp.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="5c67c-127">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="5c67c-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5c67c-128">Property</span></span>|<span data-ttu-id="5c67c-129">Typ</span><span class="sxs-lookup"><span data-stu-id="5c67c-129">Type</span></span>|<span data-ttu-id="5c67c-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5c67c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c67c-131">id</span><span class="sxs-lookup"><span data-stu-id="5c67c-131">id</span></span>|<span data-ttu-id="5c67c-132">String</span><span class="sxs-lookup"><span data-stu-id="5c67c-132">String</span></span>|<span data-ttu-id="5c67c-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5c67c-133">Key of the entity.</span></span> <span data-ttu-id="5c67c-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c67c-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c67c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="5c67c-135">displayName</span></span>|<span data-ttu-id="5c67c-136">String</span><span class="sxs-lookup"><span data-stu-id="5c67c-136">String</span></span>|<span data-ttu-id="5c67c-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="5c67c-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5c67c-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c67c-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c67c-139">description</span><span class="sxs-lookup"><span data-stu-id="5c67c-139">description</span></span>|<span data-ttu-id="5c67c-140">String</span><span class="sxs-lookup"><span data-stu-id="5c67c-140">String</span></span>|<span data-ttu-id="5c67c-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="5c67c-141">The description of the app.</span></span> <span data-ttu-id="5c67c-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c67c-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c67c-143">publisher</span><span class="sxs-lookup"><span data-stu-id="5c67c-143">publisher</span></span>|<span data-ttu-id="5c67c-144">String</span><span class="sxs-lookup"><span data-stu-id="5c67c-144">String</span></span>|<span data-ttu-id="5c67c-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="5c67c-145">The publisher of the app.</span></span> <span data-ttu-id="5c67c-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c67c-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c67c-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5c67c-147">largeIcon</span></span>|[<span data-ttu-id="5c67c-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5c67c-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5c67c-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="5c67c-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5c67c-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c67c-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c67c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c67c-151">createdDateTime</span></span>|<span data-ttu-id="5c67c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c67c-152">DateTimeOffset</span></span>|<span data-ttu-id="5c67c-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="5c67c-153">The date and time the app was created.</span></span> <span data-ttu-id="5c67c-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c67c-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c67c-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c67c-155">lastModifiedDateTime</span></span>|<span data-ttu-id="5c67c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c67c-156">DateTimeOffset</span></span>|<span data-ttu-id="5c67c-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="5c67c-157">The date and time the app was last modified.</span></span> <span data-ttu-id="5c67c-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c67c-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c67c-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5c67c-159">isFeatured</span></span>|<span data-ttu-id="5c67c-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c67c-160">Boolean</span></span>|<span data-ttu-id="5c67c-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c67c-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c67c-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5c67c-162">privacyInformationUrl</span></span>|<span data-ttu-id="5c67c-163">String</span><span class="sxs-lookup"><span data-stu-id="5c67c-163">String</span></span>|<span data-ttu-id="5c67c-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="5c67c-164">The privacy statement Url.</span></span> <span data-ttu-id="5c67c-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c67c-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c67c-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5c67c-166">informationUrl</span></span>|<span data-ttu-id="5c67c-167">String</span><span class="sxs-lookup"><span data-stu-id="5c67c-167">String</span></span>|<span data-ttu-id="5c67c-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="5c67c-168">The more information Url.</span></span> <span data-ttu-id="5c67c-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c67c-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c67c-170">owner</span><span class="sxs-lookup"><span data-stu-id="5c67c-170">owner</span></span>|<span data-ttu-id="5c67c-171">String</span><span class="sxs-lookup"><span data-stu-id="5c67c-171">String</span></span>|<span data-ttu-id="5c67c-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="5c67c-172">The owner of the app.</span></span> <span data-ttu-id="5c67c-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c67c-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c67c-174">developer</span><span class="sxs-lookup"><span data-stu-id="5c67c-174">developer</span></span>|<span data-ttu-id="5c67c-175">String</span><span class="sxs-lookup"><span data-stu-id="5c67c-175">String</span></span>|<span data-ttu-id="5c67c-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="5c67c-176">The developer of the app.</span></span> <span data-ttu-id="5c67c-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c67c-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c67c-178">notes</span><span class="sxs-lookup"><span data-stu-id="5c67c-178">notes</span></span>|<span data-ttu-id="5c67c-179">String</span><span class="sxs-lookup"><span data-stu-id="5c67c-179">String</span></span>|<span data-ttu-id="5c67c-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="5c67c-180">Notes for the app.</span></span> <span data-ttu-id="5c67c-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c67c-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c67c-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="5c67c-182">publishingState</span></span>|[<span data-ttu-id="5c67c-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="5c67c-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="5c67c-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="5c67c-184">The publishing state for the app.</span></span> <span data-ttu-id="5c67c-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="5c67c-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5c67c-186">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c67c-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="5c67c-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="5c67c-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5c67c-188">packageId</span><span class="sxs-lookup"><span data-stu-id="5c67c-188">packageId</span></span>|<span data-ttu-id="5c67c-189">String</span><span class="sxs-lookup"><span data-stu-id="5c67c-189">String</span></span>|<span data-ttu-id="5c67c-190">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="5c67c-190">The package identifier.</span></span>|
|<span data-ttu-id="5c67c-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="5c67c-191">appStoreUrl</span></span>|<span data-ttu-id="5c67c-192">String</span><span class="sxs-lookup"><span data-stu-id="5c67c-192">String</span></span>|<span data-ttu-id="5c67c-193">URL zum App-Store von Android</span><span class="sxs-lookup"><span data-stu-id="5c67c-193">The Android app store URL.</span></span>|
|<span data-ttu-id="5c67c-194">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5c67c-194">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="5c67c-195">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5c67c-195">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="5c67c-196">Wert, der angibt, welche Betriebssystemversion mindestens erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="5c67c-196">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="5c67c-197">Antwort</span><span class="sxs-lookup"><span data-stu-id="5c67c-197">Response</span></span>
<span data-ttu-id="5c67c-198">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [androidStoreApp](../resources/intune-apps-androidstoreapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5c67c-198">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c67c-199">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5c67c-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="5c67c-200">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5c67c-200">Request</span></span>
<span data-ttu-id="5c67c-201">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5c67c-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5c67c-202">Antwort</span><span class="sxs-lookup"><span data-stu-id="5c67c-202">Response</span></span>
<span data-ttu-id="5c67c-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5c67c-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



