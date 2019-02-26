---
title: microsoftStoreForBusinessApp aktualisieren
description: Aktualisieren der Eigenschaften eines microsoftStoreForBusinessApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0bd6cebc6f8aefbeb83b3e9e154f1ca1848e464e
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262937"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="56a13-103">microsoftStoreForBusinessApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="56a13-103">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="56a13-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="56a13-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56a13-105">Aktualisieren der Eigenschaften eines [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="56a13-105">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56a13-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="56a13-106">Prerequisites</span></span>
<span data-ttu-id="56a13-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="56a13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="56a13-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="56a13-109">Permission type</span></span>|<span data-ttu-id="56a13-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="56a13-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56a13-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="56a13-111">Delegated (work or school account)</span></span>|<span data-ttu-id="56a13-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56a13-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="56a13-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="56a13-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56a13-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="56a13-114">Not supported.</span></span>|
|<span data-ttu-id="56a13-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="56a13-115">Application</span></span>|<span data-ttu-id="56a13-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="56a13-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56a13-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="56a13-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="56a13-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="56a13-118">Request headers</span></span>
|<span data-ttu-id="56a13-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="56a13-119">Header</span></span>|<span data-ttu-id="56a13-120">Wert</span><span class="sxs-lookup"><span data-stu-id="56a13-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56a13-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="56a13-121">Authorization</span></span>|<span data-ttu-id="56a13-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="56a13-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56a13-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="56a13-123">Accept</span></span>|<span data-ttu-id="56a13-124">application/json</span><span class="sxs-lookup"><span data-stu-id="56a13-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56a13-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="56a13-125">Request body</span></span>
<span data-ttu-id="56a13-126">Geben Sie im Anforderungstext eine JSON-Darstellung für das [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="56a13-126">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="56a13-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="56a13-127">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="56a13-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="56a13-128">Property</span></span>|<span data-ttu-id="56a13-129">Typ</span><span class="sxs-lookup"><span data-stu-id="56a13-129">Type</span></span>|<span data-ttu-id="56a13-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56a13-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56a13-131">id</span><span class="sxs-lookup"><span data-stu-id="56a13-131">id</span></span>|<span data-ttu-id="56a13-132">string</span><span class="sxs-lookup"><span data-stu-id="56a13-132">String</span></span>|<span data-ttu-id="56a13-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="56a13-133">Key of the entity.</span></span> <span data-ttu-id="56a13-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56a13-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="56a13-135">displayName</span><span class="sxs-lookup"><span data-stu-id="56a13-135">displayName</span></span>|<span data-ttu-id="56a13-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="56a13-136">String</span></span>|<span data-ttu-id="56a13-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="56a13-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="56a13-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56a13-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="56a13-139">description</span><span class="sxs-lookup"><span data-stu-id="56a13-139">description</span></span>|<span data-ttu-id="56a13-140">String</span><span class="sxs-lookup"><span data-stu-id="56a13-140">String</span></span>|<span data-ttu-id="56a13-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="56a13-141">The description of the app.</span></span> <span data-ttu-id="56a13-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56a13-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="56a13-143">publisher</span><span class="sxs-lookup"><span data-stu-id="56a13-143">publisher</span></span>|<span data-ttu-id="56a13-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="56a13-144">String</span></span>|<span data-ttu-id="56a13-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="56a13-145">The publisher of the app.</span></span> <span data-ttu-id="56a13-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56a13-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="56a13-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="56a13-147">largeIcon</span></span>|[<span data-ttu-id="56a13-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="56a13-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="56a13-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="56a13-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="56a13-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56a13-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="56a13-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="56a13-151">createdDateTime</span></span>|<span data-ttu-id="56a13-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56a13-152">DateTimeOffset</span></span>|<span data-ttu-id="56a13-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="56a13-153">The date and time the app was created.</span></span> <span data-ttu-id="56a13-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56a13-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="56a13-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56a13-155">lastModifiedDateTime</span></span>|<span data-ttu-id="56a13-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56a13-156">DateTimeOffset</span></span>|<span data-ttu-id="56a13-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="56a13-157">The date and time the app was last modified.</span></span> <span data-ttu-id="56a13-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56a13-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="56a13-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="56a13-159">isFeatured</span></span>|<span data-ttu-id="56a13-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="56a13-160">Boolean</span></span>|<span data-ttu-id="56a13-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56a13-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="56a13-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="56a13-162">privacyInformationUrl</span></span>|<span data-ttu-id="56a13-163">String</span><span class="sxs-lookup"><span data-stu-id="56a13-163">String</span></span>|<span data-ttu-id="56a13-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="56a13-164">The privacy statement Url.</span></span> <span data-ttu-id="56a13-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56a13-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="56a13-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="56a13-166">informationUrl</span></span>|<span data-ttu-id="56a13-167">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="56a13-167">String</span></span>|<span data-ttu-id="56a13-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="56a13-168">The more information Url.</span></span> <span data-ttu-id="56a13-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56a13-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="56a13-170">owner</span><span class="sxs-lookup"><span data-stu-id="56a13-170">owner</span></span>|<span data-ttu-id="56a13-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="56a13-171">String</span></span>|<span data-ttu-id="56a13-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="56a13-172">The owner of the app.</span></span> <span data-ttu-id="56a13-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56a13-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="56a13-174">developer</span><span class="sxs-lookup"><span data-stu-id="56a13-174">developer</span></span>|<span data-ttu-id="56a13-175">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="56a13-175">String</span></span>|<span data-ttu-id="56a13-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="56a13-176">The developer of the app.</span></span> <span data-ttu-id="56a13-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56a13-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="56a13-178">notes</span><span class="sxs-lookup"><span data-stu-id="56a13-178">notes</span></span>|<span data-ttu-id="56a13-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="56a13-179">String</span></span>|<span data-ttu-id="56a13-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="56a13-180">Notes for the app.</span></span> <span data-ttu-id="56a13-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56a13-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="56a13-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="56a13-182">publishingState</span></span>|[<span data-ttu-id="56a13-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="56a13-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="56a13-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="56a13-184">The publishing state for the app.</span></span> <span data-ttu-id="56a13-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="56a13-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="56a13-186">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="56a13-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="56a13-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="56a13-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="56a13-188">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="56a13-188">usedLicenseCount</span></span>|<span data-ttu-id="56a13-189">Int32</span><span class="sxs-lookup"><span data-stu-id="56a13-189">Int32</span></span>|<span data-ttu-id="56a13-190">Die Anzahl von verwendeten Microsoft Store für Unternehmen-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="56a13-190">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="56a13-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="56a13-191">totalLicenseCount</span></span>|<span data-ttu-id="56a13-192">Int32</span><span class="sxs-lookup"><span data-stu-id="56a13-192">Int32</span></span>|<span data-ttu-id="56a13-193">Die Gesamtzahl der Microsoft Store für Unternehmen-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="56a13-193">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="56a13-194">productKey</span><span class="sxs-lookup"><span data-stu-id="56a13-194">productKey</span></span>|<span data-ttu-id="56a13-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="56a13-195">String</span></span>|<span data-ttu-id="56a13-196">Der Product Key der App</span><span class="sxs-lookup"><span data-stu-id="56a13-196">The app product key</span></span>|
|<span data-ttu-id="56a13-197">licenseType</span><span class="sxs-lookup"><span data-stu-id="56a13-197">licenseType</span></span>|[<span data-ttu-id="56a13-198">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="56a13-198">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="56a13-199">Der APP-Lizenztyp.</span><span class="sxs-lookup"><span data-stu-id="56a13-199">The app license type.</span></span> <span data-ttu-id="56a13-200">Mögliche Werte sind: `offline` und `online`.</span><span class="sxs-lookup"><span data-stu-id="56a13-200">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="56a13-201">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="56a13-201">packageIdentityName</span></span>|<span data-ttu-id="56a13-202">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="56a13-202">String</span></span>|<span data-ttu-id="56a13-203">Bezeichner des App-Pakets</span><span class="sxs-lookup"><span data-stu-id="56a13-203">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="56a13-204">Antwort</span><span class="sxs-lookup"><span data-stu-id="56a13-204">Response</span></span>
<span data-ttu-id="56a13-205">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="56a13-205">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56a13-206">Beispiel</span><span class="sxs-lookup"><span data-stu-id="56a13-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="56a13-207">Anforderung</span><span class="sxs-lookup"><span data-stu-id="56a13-207">Request</span></span>
<span data-ttu-id="56a13-208">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="56a13-208">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="56a13-209">Antwort</span><span class="sxs-lookup"><span data-stu-id="56a13-209">Response</span></span>
<span data-ttu-id="56a13-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="56a13-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



