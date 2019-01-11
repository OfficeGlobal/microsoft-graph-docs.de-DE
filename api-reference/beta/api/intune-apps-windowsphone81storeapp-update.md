---
title: WindowsPhone81StoreApp aktualisieren
description: Aktualisieren Sie die Eigenschaften eines windowsPhone81StoreApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d1ba9c814d29d57c0bcb8024dc70b537c4a92b57
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875418"
---
# <a name="update-windowsphone81storeapp"></a><span data-ttu-id="96ab4-103">WindowsPhone81StoreApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="96ab4-103">Update windowsPhone81StoreApp</span></span>

> <span data-ttu-id="96ab4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="96ab4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96ab4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="96ab4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="96ab4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="96ab4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96ab4-107">Aktualisieren Sie die Eigenschaften eines [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="96ab4-107">Update the properties of a [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="96ab4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="96ab4-108">Prerequisites</span></span>
<span data-ttu-id="96ab4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96ab4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96ab4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="96ab4-111">Permission type</span></span>|<span data-ttu-id="96ab4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="96ab4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96ab4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="96ab4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="96ab4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96ab4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="96ab4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="96ab4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96ab4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="96ab4-116">Not supported.</span></span>|
|<span data-ttu-id="96ab4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="96ab4-117">Application</span></span>|<span data-ttu-id="96ab4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="96ab4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96ab4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="96ab4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="96ab4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="96ab4-120">Request headers</span></span>
|<span data-ttu-id="96ab4-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="96ab4-121">Header</span></span>|<span data-ttu-id="96ab4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="96ab4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96ab4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="96ab4-123">Authorization</span></span>|<span data-ttu-id="96ab4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="96ab4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96ab4-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="96ab4-125">Accept</span></span>|<span data-ttu-id="96ab4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96ab4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96ab4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="96ab4-127">Request body</span></span>
<span data-ttu-id="96ab4-128">Geben Sie im Textkörper Anforderung für das Objekt [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="96ab4-128">In the request body, supply a JSON representation for the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

<span data-ttu-id="96ab4-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="96ab4-129">The following table shows the properties that are required when you create the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md).</span></span>

|<span data-ttu-id="96ab4-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="96ab4-130">Property</span></span>|<span data-ttu-id="96ab4-131">Typ</span><span class="sxs-lookup"><span data-stu-id="96ab4-131">Type</span></span>|<span data-ttu-id="96ab4-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96ab4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96ab4-133">id</span><span class="sxs-lookup"><span data-stu-id="96ab4-133">id</span></span>|<span data-ttu-id="96ab4-134">String</span><span class="sxs-lookup"><span data-stu-id="96ab4-134">String</span></span>|<span data-ttu-id="96ab4-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="96ab4-135">Key of the entity.</span></span> <span data-ttu-id="96ab4-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96ab4-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96ab4-137">displayName</span><span class="sxs-lookup"><span data-stu-id="96ab4-137">displayName</span></span>|<span data-ttu-id="96ab4-138">String</span><span class="sxs-lookup"><span data-stu-id="96ab4-138">String</span></span>|<span data-ttu-id="96ab4-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="96ab4-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="96ab4-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96ab4-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96ab4-141">description</span><span class="sxs-lookup"><span data-stu-id="96ab4-141">description</span></span>|<span data-ttu-id="96ab4-142">String</span><span class="sxs-lookup"><span data-stu-id="96ab4-142">String</span></span>|<span data-ttu-id="96ab4-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="96ab4-143">The description of the app.</span></span> <span data-ttu-id="96ab4-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96ab4-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96ab4-145">publisher</span><span class="sxs-lookup"><span data-stu-id="96ab4-145">publisher</span></span>|<span data-ttu-id="96ab4-146">String</span><span class="sxs-lookup"><span data-stu-id="96ab4-146">String</span></span>|<span data-ttu-id="96ab4-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="96ab4-147">The publisher of the app.</span></span> <span data-ttu-id="96ab4-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96ab4-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96ab4-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="96ab4-149">largeIcon</span></span>|[<span data-ttu-id="96ab4-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="96ab4-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="96ab4-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="96ab4-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="96ab4-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96ab4-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96ab4-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="96ab4-153">createdDateTime</span></span>|<span data-ttu-id="96ab4-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96ab4-154">DateTimeOffset</span></span>|<span data-ttu-id="96ab4-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="96ab4-155">The date and time the app was created.</span></span> <span data-ttu-id="96ab4-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96ab4-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96ab4-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96ab4-157">lastModifiedDateTime</span></span>|<span data-ttu-id="96ab4-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96ab4-158">DateTimeOffset</span></span>|<span data-ttu-id="96ab4-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="96ab4-159">The date and time the app was last modified.</span></span> <span data-ttu-id="96ab4-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96ab4-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96ab4-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="96ab4-161">isFeatured</span></span>|<span data-ttu-id="96ab4-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="96ab4-162">Boolean</span></span>|<span data-ttu-id="96ab4-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96ab4-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96ab4-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="96ab4-164">privacyInformationUrl</span></span>|<span data-ttu-id="96ab4-165">String</span><span class="sxs-lookup"><span data-stu-id="96ab4-165">String</span></span>|<span data-ttu-id="96ab4-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="96ab4-166">The privacy statement Url.</span></span> <span data-ttu-id="96ab4-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96ab4-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96ab4-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="96ab4-168">informationUrl</span></span>|<span data-ttu-id="96ab4-169">String</span><span class="sxs-lookup"><span data-stu-id="96ab4-169">String</span></span>|<span data-ttu-id="96ab4-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="96ab4-170">The more information Url.</span></span> <span data-ttu-id="96ab4-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96ab4-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96ab4-172">owner</span><span class="sxs-lookup"><span data-stu-id="96ab4-172">owner</span></span>|<span data-ttu-id="96ab4-173">String</span><span class="sxs-lookup"><span data-stu-id="96ab4-173">String</span></span>|<span data-ttu-id="96ab4-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="96ab4-174">The owner of the app.</span></span> <span data-ttu-id="96ab4-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96ab4-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96ab4-176">developer</span><span class="sxs-lookup"><span data-stu-id="96ab4-176">developer</span></span>|<span data-ttu-id="96ab4-177">String</span><span class="sxs-lookup"><span data-stu-id="96ab4-177">String</span></span>|<span data-ttu-id="96ab4-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="96ab4-178">The developer of the app.</span></span> <span data-ttu-id="96ab4-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96ab4-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96ab4-180">notes</span><span class="sxs-lookup"><span data-stu-id="96ab4-180">notes</span></span>|<span data-ttu-id="96ab4-181">String</span><span class="sxs-lookup"><span data-stu-id="96ab4-181">String</span></span>|<span data-ttu-id="96ab4-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="96ab4-182">Notes for the app.</span></span> <span data-ttu-id="96ab4-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96ab4-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96ab4-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="96ab4-184">uploadState</span></span>|<span data-ttu-id="96ab4-185">Int32</span><span class="sxs-lookup"><span data-stu-id="96ab4-185">Int32</span></span>|<span data-ttu-id="96ab4-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="96ab4-186">The upload state.</span></span> <span data-ttu-id="96ab4-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96ab4-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96ab4-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="96ab4-188">publishingState</span></span>|[<span data-ttu-id="96ab4-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="96ab4-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="96ab4-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="96ab4-190">The publishing state for the app.</span></span> <span data-ttu-id="96ab4-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="96ab4-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="96ab4-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96ab4-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="96ab4-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="96ab4-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="96ab4-194">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="96ab4-194">appStoreUrl</span></span>|<span data-ttu-id="96ab4-195">String</span><span class="sxs-lookup"><span data-stu-id="96ab4-195">String</span></span>|<span data-ttu-id="96ab4-196">Die URL der 8.1 für Windows Phone-app-Store.</span><span class="sxs-lookup"><span data-stu-id="96ab4-196">The Windows Phone 8.1 app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="96ab4-197">Antwort</span><span class="sxs-lookup"><span data-stu-id="96ab4-197">Response</span></span>
<span data-ttu-id="96ab4-198">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="96ab4-198">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96ab4-199">Beispiel</span><span class="sxs-lookup"><span data-stu-id="96ab4-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="96ab4-200">Anforderung</span><span class="sxs-lookup"><span data-stu-id="96ab4-200">Request</span></span>
<span data-ttu-id="96ab4-201">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="96ab4-201">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 666

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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="96ab4-202">Antwort</span><span class="sxs-lookup"><span data-stu-id="96ab4-202">Response</span></span>
<span data-ttu-id="96ab4-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="96ab4-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 835

{
  "@odata.type": "#microsoft.graph.windowsPhone81StoreApp",
  "id": "f68ce6a1-e6a1-f68c-a1e6-8cf6a1e68cf6",
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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```





