---
title: Erstellen von androidForWorkApp
description: Erstellen eines neuen AndroidForWorkApp-Objekts.
author: tfitzmac
ms.openlocfilehash: d88346184c1eee294c9cff2abe8274493d57ebef
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340873"
---
# <a name="create-androidforworkapp"></a><span data-ttu-id="7bdbf-103">Erstellen von androidForWorkApp</span><span class="sxs-lookup"><span data-stu-id="7bdbf-103">Create androidForWorkApp</span></span>

> <span data-ttu-id="7bdbf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7bdbf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7bdbf-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7bdbf-107">Erstellen eines neuen [AndroidForWorkApp](../resources/intune-apps-androidforworkapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-107">Create a new [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7bdbf-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7bdbf-108">Prerequisites</span></span>
<span data-ttu-id="7bdbf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bdbf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bdbf-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7bdbf-111">Permission type</span></span>|<span data-ttu-id="7bdbf-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7bdbf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bdbf-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7bdbf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7bdbf-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bdbf-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7bdbf-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7bdbf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7bdbf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7bdbf-116">Not supported.</span></span>|
|<span data-ttu-id="7bdbf-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7bdbf-117">Application</span></span>|<span data-ttu-id="7bdbf-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7bdbf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bdbf-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7bdbf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="7bdbf-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7bdbf-120">Request headers</span></span>
|<span data-ttu-id="7bdbf-121">Header</span><span class="sxs-lookup"><span data-stu-id="7bdbf-121">Header</span></span>|<span data-ttu-id="7bdbf-122">Wert</span><span class="sxs-lookup"><span data-stu-id="7bdbf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7bdbf-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7bdbf-123">Authorization</span></span>|<span data-ttu-id="7bdbf-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7bdbf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7bdbf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7bdbf-125">Accept</span></span>|<span data-ttu-id="7bdbf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7bdbf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bdbf-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7bdbf-127">Request body</span></span>
<span data-ttu-id="7bdbf-128">Geben Sie im Textkörper Anforderung für das Objekt AndroidForWorkApp eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-128">In the request body, supply a JSON representation for the androidForWorkApp object.</span></span>

<span data-ttu-id="7bdbf-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidForWorkApp erstellen.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-129">The following table shows the properties that are required when you create the androidForWorkApp.</span></span>

|<span data-ttu-id="7bdbf-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7bdbf-130">Property</span></span>|<span data-ttu-id="7bdbf-131">Typ</span><span class="sxs-lookup"><span data-stu-id="7bdbf-131">Type</span></span>|<span data-ttu-id="7bdbf-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7bdbf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bdbf-133">id</span><span class="sxs-lookup"><span data-stu-id="7bdbf-133">id</span></span>|<span data-ttu-id="7bdbf-134">String</span><span class="sxs-lookup"><span data-stu-id="7bdbf-134">String</span></span>|<span data-ttu-id="7bdbf-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7bdbf-135">Key of the entity.</span></span> <span data-ttu-id="7bdbf-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bdbf-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bdbf-137">displayName</span><span class="sxs-lookup"><span data-stu-id="7bdbf-137">displayName</span></span>|<span data-ttu-id="7bdbf-138">String</span><span class="sxs-lookup"><span data-stu-id="7bdbf-138">String</span></span>|<span data-ttu-id="7bdbf-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7bdbf-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bdbf-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bdbf-141">description</span><span class="sxs-lookup"><span data-stu-id="7bdbf-141">description</span></span>|<span data-ttu-id="7bdbf-142">String</span><span class="sxs-lookup"><span data-stu-id="7bdbf-142">String</span></span>|<span data-ttu-id="7bdbf-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-143">The description of the app.</span></span> <span data-ttu-id="7bdbf-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bdbf-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bdbf-145">publisher</span><span class="sxs-lookup"><span data-stu-id="7bdbf-145">publisher</span></span>|<span data-ttu-id="7bdbf-146">String</span><span class="sxs-lookup"><span data-stu-id="7bdbf-146">String</span></span>|<span data-ttu-id="7bdbf-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-147">The publisher of the app.</span></span> <span data-ttu-id="7bdbf-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bdbf-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bdbf-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7bdbf-149">largeIcon</span></span>|[<span data-ttu-id="7bdbf-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7bdbf-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7bdbf-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7bdbf-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bdbf-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bdbf-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7bdbf-153">createdDateTime</span></span>|<span data-ttu-id="7bdbf-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bdbf-154">DateTimeOffset</span></span>|<span data-ttu-id="7bdbf-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-155">The date and time the app was created.</span></span> <span data-ttu-id="7bdbf-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bdbf-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bdbf-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7bdbf-157">lastModifiedDateTime</span></span>|<span data-ttu-id="7bdbf-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bdbf-158">DateTimeOffset</span></span>|<span data-ttu-id="7bdbf-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-159">The date and time the app was last modified.</span></span> <span data-ttu-id="7bdbf-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bdbf-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bdbf-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7bdbf-161">isFeatured</span></span>|<span data-ttu-id="7bdbf-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="7bdbf-162">Boolean</span></span>|<span data-ttu-id="7bdbf-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bdbf-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bdbf-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7bdbf-164">privacyInformationUrl</span></span>|<span data-ttu-id="7bdbf-165">String</span><span class="sxs-lookup"><span data-stu-id="7bdbf-165">String</span></span>|<span data-ttu-id="7bdbf-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-166">The privacy statement Url.</span></span> <span data-ttu-id="7bdbf-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bdbf-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bdbf-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7bdbf-168">informationUrl</span></span>|<span data-ttu-id="7bdbf-169">String</span><span class="sxs-lookup"><span data-stu-id="7bdbf-169">String</span></span>|<span data-ttu-id="7bdbf-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-170">The more information Url.</span></span> <span data-ttu-id="7bdbf-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bdbf-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bdbf-172">owner</span><span class="sxs-lookup"><span data-stu-id="7bdbf-172">owner</span></span>|<span data-ttu-id="7bdbf-173">String</span><span class="sxs-lookup"><span data-stu-id="7bdbf-173">String</span></span>|<span data-ttu-id="7bdbf-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-174">The owner of the app.</span></span> <span data-ttu-id="7bdbf-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bdbf-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bdbf-176">developer</span><span class="sxs-lookup"><span data-stu-id="7bdbf-176">developer</span></span>|<span data-ttu-id="7bdbf-177">String</span><span class="sxs-lookup"><span data-stu-id="7bdbf-177">String</span></span>|<span data-ttu-id="7bdbf-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-178">The developer of the app.</span></span> <span data-ttu-id="7bdbf-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bdbf-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bdbf-180">notes</span><span class="sxs-lookup"><span data-stu-id="7bdbf-180">notes</span></span>|<span data-ttu-id="7bdbf-181">String</span><span class="sxs-lookup"><span data-stu-id="7bdbf-181">String</span></span>|<span data-ttu-id="7bdbf-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-182">Notes for the app.</span></span> <span data-ttu-id="7bdbf-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bdbf-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bdbf-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="7bdbf-184">uploadState</span></span>|<span data-ttu-id="7bdbf-185">Int32</span><span class="sxs-lookup"><span data-stu-id="7bdbf-185">Int32</span></span>|<span data-ttu-id="7bdbf-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-186">The upload state.</span></span> <span data-ttu-id="7bdbf-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bdbf-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7bdbf-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="7bdbf-188">publishingState</span></span>|[<span data-ttu-id="7bdbf-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7bdbf-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7bdbf-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-190">The publishing state for the app.</span></span> <span data-ttu-id="7bdbf-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7bdbf-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7bdbf-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="7bdbf-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7bdbf-194">packageId</span><span class="sxs-lookup"><span data-stu-id="7bdbf-194">packageId</span></span>|<span data-ttu-id="7bdbf-195">String</span><span class="sxs-lookup"><span data-stu-id="7bdbf-195">String</span></span>|<span data-ttu-id="7bdbf-196">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="7bdbf-196">The package identifier.</span></span>|
|<span data-ttu-id="7bdbf-197">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="7bdbf-197">appIdentifier</span></span>|<span data-ttu-id="7bdbf-198">String</span><span class="sxs-lookup"><span data-stu-id="7bdbf-198">String</span></span>|<span data-ttu-id="7bdbf-199">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="7bdbf-199">The Identity Name.</span></span>|
|<span data-ttu-id="7bdbf-200">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="7bdbf-200">usedLicenseCount</span></span>|<span data-ttu-id="7bdbf-201">Int32</span><span class="sxs-lookup"><span data-stu-id="7bdbf-201">Int32</span></span>|<span data-ttu-id="7bdbf-202">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-202">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="7bdbf-203">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="7bdbf-203">totalLicenseCount</span></span>|<span data-ttu-id="7bdbf-204">Int32</span><span class="sxs-lookup"><span data-stu-id="7bdbf-204">Int32</span></span>|<span data-ttu-id="7bdbf-205">Gesamtanzahl von VPP-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-205">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="7bdbf-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="7bdbf-206">appStoreUrl</span></span>|<span data-ttu-id="7bdbf-207">String</span><span class="sxs-lookup"><span data-stu-id="7bdbf-207">String</span></span>|<span data-ttu-id="7bdbf-208">Wiedergeben für Arbeit Store-app-URL.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-208">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="7bdbf-209">Antwort</span><span class="sxs-lookup"><span data-stu-id="7bdbf-209">Response</span></span>
<span data-ttu-id="7bdbf-210">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidForWorkApp](../resources/intune-apps-androidforworkapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-210">If successful, this method returns a `201 Created` response code and a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bdbf-211">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7bdbf-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="7bdbf-212">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7bdbf-212">Request</span></span>
<span data-ttu-id="7bdbf-213">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-213">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 855

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
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

### <a name="response"></a><span data-ttu-id="7bdbf-214">Antwort</span><span class="sxs-lookup"><span data-stu-id="7bdbf-214">Response</span></span>
<span data-ttu-id="7bdbf-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7bdbf-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





