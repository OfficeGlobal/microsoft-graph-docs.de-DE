---
title: Erstellen von androidManagedStoreApp
description: Erstellen eines neuen AndroidManagedStoreApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 37e59470f8c1bf5cd740aa9ce4d6a09c13a7d5b5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930495"
---
# <a name="create-androidmanagedstoreapp"></a><span data-ttu-id="37f16-103">Erstellen von androidManagedStoreApp</span><span class="sxs-lookup"><span data-stu-id="37f16-103">Create androidManagedStoreApp</span></span>

> <span data-ttu-id="37f16-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="37f16-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37f16-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="37f16-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37f16-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="37f16-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37f16-107">Erstellen eines neuen [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="37f16-107">Create a new [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="37f16-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="37f16-108">Prerequisites</span></span>
<span data-ttu-id="37f16-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37f16-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37f16-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="37f16-111">Permission type</span></span>|<span data-ttu-id="37f16-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="37f16-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37f16-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="37f16-113">Delegated (work or school account)</span></span>|<span data-ttu-id="37f16-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37f16-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="37f16-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="37f16-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37f16-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="37f16-116">Not supported.</span></span>|
|<span data-ttu-id="37f16-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="37f16-117">Application</span></span>|<span data-ttu-id="37f16-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="37f16-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37f16-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="37f16-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="37f16-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="37f16-120">Request headers</span></span>
|<span data-ttu-id="37f16-121">Header</span><span class="sxs-lookup"><span data-stu-id="37f16-121">Header</span></span>|<span data-ttu-id="37f16-122">Wert</span><span class="sxs-lookup"><span data-stu-id="37f16-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37f16-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="37f16-123">Authorization</span></span>|<span data-ttu-id="37f16-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="37f16-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37f16-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="37f16-125">Accept</span></span>|<span data-ttu-id="37f16-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37f16-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37f16-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="37f16-127">Request body</span></span>
<span data-ttu-id="37f16-128">Geben Sie im Textkörper Anforderung für das Objekt AndroidManagedStoreApp eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="37f16-128">In the request body, supply a JSON representation for the androidManagedStoreApp object.</span></span>

<span data-ttu-id="37f16-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die AndroidManagedStoreApp erstellen.</span><span class="sxs-lookup"><span data-stu-id="37f16-129">The following table shows the properties that are required when you create the androidManagedStoreApp.</span></span>

|<span data-ttu-id="37f16-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="37f16-130">Property</span></span>|<span data-ttu-id="37f16-131">Typ</span><span class="sxs-lookup"><span data-stu-id="37f16-131">Type</span></span>|<span data-ttu-id="37f16-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="37f16-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37f16-133">id</span><span class="sxs-lookup"><span data-stu-id="37f16-133">id</span></span>|<span data-ttu-id="37f16-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="37f16-134">String</span></span>|<span data-ttu-id="37f16-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="37f16-135">Key of the entity.</span></span> <span data-ttu-id="37f16-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37f16-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37f16-137">displayName</span><span class="sxs-lookup"><span data-stu-id="37f16-137">displayName</span></span>|<span data-ttu-id="37f16-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="37f16-138">String</span></span>|<span data-ttu-id="37f16-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="37f16-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="37f16-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37f16-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37f16-141">description</span><span class="sxs-lookup"><span data-stu-id="37f16-141">description</span></span>|<span data-ttu-id="37f16-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="37f16-142">String</span></span>|<span data-ttu-id="37f16-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="37f16-143">The description of the app.</span></span> <span data-ttu-id="37f16-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37f16-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37f16-145">publisher</span><span class="sxs-lookup"><span data-stu-id="37f16-145">publisher</span></span>|<span data-ttu-id="37f16-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="37f16-146">String</span></span>|<span data-ttu-id="37f16-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="37f16-147">The publisher of the app.</span></span> <span data-ttu-id="37f16-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37f16-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37f16-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="37f16-149">largeIcon</span></span>|[<span data-ttu-id="37f16-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="37f16-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="37f16-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="37f16-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="37f16-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37f16-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37f16-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="37f16-153">createdDateTime</span></span>|<span data-ttu-id="37f16-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37f16-154">DateTimeOffset</span></span>|<span data-ttu-id="37f16-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="37f16-155">The date and time the app was created.</span></span> <span data-ttu-id="37f16-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37f16-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37f16-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="37f16-157">lastModifiedDateTime</span></span>|<span data-ttu-id="37f16-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37f16-158">DateTimeOffset</span></span>|<span data-ttu-id="37f16-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="37f16-159">The date and time the app was last modified.</span></span> <span data-ttu-id="37f16-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37f16-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37f16-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="37f16-161">isFeatured</span></span>|<span data-ttu-id="37f16-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="37f16-162">Boolean</span></span>|<span data-ttu-id="37f16-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37f16-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37f16-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="37f16-164">privacyInformationUrl</span></span>|<span data-ttu-id="37f16-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="37f16-165">String</span></span>|<span data-ttu-id="37f16-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="37f16-166">The privacy statement Url.</span></span> <span data-ttu-id="37f16-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37f16-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37f16-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="37f16-168">informationUrl</span></span>|<span data-ttu-id="37f16-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="37f16-169">String</span></span>|<span data-ttu-id="37f16-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="37f16-170">The more information Url.</span></span> <span data-ttu-id="37f16-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37f16-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37f16-172">owner</span><span class="sxs-lookup"><span data-stu-id="37f16-172">owner</span></span>|<span data-ttu-id="37f16-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="37f16-173">String</span></span>|<span data-ttu-id="37f16-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="37f16-174">The owner of the app.</span></span> <span data-ttu-id="37f16-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37f16-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37f16-176">developer</span><span class="sxs-lookup"><span data-stu-id="37f16-176">developer</span></span>|<span data-ttu-id="37f16-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="37f16-177">String</span></span>|<span data-ttu-id="37f16-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="37f16-178">The developer of the app.</span></span> <span data-ttu-id="37f16-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37f16-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37f16-180">notes</span><span class="sxs-lookup"><span data-stu-id="37f16-180">notes</span></span>|<span data-ttu-id="37f16-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="37f16-181">String</span></span>|<span data-ttu-id="37f16-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="37f16-182">Notes for the app.</span></span> <span data-ttu-id="37f16-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37f16-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37f16-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="37f16-184">uploadState</span></span>|<span data-ttu-id="37f16-185">Int32</span><span class="sxs-lookup"><span data-stu-id="37f16-185">Int32</span></span>|<span data-ttu-id="37f16-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="37f16-186">The upload state.</span></span> <span data-ttu-id="37f16-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37f16-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37f16-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="37f16-188">publishingState</span></span>|[<span data-ttu-id="37f16-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="37f16-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="37f16-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="37f16-190">The publishing state for the app.</span></span> <span data-ttu-id="37f16-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="37f16-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="37f16-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37f16-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="37f16-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="37f16-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="37f16-194">packageId</span><span class="sxs-lookup"><span data-stu-id="37f16-194">packageId</span></span>|<span data-ttu-id="37f16-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="37f16-195">String</span></span>|<span data-ttu-id="37f16-196">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="37f16-196">The package identifier.</span></span>|
|<span data-ttu-id="37f16-197">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="37f16-197">appIdentifier</span></span>|<span data-ttu-id="37f16-198">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="37f16-198">String</span></span>|<span data-ttu-id="37f16-199">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="37f16-199">The Identity Name.</span></span>|
|<span data-ttu-id="37f16-200">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="37f16-200">usedLicenseCount</span></span>|<span data-ttu-id="37f16-201">Int32</span><span class="sxs-lookup"><span data-stu-id="37f16-201">Int32</span></span>|<span data-ttu-id="37f16-202">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="37f16-202">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="37f16-203">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="37f16-203">totalLicenseCount</span></span>|<span data-ttu-id="37f16-204">Int32</span><span class="sxs-lookup"><span data-stu-id="37f16-204">Int32</span></span>|<span data-ttu-id="37f16-205">Gesamtanzahl von VPP-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="37f16-205">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="37f16-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="37f16-206">appStoreUrl</span></span>|<span data-ttu-id="37f16-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="37f16-207">String</span></span>|<span data-ttu-id="37f16-208">Wiedergeben für Arbeit Store-app-URL.</span><span class="sxs-lookup"><span data-stu-id="37f16-208">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="37f16-209">Antwort</span><span class="sxs-lookup"><span data-stu-id="37f16-209">Response</span></span>
<span data-ttu-id="37f16-210">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="37f16-210">If successful, this method returns a `201 Created` response code and a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37f16-211">Beispiel</span><span class="sxs-lookup"><span data-stu-id="37f16-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="37f16-212">Anforderung</span><span class="sxs-lookup"><span data-stu-id="37f16-212">Request</span></span>
<span data-ttu-id="37f16-213">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="37f16-213">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 860

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
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

### <a name="response"></a><span data-ttu-id="37f16-214">Antwort</span><span class="sxs-lookup"><span data-stu-id="37f16-214">Response</span></span>
<span data-ttu-id="37f16-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="37f16-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





