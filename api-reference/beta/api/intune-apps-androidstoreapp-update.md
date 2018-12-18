---
title: androidStoreApp aktualisieren
description: Aktualisieren der Eigenschaften eines androidStoreApp-Objekts.
author: tfitzmac
ms.openlocfilehash: 3bb27d6ae14dfdde671ddc799e32b8d2ae66982e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330940"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="1b919-103">androidStoreApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1b919-103">Update androidStoreApp</span></span>

> <span data-ttu-id="1b919-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1b919-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b919-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1b919-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1b919-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1b919-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b919-107">Aktualisieren der Eigenschaften eines [androidStoreApp](../resources/intune-apps-androidstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1b919-107">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1b919-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1b919-108">Prerequisites</span></span>
<span data-ttu-id="1b919-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b919-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b919-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1b919-111">Permission type</span></span>|<span data-ttu-id="1b919-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1b919-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b919-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1b919-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1b919-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b919-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1b919-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1b919-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b919-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1b919-116">Not supported.</span></span>|
|<span data-ttu-id="1b919-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1b919-117">Application</span></span>|<span data-ttu-id="1b919-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1b919-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b919-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1b919-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="1b919-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1b919-120">Request headers</span></span>
|<span data-ttu-id="1b919-121">Header</span><span class="sxs-lookup"><span data-stu-id="1b919-121">Header</span></span>|<span data-ttu-id="1b919-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1b919-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b919-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1b919-123">Authorization</span></span>|<span data-ttu-id="1b919-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1b919-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b919-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1b919-125">Accept</span></span>|<span data-ttu-id="1b919-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1b919-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b919-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1b919-127">Request body</span></span>
<span data-ttu-id="1b919-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [androidStoreApp](../resources/intune-apps-androidstoreapp.md) an.</span><span class="sxs-lookup"><span data-stu-id="1b919-128">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="1b919-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [androidStoreApp](../resources/intune-apps-androidstoreapp.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="1b919-129">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="1b919-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1b919-130">Property</span></span>|<span data-ttu-id="1b919-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1b919-131">Type</span></span>|<span data-ttu-id="1b919-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1b919-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b919-133">id</span><span class="sxs-lookup"><span data-stu-id="1b919-133">id</span></span>|<span data-ttu-id="1b919-134">String</span><span class="sxs-lookup"><span data-stu-id="1b919-134">String</span></span>|<span data-ttu-id="1b919-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1b919-135">Key of the entity.</span></span> <span data-ttu-id="1b919-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b919-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b919-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1b919-137">displayName</span></span>|<span data-ttu-id="1b919-138">String</span><span class="sxs-lookup"><span data-stu-id="1b919-138">String</span></span>|<span data-ttu-id="1b919-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="1b919-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1b919-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b919-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b919-141">description</span><span class="sxs-lookup"><span data-stu-id="1b919-141">description</span></span>|<span data-ttu-id="1b919-142">String</span><span class="sxs-lookup"><span data-stu-id="1b919-142">String</span></span>|<span data-ttu-id="1b919-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="1b919-143">The description of the app.</span></span> <span data-ttu-id="1b919-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b919-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b919-145">publisher</span><span class="sxs-lookup"><span data-stu-id="1b919-145">publisher</span></span>|<span data-ttu-id="1b919-146">String</span><span class="sxs-lookup"><span data-stu-id="1b919-146">String</span></span>|<span data-ttu-id="1b919-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="1b919-147">The publisher of the app.</span></span> <span data-ttu-id="1b919-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b919-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b919-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1b919-149">largeIcon</span></span>|[<span data-ttu-id="1b919-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1b919-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1b919-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="1b919-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1b919-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b919-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b919-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b919-153">createdDateTime</span></span>|<span data-ttu-id="1b919-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b919-154">DateTimeOffset</span></span>|<span data-ttu-id="1b919-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="1b919-155">The date and time the app was created.</span></span> <span data-ttu-id="1b919-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b919-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b919-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b919-157">lastModifiedDateTime</span></span>|<span data-ttu-id="1b919-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b919-158">DateTimeOffset</span></span>|<span data-ttu-id="1b919-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="1b919-159">The date and time the app was last modified.</span></span> <span data-ttu-id="1b919-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b919-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b919-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1b919-161">isFeatured</span></span>|<span data-ttu-id="1b919-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1b919-162">Boolean</span></span>|<span data-ttu-id="1b919-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b919-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b919-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1b919-164">privacyInformationUrl</span></span>|<span data-ttu-id="1b919-165">String</span><span class="sxs-lookup"><span data-stu-id="1b919-165">String</span></span>|<span data-ttu-id="1b919-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="1b919-166">The privacy statement Url.</span></span> <span data-ttu-id="1b919-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b919-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b919-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1b919-168">informationUrl</span></span>|<span data-ttu-id="1b919-169">String</span><span class="sxs-lookup"><span data-stu-id="1b919-169">String</span></span>|<span data-ttu-id="1b919-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="1b919-170">The more information Url.</span></span> <span data-ttu-id="1b919-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b919-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b919-172">owner</span><span class="sxs-lookup"><span data-stu-id="1b919-172">owner</span></span>|<span data-ttu-id="1b919-173">String</span><span class="sxs-lookup"><span data-stu-id="1b919-173">String</span></span>|<span data-ttu-id="1b919-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="1b919-174">The owner of the app.</span></span> <span data-ttu-id="1b919-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b919-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b919-176">developer</span><span class="sxs-lookup"><span data-stu-id="1b919-176">developer</span></span>|<span data-ttu-id="1b919-177">String</span><span class="sxs-lookup"><span data-stu-id="1b919-177">String</span></span>|<span data-ttu-id="1b919-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="1b919-178">The developer of the app.</span></span> <span data-ttu-id="1b919-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b919-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b919-180">notes</span><span class="sxs-lookup"><span data-stu-id="1b919-180">notes</span></span>|<span data-ttu-id="1b919-181">String</span><span class="sxs-lookup"><span data-stu-id="1b919-181">String</span></span>|<span data-ttu-id="1b919-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="1b919-182">Notes for the app.</span></span> <span data-ttu-id="1b919-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b919-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b919-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="1b919-184">uploadState</span></span>|<span data-ttu-id="1b919-185">Int32</span><span class="sxs-lookup"><span data-stu-id="1b919-185">Int32</span></span>|<span data-ttu-id="1b919-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="1b919-186">The upload state.</span></span> <span data-ttu-id="1b919-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b919-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b919-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="1b919-188">publishingState</span></span>|[<span data-ttu-id="1b919-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1b919-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1b919-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="1b919-190">The publishing state for the app.</span></span> <span data-ttu-id="1b919-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="1b919-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1b919-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b919-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="1b919-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="1b919-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1b919-194">packageId</span><span class="sxs-lookup"><span data-stu-id="1b919-194">packageId</span></span>|<span data-ttu-id="1b919-195">String</span><span class="sxs-lookup"><span data-stu-id="1b919-195">String</span></span>|<span data-ttu-id="1b919-196">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="1b919-196">The package identifier.</span></span>|
|<span data-ttu-id="1b919-197">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="1b919-197">appIdentifier</span></span>|<span data-ttu-id="1b919-198">String</span><span class="sxs-lookup"><span data-stu-id="1b919-198">String</span></span>|<span data-ttu-id="1b919-199">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="1b919-199">The Identity Name.</span></span>|
|<span data-ttu-id="1b919-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="1b919-200">appStoreUrl</span></span>|<span data-ttu-id="1b919-201">String</span><span class="sxs-lookup"><span data-stu-id="1b919-201">String</span></span>|<span data-ttu-id="1b919-202">URL zum App-Store von Android</span><span class="sxs-lookup"><span data-stu-id="1b919-202">The Android app store URL.</span></span>|
|<span data-ttu-id="1b919-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1b919-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1b919-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1b919-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="1b919-205">Wert, der angibt, welche Betriebssystemversion mindestens erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="1b919-205">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="1b919-206">Antwort</span><span class="sxs-lookup"><span data-stu-id="1b919-206">Response</span></span>
<span data-ttu-id="1b919-207">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [androidStoreApp](../resources/intune-apps-androidstoreapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1b919-207">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b919-208">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1b919-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="1b919-209">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1b919-209">Request</span></span>
<span data-ttu-id="1b919-210">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1b919-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1128

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
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

### <a name="response"></a><span data-ttu-id="1b919-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="1b919-211">Response</span></span>
<span data-ttu-id="1b919-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1b919-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1290

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
  "uploadState": 11,
  "publishingState": "processing",
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
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





