---
title: AndroidManagedStoreApp aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidManagedStoreApp-Objekts.
ms.openlocfilehash: c3c2edde22e1b6538b08930507136e15d470e221
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064112"
---
# <a name="update-androidmanagedstoreapp"></a><span data-ttu-id="cd59b-103">AndroidManagedStoreApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="cd59b-103">Update androidManagedStoreApp</span></span>

> <span data-ttu-id="cd59b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cd59b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd59b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cd59b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cd59b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cd59b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd59b-107">Aktualisieren Sie die Eigenschaften eines [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="cd59b-107">Update the properties of a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cd59b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cd59b-108">Prerequisites</span></span>
<span data-ttu-id="cd59b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd59b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd59b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cd59b-111">Permission type</span></span>|<span data-ttu-id="cd59b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cd59b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd59b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cd59b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cd59b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd59b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cd59b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cd59b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd59b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd59b-116">Not supported.</span></span>|
|<span data-ttu-id="cd59b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cd59b-117">Application</span></span>|<span data-ttu-id="cd59b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd59b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd59b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd59b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="cd59b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cd59b-120">Request headers</span></span>
|<span data-ttu-id="cd59b-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cd59b-121">Header</span></span>|<span data-ttu-id="cd59b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="cd59b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd59b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd59b-123">Authorization</span></span>|<span data-ttu-id="cd59b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cd59b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd59b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cd59b-125">Accept</span></span>|<span data-ttu-id="cd59b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cd59b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd59b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cd59b-127">Request body</span></span>
<span data-ttu-id="cd59b-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="cd59b-128">In the request body, supply a JSON representation for the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

<span data-ttu-id="cd59b-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="cd59b-129">The following table shows the properties that are required when you create the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md).</span></span>

|<span data-ttu-id="cd59b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cd59b-130">Property</span></span>|<span data-ttu-id="cd59b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="cd59b-131">Type</span></span>|<span data-ttu-id="cd59b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cd59b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd59b-133">id</span><span class="sxs-lookup"><span data-stu-id="cd59b-133">id</span></span>|<span data-ttu-id="cd59b-134">String</span><span class="sxs-lookup"><span data-stu-id="cd59b-134">String</span></span>|<span data-ttu-id="cd59b-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="cd59b-135">Key of the entity.</span></span> <span data-ttu-id="cd59b-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd59b-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd59b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="cd59b-137">displayName</span></span>|<span data-ttu-id="cd59b-138">String</span><span class="sxs-lookup"><span data-stu-id="cd59b-138">String</span></span>|<span data-ttu-id="cd59b-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="cd59b-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cd59b-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd59b-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd59b-141">description</span><span class="sxs-lookup"><span data-stu-id="cd59b-141">description</span></span>|<span data-ttu-id="cd59b-142">String</span><span class="sxs-lookup"><span data-stu-id="cd59b-142">String</span></span>|<span data-ttu-id="cd59b-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="cd59b-143">The description of the app.</span></span> <span data-ttu-id="cd59b-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd59b-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd59b-145">publisher</span><span class="sxs-lookup"><span data-stu-id="cd59b-145">publisher</span></span>|<span data-ttu-id="cd59b-146">String</span><span class="sxs-lookup"><span data-stu-id="cd59b-146">String</span></span>|<span data-ttu-id="cd59b-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="cd59b-147">The publisher of the app.</span></span> <span data-ttu-id="cd59b-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd59b-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd59b-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cd59b-149">largeIcon</span></span>|[<span data-ttu-id="cd59b-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cd59b-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cd59b-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="cd59b-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cd59b-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd59b-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd59b-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cd59b-153">createdDateTime</span></span>|<span data-ttu-id="cd59b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd59b-154">DateTimeOffset</span></span>|<span data-ttu-id="cd59b-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="cd59b-155">The date and time the app was created.</span></span> <span data-ttu-id="cd59b-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd59b-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd59b-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd59b-157">lastModifiedDateTime</span></span>|<span data-ttu-id="cd59b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd59b-158">DateTimeOffset</span></span>|<span data-ttu-id="cd59b-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="cd59b-159">The date and time the app was last modified.</span></span> <span data-ttu-id="cd59b-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd59b-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd59b-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cd59b-161">isFeatured</span></span>|<span data-ttu-id="cd59b-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="cd59b-162">Boolean</span></span>|<span data-ttu-id="cd59b-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd59b-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd59b-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cd59b-164">privacyInformationUrl</span></span>|<span data-ttu-id="cd59b-165">String</span><span class="sxs-lookup"><span data-stu-id="cd59b-165">String</span></span>|<span data-ttu-id="cd59b-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="cd59b-166">The privacy statement Url.</span></span> <span data-ttu-id="cd59b-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd59b-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd59b-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cd59b-168">informationUrl</span></span>|<span data-ttu-id="cd59b-169">String</span><span class="sxs-lookup"><span data-stu-id="cd59b-169">String</span></span>|<span data-ttu-id="cd59b-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="cd59b-170">The more information Url.</span></span> <span data-ttu-id="cd59b-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd59b-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd59b-172">owner</span><span class="sxs-lookup"><span data-stu-id="cd59b-172">owner</span></span>|<span data-ttu-id="cd59b-173">String</span><span class="sxs-lookup"><span data-stu-id="cd59b-173">String</span></span>|<span data-ttu-id="cd59b-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="cd59b-174">The owner of the app.</span></span> <span data-ttu-id="cd59b-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd59b-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd59b-176">developer</span><span class="sxs-lookup"><span data-stu-id="cd59b-176">developer</span></span>|<span data-ttu-id="cd59b-177">String</span><span class="sxs-lookup"><span data-stu-id="cd59b-177">String</span></span>|<span data-ttu-id="cd59b-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="cd59b-178">The developer of the app.</span></span> <span data-ttu-id="cd59b-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd59b-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd59b-180">notes</span><span class="sxs-lookup"><span data-stu-id="cd59b-180">notes</span></span>|<span data-ttu-id="cd59b-181">String</span><span class="sxs-lookup"><span data-stu-id="cd59b-181">String</span></span>|<span data-ttu-id="cd59b-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="cd59b-182">Notes for the app.</span></span> <span data-ttu-id="cd59b-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd59b-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd59b-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="cd59b-184">uploadState</span></span>|<span data-ttu-id="cd59b-185">Int32</span><span class="sxs-lookup"><span data-stu-id="cd59b-185">Int32</span></span>|<span data-ttu-id="cd59b-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="cd59b-186">The upload state.</span></span> <span data-ttu-id="cd59b-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd59b-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cd59b-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="cd59b-188">publishingState</span></span>|[<span data-ttu-id="cd59b-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="cd59b-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="cd59b-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="cd59b-190">The publishing state for the app.</span></span> <span data-ttu-id="cd59b-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="cd59b-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cd59b-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd59b-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="cd59b-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="cd59b-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cd59b-194">packageId</span><span class="sxs-lookup"><span data-stu-id="cd59b-194">packageId</span></span>|<span data-ttu-id="cd59b-195">String</span><span class="sxs-lookup"><span data-stu-id="cd59b-195">String</span></span>|<span data-ttu-id="cd59b-196">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="cd59b-196">The package identifier.</span></span>|
|<span data-ttu-id="cd59b-197">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="cd59b-197">appIdentifier</span></span>|<span data-ttu-id="cd59b-198">String</span><span class="sxs-lookup"><span data-stu-id="cd59b-198">String</span></span>|<span data-ttu-id="cd59b-199">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="cd59b-199">The Identity Name.</span></span>|
|<span data-ttu-id="cd59b-200">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="cd59b-200">usedLicenseCount</span></span>|<span data-ttu-id="cd59b-201">Int32</span><span class="sxs-lookup"><span data-stu-id="cd59b-201">Int32</span></span>|<span data-ttu-id="cd59b-202">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="cd59b-202">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="cd59b-203">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="cd59b-203">totalLicenseCount</span></span>|<span data-ttu-id="cd59b-204">Int32</span><span class="sxs-lookup"><span data-stu-id="cd59b-204">Int32</span></span>|<span data-ttu-id="cd59b-205">Gesamtanzahl von VPP-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="cd59b-205">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="cd59b-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="cd59b-206">appStoreUrl</span></span>|<span data-ttu-id="cd59b-207">String</span><span class="sxs-lookup"><span data-stu-id="cd59b-207">String</span></span>|<span data-ttu-id="cd59b-208">Wiedergeben für Arbeit Store-app-URL.</span><span class="sxs-lookup"><span data-stu-id="cd59b-208">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="cd59b-209">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd59b-209">Response</span></span>
<span data-ttu-id="cd59b-210">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="cd59b-210">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd59b-211">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cd59b-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="cd59b-212">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd59b-212">Request</span></span>
<span data-ttu-id="cd59b-213">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cd59b-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 799

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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="cd59b-214">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd59b-214">Response</span></span>
<span data-ttu-id="cd59b-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd59b-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 968

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
  "id": "87247525-7525-8724-2575-248725752487",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```





