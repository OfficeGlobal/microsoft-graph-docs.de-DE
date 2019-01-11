---
title: androidStoreApp aktualisieren
description: Aktualisieren der Eigenschaften eines androidStoreApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8cd9efebe6d7a68c2b0e023e17e881850e01843f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818837"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="3213a-103">androidStoreApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="3213a-103">Update androidStoreApp</span></span>

> <span data-ttu-id="3213a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3213a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3213a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3213a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3213a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3213a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3213a-107">Aktualisieren der Eigenschaften eines [androidStoreApp](../resources/intune-apps-androidstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3213a-107">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3213a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3213a-108">Prerequisites</span></span>
<span data-ttu-id="3213a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3213a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3213a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3213a-111">Permission type</span></span>|<span data-ttu-id="3213a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3213a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3213a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3213a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3213a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3213a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3213a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3213a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3213a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3213a-116">Not supported.</span></span>|
|<span data-ttu-id="3213a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3213a-117">Application</span></span>|<span data-ttu-id="3213a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3213a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3213a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3213a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="3213a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3213a-120">Request headers</span></span>
|<span data-ttu-id="3213a-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3213a-121">Header</span></span>|<span data-ttu-id="3213a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3213a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3213a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3213a-123">Authorization</span></span>|<span data-ttu-id="3213a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3213a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3213a-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3213a-125">Accept</span></span>|<span data-ttu-id="3213a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3213a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3213a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3213a-127">Request body</span></span>
<span data-ttu-id="3213a-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [androidStoreApp](../resources/intune-apps-androidstoreapp.md) an.</span><span class="sxs-lookup"><span data-stu-id="3213a-128">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="3213a-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [androidStoreApp](../resources/intune-apps-androidstoreapp.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="3213a-129">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="3213a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3213a-130">Property</span></span>|<span data-ttu-id="3213a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="3213a-131">Type</span></span>|<span data-ttu-id="3213a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3213a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3213a-133">id</span><span class="sxs-lookup"><span data-stu-id="3213a-133">id</span></span>|<span data-ttu-id="3213a-134">String</span><span class="sxs-lookup"><span data-stu-id="3213a-134">String</span></span>|<span data-ttu-id="3213a-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3213a-135">Key of the entity.</span></span> <span data-ttu-id="3213a-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3213a-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3213a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3213a-137">displayName</span></span>|<span data-ttu-id="3213a-138">String</span><span class="sxs-lookup"><span data-stu-id="3213a-138">String</span></span>|<span data-ttu-id="3213a-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="3213a-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3213a-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3213a-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3213a-141">description</span><span class="sxs-lookup"><span data-stu-id="3213a-141">description</span></span>|<span data-ttu-id="3213a-142">String</span><span class="sxs-lookup"><span data-stu-id="3213a-142">String</span></span>|<span data-ttu-id="3213a-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="3213a-143">The description of the app.</span></span> <span data-ttu-id="3213a-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3213a-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3213a-145">publisher</span><span class="sxs-lookup"><span data-stu-id="3213a-145">publisher</span></span>|<span data-ttu-id="3213a-146">String</span><span class="sxs-lookup"><span data-stu-id="3213a-146">String</span></span>|<span data-ttu-id="3213a-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="3213a-147">The publisher of the app.</span></span> <span data-ttu-id="3213a-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3213a-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3213a-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3213a-149">largeIcon</span></span>|[<span data-ttu-id="3213a-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3213a-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3213a-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="3213a-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3213a-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3213a-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3213a-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3213a-153">createdDateTime</span></span>|<span data-ttu-id="3213a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3213a-154">DateTimeOffset</span></span>|<span data-ttu-id="3213a-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="3213a-155">The date and time the app was created.</span></span> <span data-ttu-id="3213a-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3213a-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3213a-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3213a-157">lastModifiedDateTime</span></span>|<span data-ttu-id="3213a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3213a-158">DateTimeOffset</span></span>|<span data-ttu-id="3213a-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="3213a-159">The date and time the app was last modified.</span></span> <span data-ttu-id="3213a-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3213a-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3213a-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3213a-161">isFeatured</span></span>|<span data-ttu-id="3213a-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="3213a-162">Boolean</span></span>|<span data-ttu-id="3213a-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3213a-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3213a-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3213a-164">privacyInformationUrl</span></span>|<span data-ttu-id="3213a-165">String</span><span class="sxs-lookup"><span data-stu-id="3213a-165">String</span></span>|<span data-ttu-id="3213a-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="3213a-166">The privacy statement Url.</span></span> <span data-ttu-id="3213a-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3213a-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3213a-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3213a-168">informationUrl</span></span>|<span data-ttu-id="3213a-169">String</span><span class="sxs-lookup"><span data-stu-id="3213a-169">String</span></span>|<span data-ttu-id="3213a-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="3213a-170">The more information Url.</span></span> <span data-ttu-id="3213a-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3213a-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3213a-172">owner</span><span class="sxs-lookup"><span data-stu-id="3213a-172">owner</span></span>|<span data-ttu-id="3213a-173">String</span><span class="sxs-lookup"><span data-stu-id="3213a-173">String</span></span>|<span data-ttu-id="3213a-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="3213a-174">The owner of the app.</span></span> <span data-ttu-id="3213a-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3213a-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3213a-176">developer</span><span class="sxs-lookup"><span data-stu-id="3213a-176">developer</span></span>|<span data-ttu-id="3213a-177">String</span><span class="sxs-lookup"><span data-stu-id="3213a-177">String</span></span>|<span data-ttu-id="3213a-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="3213a-178">The developer of the app.</span></span> <span data-ttu-id="3213a-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3213a-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3213a-180">notes</span><span class="sxs-lookup"><span data-stu-id="3213a-180">notes</span></span>|<span data-ttu-id="3213a-181">String</span><span class="sxs-lookup"><span data-stu-id="3213a-181">String</span></span>|<span data-ttu-id="3213a-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="3213a-182">Notes for the app.</span></span> <span data-ttu-id="3213a-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3213a-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3213a-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="3213a-184">uploadState</span></span>|<span data-ttu-id="3213a-185">Int32</span><span class="sxs-lookup"><span data-stu-id="3213a-185">Int32</span></span>|<span data-ttu-id="3213a-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="3213a-186">The upload state.</span></span> <span data-ttu-id="3213a-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3213a-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3213a-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="3213a-188">publishingState</span></span>|[<span data-ttu-id="3213a-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="3213a-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3213a-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="3213a-190">The publishing state for the app.</span></span> <span data-ttu-id="3213a-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="3213a-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3213a-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3213a-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="3213a-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="3213a-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3213a-194">packageId</span><span class="sxs-lookup"><span data-stu-id="3213a-194">packageId</span></span>|<span data-ttu-id="3213a-195">String</span><span class="sxs-lookup"><span data-stu-id="3213a-195">String</span></span>|<span data-ttu-id="3213a-196">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="3213a-196">The package identifier.</span></span>|
|<span data-ttu-id="3213a-197">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="3213a-197">appIdentifier</span></span>|<span data-ttu-id="3213a-198">String</span><span class="sxs-lookup"><span data-stu-id="3213a-198">String</span></span>|<span data-ttu-id="3213a-199">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="3213a-199">The Identity Name.</span></span>|
|<span data-ttu-id="3213a-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="3213a-200">appStoreUrl</span></span>|<span data-ttu-id="3213a-201">String</span><span class="sxs-lookup"><span data-stu-id="3213a-201">String</span></span>|<span data-ttu-id="3213a-202">URL zum App-Store von Android</span><span class="sxs-lookup"><span data-stu-id="3213a-202">The Android app store URL.</span></span>|
|<span data-ttu-id="3213a-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3213a-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="3213a-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3213a-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="3213a-205">Wert, der angibt, welche Betriebssystemversion mindestens erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="3213a-205">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="3213a-206">Antwort</span><span class="sxs-lookup"><span data-stu-id="3213a-206">Response</span></span>
<span data-ttu-id="3213a-207">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [androidStoreApp](../resources/intune-apps-androidstoreapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3213a-207">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3213a-208">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3213a-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="3213a-209">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3213a-209">Request</span></span>
<span data-ttu-id="3213a-210">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3213a-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3213a-211">Antwort</span><span class="sxs-lookup"><span data-stu-id="3213a-211">Response</span></span>
<span data-ttu-id="3213a-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3213a-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





