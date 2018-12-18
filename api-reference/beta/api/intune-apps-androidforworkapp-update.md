---
title: AndroidForWorkApp aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidForWorkApp-Objekts.
author: tfitzmac
ms.openlocfilehash: 4697de749fbc4308118c9e82bda839b3871853c9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356049"
---
# <a name="update-androidforworkapp"></a><span data-ttu-id="ef803-103">AndroidForWorkApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ef803-103">Update androidForWorkApp</span></span>

> <span data-ttu-id="ef803-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ef803-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef803-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ef803-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ef803-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ef803-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef803-107">Aktualisieren Sie die Eigenschaften eines [AndroidForWorkApp](../resources/intune-apps-androidforworkapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ef803-107">Update the properties of a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ef803-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ef803-108">Prerequisites</span></span>
<span data-ttu-id="ef803-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef803-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef803-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ef803-111">Permission type</span></span>|<span data-ttu-id="ef803-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ef803-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef803-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ef803-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef803-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef803-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ef803-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ef803-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef803-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ef803-116">Not supported.</span></span>|
|<span data-ttu-id="ef803-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ef803-117">Application</span></span>|<span data-ttu-id="ef803-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ef803-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef803-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef803-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="ef803-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ef803-120">Request headers</span></span>
|<span data-ttu-id="ef803-121">Header</span><span class="sxs-lookup"><span data-stu-id="ef803-121">Header</span></span>|<span data-ttu-id="ef803-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ef803-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef803-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ef803-123">Authorization</span></span>|<span data-ttu-id="ef803-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ef803-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef803-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ef803-125">Accept</span></span>|<span data-ttu-id="ef803-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef803-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef803-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ef803-127">Request body</span></span>
<span data-ttu-id="ef803-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidForWorkApp](../resources/intune-apps-androidforworkapp.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="ef803-128">In the request body, supply a JSON representation for the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

<span data-ttu-id="ef803-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidForWorkApp](../resources/intune-apps-androidforworkapp.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="ef803-129">The following table shows the properties that are required when you create the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md).</span></span>

|<span data-ttu-id="ef803-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ef803-130">Property</span></span>|<span data-ttu-id="ef803-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ef803-131">Type</span></span>|<span data-ttu-id="ef803-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ef803-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef803-133">id</span><span class="sxs-lookup"><span data-stu-id="ef803-133">id</span></span>|<span data-ttu-id="ef803-134">String</span><span class="sxs-lookup"><span data-stu-id="ef803-134">String</span></span>|<span data-ttu-id="ef803-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ef803-135">Key of the entity.</span></span> <span data-ttu-id="ef803-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef803-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef803-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ef803-137">displayName</span></span>|<span data-ttu-id="ef803-138">String</span><span class="sxs-lookup"><span data-stu-id="ef803-138">String</span></span>|<span data-ttu-id="ef803-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="ef803-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ef803-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef803-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef803-141">description</span><span class="sxs-lookup"><span data-stu-id="ef803-141">description</span></span>|<span data-ttu-id="ef803-142">String</span><span class="sxs-lookup"><span data-stu-id="ef803-142">String</span></span>|<span data-ttu-id="ef803-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="ef803-143">The description of the app.</span></span> <span data-ttu-id="ef803-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef803-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef803-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ef803-145">publisher</span></span>|<span data-ttu-id="ef803-146">String</span><span class="sxs-lookup"><span data-stu-id="ef803-146">String</span></span>|<span data-ttu-id="ef803-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="ef803-147">The publisher of the app.</span></span> <span data-ttu-id="ef803-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef803-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef803-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ef803-149">largeIcon</span></span>|[<span data-ttu-id="ef803-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ef803-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ef803-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="ef803-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ef803-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef803-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef803-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef803-153">createdDateTime</span></span>|<span data-ttu-id="ef803-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef803-154">DateTimeOffset</span></span>|<span data-ttu-id="ef803-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="ef803-155">The date and time the app was created.</span></span> <span data-ttu-id="ef803-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef803-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef803-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef803-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ef803-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef803-158">DateTimeOffset</span></span>|<span data-ttu-id="ef803-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="ef803-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ef803-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef803-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef803-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ef803-161">isFeatured</span></span>|<span data-ttu-id="ef803-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ef803-162">Boolean</span></span>|<span data-ttu-id="ef803-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef803-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef803-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ef803-164">privacyInformationUrl</span></span>|<span data-ttu-id="ef803-165">String</span><span class="sxs-lookup"><span data-stu-id="ef803-165">String</span></span>|<span data-ttu-id="ef803-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="ef803-166">The privacy statement Url.</span></span> <span data-ttu-id="ef803-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef803-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef803-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ef803-168">informationUrl</span></span>|<span data-ttu-id="ef803-169">String</span><span class="sxs-lookup"><span data-stu-id="ef803-169">String</span></span>|<span data-ttu-id="ef803-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="ef803-170">The more information Url.</span></span> <span data-ttu-id="ef803-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef803-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef803-172">owner</span><span class="sxs-lookup"><span data-stu-id="ef803-172">owner</span></span>|<span data-ttu-id="ef803-173">String</span><span class="sxs-lookup"><span data-stu-id="ef803-173">String</span></span>|<span data-ttu-id="ef803-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="ef803-174">The owner of the app.</span></span> <span data-ttu-id="ef803-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef803-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef803-176">developer</span><span class="sxs-lookup"><span data-stu-id="ef803-176">developer</span></span>|<span data-ttu-id="ef803-177">String</span><span class="sxs-lookup"><span data-stu-id="ef803-177">String</span></span>|<span data-ttu-id="ef803-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="ef803-178">The developer of the app.</span></span> <span data-ttu-id="ef803-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef803-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef803-180">notes</span><span class="sxs-lookup"><span data-stu-id="ef803-180">notes</span></span>|<span data-ttu-id="ef803-181">String</span><span class="sxs-lookup"><span data-stu-id="ef803-181">String</span></span>|<span data-ttu-id="ef803-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="ef803-182">Notes for the app.</span></span> <span data-ttu-id="ef803-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef803-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef803-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ef803-184">uploadState</span></span>|<span data-ttu-id="ef803-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ef803-185">Int32</span></span>|<span data-ttu-id="ef803-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="ef803-186">The upload state.</span></span> <span data-ttu-id="ef803-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef803-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef803-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="ef803-188">publishingState</span></span>|[<span data-ttu-id="ef803-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ef803-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ef803-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="ef803-190">The publishing state for the app.</span></span> <span data-ttu-id="ef803-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="ef803-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ef803-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef803-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="ef803-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="ef803-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ef803-194">packageId</span><span class="sxs-lookup"><span data-stu-id="ef803-194">packageId</span></span>|<span data-ttu-id="ef803-195">String</span><span class="sxs-lookup"><span data-stu-id="ef803-195">String</span></span>|<span data-ttu-id="ef803-196">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="ef803-196">The package identifier.</span></span>|
|<span data-ttu-id="ef803-197">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="ef803-197">appIdentifier</span></span>|<span data-ttu-id="ef803-198">String</span><span class="sxs-lookup"><span data-stu-id="ef803-198">String</span></span>|<span data-ttu-id="ef803-199">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="ef803-199">The Identity Name.</span></span>|
|<span data-ttu-id="ef803-200">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="ef803-200">usedLicenseCount</span></span>|<span data-ttu-id="ef803-201">Int32</span><span class="sxs-lookup"><span data-stu-id="ef803-201">Int32</span></span>|<span data-ttu-id="ef803-202">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="ef803-202">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="ef803-203">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="ef803-203">totalLicenseCount</span></span>|<span data-ttu-id="ef803-204">Int32</span><span class="sxs-lookup"><span data-stu-id="ef803-204">Int32</span></span>|<span data-ttu-id="ef803-205">Gesamtanzahl von VPP-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="ef803-205">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="ef803-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="ef803-206">appStoreUrl</span></span>|<span data-ttu-id="ef803-207">String</span><span class="sxs-lookup"><span data-stu-id="ef803-207">String</span></span>|<span data-ttu-id="ef803-208">Wiedergeben für Arbeit Store-app-URL.</span><span class="sxs-lookup"><span data-stu-id="ef803-208">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="ef803-209">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef803-209">Response</span></span>
<span data-ttu-id="ef803-210">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidForWorkApp](../resources/intune-apps-androidforworkapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ef803-210">If successful, this method returns a `200 OK` response code and an updated [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef803-211">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ef803-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="ef803-212">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef803-212">Request</span></span>
<span data-ttu-id="ef803-213">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ef803-213">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ef803-214">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef803-214">Response</span></span>
<span data-ttu-id="ef803-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ef803-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 963

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
  "id": "c5010785-0785-c501-8507-01c5850701c5",
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





