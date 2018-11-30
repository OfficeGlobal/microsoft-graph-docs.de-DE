---
title: microsoftStoreForBusinessApp erstellen
description: Erstellen eines neuen microsoftStoreForBusinessApp-Objekts.
ms.openlocfilehash: 478bf95892628b4b3bc0195804a48c9d9cf415e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016965"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="a2ead-103">microsoftStoreForBusinessApp erstellen</span><span class="sxs-lookup"><span data-stu-id="a2ead-103">Create microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="a2ead-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a2ead-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2ead-105">Erstellen eines neuen [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a2ead-105">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a2ead-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a2ead-106">Prerequisites</span></span>
<span data-ttu-id="a2ead-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2ead-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2ead-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a2ead-109">Permission type</span></span>|<span data-ttu-id="a2ead-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a2ead-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2ead-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a2ead-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a2ead-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2ead-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a2ead-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a2ead-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2ead-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2ead-114">Not supported.</span></span>|
|<span data-ttu-id="a2ead-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a2ead-115">Application</span></span>|<span data-ttu-id="a2ead-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2ead-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2ead-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2ead-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a2ead-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a2ead-118">Request headers</span></span>
|<span data-ttu-id="a2ead-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a2ead-119">Header</span></span>|<span data-ttu-id="a2ead-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a2ead-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2ead-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2ead-121">Authorization</span></span>|<span data-ttu-id="a2ead-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a2ead-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2ead-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a2ead-123">Accept</span></span>|<span data-ttu-id="a2ead-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a2ead-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2ead-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a2ead-125">Request body</span></span>
<span data-ttu-id="a2ead-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das microsoftStoreForBusinessApp-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="a2ead-126">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="a2ead-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der microsoftStoreForBusinessApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="a2ead-127">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="a2ead-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a2ead-128">Property</span></span>|<span data-ttu-id="a2ead-129">Typ</span><span class="sxs-lookup"><span data-stu-id="a2ead-129">Type</span></span>|<span data-ttu-id="a2ead-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a2ead-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2ead-131">id</span><span class="sxs-lookup"><span data-stu-id="a2ead-131">id</span></span>|<span data-ttu-id="a2ead-132">String</span><span class="sxs-lookup"><span data-stu-id="a2ead-132">String</span></span>|<span data-ttu-id="a2ead-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a2ead-133">Key of the entity.</span></span> <span data-ttu-id="a2ead-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2ead-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2ead-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a2ead-135">displayName</span></span>|<span data-ttu-id="a2ead-136">String</span><span class="sxs-lookup"><span data-stu-id="a2ead-136">String</span></span>|<span data-ttu-id="a2ead-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="a2ead-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a2ead-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2ead-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2ead-139">description</span><span class="sxs-lookup"><span data-stu-id="a2ead-139">description</span></span>|<span data-ttu-id="a2ead-140">String</span><span class="sxs-lookup"><span data-stu-id="a2ead-140">String</span></span>|<span data-ttu-id="a2ead-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="a2ead-141">The description of the app.</span></span> <span data-ttu-id="a2ead-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2ead-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2ead-143">publisher</span><span class="sxs-lookup"><span data-stu-id="a2ead-143">publisher</span></span>|<span data-ttu-id="a2ead-144">String</span><span class="sxs-lookup"><span data-stu-id="a2ead-144">String</span></span>|<span data-ttu-id="a2ead-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="a2ead-145">The publisher of the app.</span></span> <span data-ttu-id="a2ead-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2ead-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2ead-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a2ead-147">largeIcon</span></span>|[<span data-ttu-id="a2ead-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a2ead-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a2ead-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="a2ead-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a2ead-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2ead-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2ead-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2ead-151">createdDateTime</span></span>|<span data-ttu-id="a2ead-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2ead-152">DateTimeOffset</span></span>|<span data-ttu-id="a2ead-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="a2ead-153">The date and time the app was created.</span></span> <span data-ttu-id="a2ead-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2ead-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2ead-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2ead-155">lastModifiedDateTime</span></span>|<span data-ttu-id="a2ead-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2ead-156">DateTimeOffset</span></span>|<span data-ttu-id="a2ead-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="a2ead-157">The date and time the app was last modified.</span></span> <span data-ttu-id="a2ead-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2ead-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2ead-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a2ead-159">isFeatured</span></span>|<span data-ttu-id="a2ead-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a2ead-160">Boolean</span></span>|<span data-ttu-id="a2ead-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2ead-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2ead-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a2ead-162">privacyInformationUrl</span></span>|<span data-ttu-id="a2ead-163">String</span><span class="sxs-lookup"><span data-stu-id="a2ead-163">String</span></span>|<span data-ttu-id="a2ead-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="a2ead-164">The privacy statement Url.</span></span> <span data-ttu-id="a2ead-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2ead-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2ead-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a2ead-166">informationUrl</span></span>|<span data-ttu-id="a2ead-167">String</span><span class="sxs-lookup"><span data-stu-id="a2ead-167">String</span></span>|<span data-ttu-id="a2ead-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="a2ead-168">The more information Url.</span></span> <span data-ttu-id="a2ead-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2ead-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2ead-170">owner</span><span class="sxs-lookup"><span data-stu-id="a2ead-170">owner</span></span>|<span data-ttu-id="a2ead-171">String</span><span class="sxs-lookup"><span data-stu-id="a2ead-171">String</span></span>|<span data-ttu-id="a2ead-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="a2ead-172">The owner of the app.</span></span> <span data-ttu-id="a2ead-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2ead-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2ead-174">developer</span><span class="sxs-lookup"><span data-stu-id="a2ead-174">developer</span></span>|<span data-ttu-id="a2ead-175">String</span><span class="sxs-lookup"><span data-stu-id="a2ead-175">String</span></span>|<span data-ttu-id="a2ead-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="a2ead-176">The developer of the app.</span></span> <span data-ttu-id="a2ead-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2ead-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2ead-178">notes</span><span class="sxs-lookup"><span data-stu-id="a2ead-178">notes</span></span>|<span data-ttu-id="a2ead-179">String</span><span class="sxs-lookup"><span data-stu-id="a2ead-179">String</span></span>|<span data-ttu-id="a2ead-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="a2ead-180">Notes for the app.</span></span> <span data-ttu-id="a2ead-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2ead-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2ead-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="a2ead-182">publishingState</span></span>|[<span data-ttu-id="a2ead-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a2ead-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a2ead-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="a2ead-184">The publishing state for the app.</span></span> <span data-ttu-id="a2ead-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="a2ead-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a2ead-186">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2ead-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a2ead-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="a2ead-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a2ead-188">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="a2ead-188">usedLicenseCount</span></span>|<span data-ttu-id="a2ead-189">Int32</span><span class="sxs-lookup"><span data-stu-id="a2ead-189">Int32</span></span>|<span data-ttu-id="a2ead-190">Die Anzahl von verwendeten Microsoft Store für Unternehmen-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="a2ead-190">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="a2ead-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="a2ead-191">totalLicenseCount</span></span>|<span data-ttu-id="a2ead-192">Int32</span><span class="sxs-lookup"><span data-stu-id="a2ead-192">Int32</span></span>|<span data-ttu-id="a2ead-193">Die Gesamtzahl der Microsoft Store für Unternehmen-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="a2ead-193">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="a2ead-194">productKey</span><span class="sxs-lookup"><span data-stu-id="a2ead-194">productKey</span></span>|<span data-ttu-id="a2ead-195">String</span><span class="sxs-lookup"><span data-stu-id="a2ead-195">String</span></span>|<span data-ttu-id="a2ead-196">Der Product Key der App</span><span class="sxs-lookup"><span data-stu-id="a2ead-196">The app product key</span></span>|
|<span data-ttu-id="a2ead-197">licenseType</span><span class="sxs-lookup"><span data-stu-id="a2ead-197">licenseType</span></span>|[<span data-ttu-id="a2ead-198">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="a2ead-198">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="a2ead-199">Der Typ des app-Lizenz.</span><span class="sxs-lookup"><span data-stu-id="a2ead-199">The app license type.</span></span> <span data-ttu-id="a2ead-200">Mögliche Werte sind: `offline` und `online`.</span><span class="sxs-lookup"><span data-stu-id="a2ead-200">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="a2ead-201">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="a2ead-201">packageIdentityName</span></span>|<span data-ttu-id="a2ead-202">String</span><span class="sxs-lookup"><span data-stu-id="a2ead-202">String</span></span>|<span data-ttu-id="a2ead-203">Bezeichner des App-Pakets</span><span class="sxs-lookup"><span data-stu-id="a2ead-203">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="a2ead-204">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2ead-204">Response</span></span>
<span data-ttu-id="a2ead-205">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a2ead-205">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2ead-206">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a2ead-206">Example</span></span>
### <a name="request"></a><span data-ttu-id="a2ead-207">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2ead-207">Request</span></span>
<span data-ttu-id="a2ead-208">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a2ead-208">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 769

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```

### <a name="response"></a><span data-ttu-id="a2ead-209">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2ead-209">Response</span></span>
<span data-ttu-id="a2ead-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a2ead-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 941

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```


