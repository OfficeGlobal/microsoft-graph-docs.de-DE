---
title: microsoftStoreForBusinessApp aktualisieren
description: Aktualisieren der Eigenschaften eines microsoftStoreForBusinessApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9acbb9b500f9d4a77e0a9b3cb33746ac3db31b3d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962785"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="e467b-103">microsoftStoreForBusinessApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e467b-103">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="e467b-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e467b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e467b-105">Aktualisieren der Eigenschaften eines [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e467b-105">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e467b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e467b-106">Prerequisites</span></span>
<span data-ttu-id="e467b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e467b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e467b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e467b-109">Permission type</span></span>|<span data-ttu-id="e467b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e467b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e467b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e467b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e467b-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e467b-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e467b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e467b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e467b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e467b-114">Not supported.</span></span>|
|<span data-ttu-id="e467b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e467b-115">Application</span></span>|<span data-ttu-id="e467b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e467b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e467b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e467b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="e467b-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e467b-118">Request headers</span></span>
|<span data-ttu-id="e467b-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e467b-119">Header</span></span>|<span data-ttu-id="e467b-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e467b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e467b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e467b-121">Authorization</span></span>|<span data-ttu-id="e467b-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e467b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e467b-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e467b-123">Accept</span></span>|<span data-ttu-id="e467b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e467b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e467b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e467b-125">Request body</span></span>
<span data-ttu-id="e467b-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="e467b-126">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="e467b-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e467b-127">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="e467b-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e467b-128">Property</span></span>|<span data-ttu-id="e467b-129">Typ</span><span class="sxs-lookup"><span data-stu-id="e467b-129">Type</span></span>|<span data-ttu-id="e467b-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e467b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e467b-131">id</span><span class="sxs-lookup"><span data-stu-id="e467b-131">id</span></span>|<span data-ttu-id="e467b-132">String</span><span class="sxs-lookup"><span data-stu-id="e467b-132">String</span></span>|<span data-ttu-id="e467b-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e467b-133">Key of the entity.</span></span> <span data-ttu-id="e467b-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e467b-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e467b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e467b-135">displayName</span></span>|<span data-ttu-id="e467b-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e467b-136">String</span></span>|<span data-ttu-id="e467b-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="e467b-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e467b-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e467b-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e467b-139">description</span><span class="sxs-lookup"><span data-stu-id="e467b-139">description</span></span>|<span data-ttu-id="e467b-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e467b-140">String</span></span>|<span data-ttu-id="e467b-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="e467b-141">The description of the app.</span></span> <span data-ttu-id="e467b-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e467b-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e467b-143">publisher</span><span class="sxs-lookup"><span data-stu-id="e467b-143">publisher</span></span>|<span data-ttu-id="e467b-144">String</span><span class="sxs-lookup"><span data-stu-id="e467b-144">String</span></span>|<span data-ttu-id="e467b-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="e467b-145">The publisher of the app.</span></span> <span data-ttu-id="e467b-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e467b-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e467b-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e467b-147">largeIcon</span></span>|[<span data-ttu-id="e467b-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e467b-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e467b-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="e467b-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e467b-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e467b-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e467b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e467b-151">createdDateTime</span></span>|<span data-ttu-id="e467b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e467b-152">DateTimeOffset</span></span>|<span data-ttu-id="e467b-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="e467b-153">The date and time the app was created.</span></span> <span data-ttu-id="e467b-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e467b-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e467b-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e467b-155">lastModifiedDateTime</span></span>|<span data-ttu-id="e467b-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e467b-156">DateTimeOffset</span></span>|<span data-ttu-id="e467b-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="e467b-157">The date and time the app was last modified.</span></span> <span data-ttu-id="e467b-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e467b-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e467b-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e467b-159">isFeatured</span></span>|<span data-ttu-id="e467b-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="e467b-160">Boolean</span></span>|<span data-ttu-id="e467b-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e467b-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e467b-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e467b-162">privacyInformationUrl</span></span>|<span data-ttu-id="e467b-163">String</span><span class="sxs-lookup"><span data-stu-id="e467b-163">String</span></span>|<span data-ttu-id="e467b-164">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="e467b-164">The privacy statement Url.</span></span> <span data-ttu-id="e467b-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e467b-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e467b-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e467b-166">informationUrl</span></span>|<span data-ttu-id="e467b-167">String</span><span class="sxs-lookup"><span data-stu-id="e467b-167">String</span></span>|<span data-ttu-id="e467b-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="e467b-168">The more information Url.</span></span> <span data-ttu-id="e467b-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e467b-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e467b-170">owner</span><span class="sxs-lookup"><span data-stu-id="e467b-170">owner</span></span>|<span data-ttu-id="e467b-171">String</span><span class="sxs-lookup"><span data-stu-id="e467b-171">String</span></span>|<span data-ttu-id="e467b-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="e467b-172">The owner of the app.</span></span> <span data-ttu-id="e467b-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e467b-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e467b-174">developer</span><span class="sxs-lookup"><span data-stu-id="e467b-174">developer</span></span>|<span data-ttu-id="e467b-175">String</span><span class="sxs-lookup"><span data-stu-id="e467b-175">String</span></span>|<span data-ttu-id="e467b-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="e467b-176">The developer of the app.</span></span> <span data-ttu-id="e467b-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e467b-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e467b-178">notes</span><span class="sxs-lookup"><span data-stu-id="e467b-178">notes</span></span>|<span data-ttu-id="e467b-179">String</span><span class="sxs-lookup"><span data-stu-id="e467b-179">String</span></span>|<span data-ttu-id="e467b-180">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="e467b-180">Notes for the app.</span></span> <span data-ttu-id="e467b-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e467b-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e467b-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="e467b-182">publishingState</span></span>|[<span data-ttu-id="e467b-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e467b-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e467b-184">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="e467b-184">The publishing state for the app.</span></span> <span data-ttu-id="e467b-185">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="e467b-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e467b-186">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="e467b-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e467b-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="e467b-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e467b-188">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e467b-188">usedLicenseCount</span></span>|<span data-ttu-id="e467b-189">Int32</span><span class="sxs-lookup"><span data-stu-id="e467b-189">Int32</span></span>|<span data-ttu-id="e467b-190">Die Anzahl von verwendeten Microsoft Store für Unternehmen-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="e467b-190">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="e467b-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e467b-191">totalLicenseCount</span></span>|<span data-ttu-id="e467b-192">Int32</span><span class="sxs-lookup"><span data-stu-id="e467b-192">Int32</span></span>|<span data-ttu-id="e467b-193">Die Gesamtzahl der Microsoft Store für Unternehmen-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="e467b-193">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="e467b-194">productKey</span><span class="sxs-lookup"><span data-stu-id="e467b-194">productKey</span></span>|<span data-ttu-id="e467b-195">String</span><span class="sxs-lookup"><span data-stu-id="e467b-195">String</span></span>|<span data-ttu-id="e467b-196">Der Product Key der App</span><span class="sxs-lookup"><span data-stu-id="e467b-196">The app product key</span></span>|
|<span data-ttu-id="e467b-197">licenseType</span><span class="sxs-lookup"><span data-stu-id="e467b-197">licenseType</span></span>|[<span data-ttu-id="e467b-198">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="e467b-198">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="e467b-199">Der APP-Lizenztyp.</span><span class="sxs-lookup"><span data-stu-id="e467b-199">The app license type.</span></span> <span data-ttu-id="e467b-200">Mögliche Werte sind: `offline` und `online`.</span><span class="sxs-lookup"><span data-stu-id="e467b-200">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="e467b-201">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="e467b-201">packageIdentityName</span></span>|<span data-ttu-id="e467b-202">String</span><span class="sxs-lookup"><span data-stu-id="e467b-202">String</span></span>|<span data-ttu-id="e467b-203">Bezeichner des App-Pakets</span><span class="sxs-lookup"><span data-stu-id="e467b-203">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="e467b-204">Antwort</span><span class="sxs-lookup"><span data-stu-id="e467b-204">Response</span></span>
<span data-ttu-id="e467b-205">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e467b-205">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e467b-206">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e467b-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="e467b-207">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e467b-207">Request</span></span>
<span data-ttu-id="e467b-208">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e467b-208">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="e467b-209">Antwort</span><span class="sxs-lookup"><span data-stu-id="e467b-209">Response</span></span>
<span data-ttu-id="e467b-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e467b-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



