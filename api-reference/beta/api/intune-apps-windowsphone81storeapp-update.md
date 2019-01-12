---
title: WindowsPhone81StoreApp aktualisieren
description: Aktualisieren Sie die Eigenschaften eines windowsPhone81StoreApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e7988ec329f19c13804b81650be03890e91802db
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956367"
---
# <a name="update-windowsphone81storeapp"></a><span data-ttu-id="4379d-103">WindowsPhone81StoreApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4379d-103">Update windowsPhone81StoreApp</span></span>

> <span data-ttu-id="4379d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4379d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4379d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4379d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4379d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4379d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4379d-107">Aktualisieren Sie die Eigenschaften eines [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4379d-107">Update the properties of a [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4379d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4379d-108">Prerequisites</span></span>
<span data-ttu-id="4379d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4379d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4379d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4379d-111">Permission type</span></span>|<span data-ttu-id="4379d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4379d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4379d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4379d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4379d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4379d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4379d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4379d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4379d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4379d-116">Not supported.</span></span>|
|<span data-ttu-id="4379d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4379d-117">Application</span></span>|<span data-ttu-id="4379d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4379d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4379d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4379d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="4379d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4379d-120">Request headers</span></span>
|<span data-ttu-id="4379d-121">Header</span><span class="sxs-lookup"><span data-stu-id="4379d-121">Header</span></span>|<span data-ttu-id="4379d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4379d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4379d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4379d-123">Authorization</span></span>|<span data-ttu-id="4379d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4379d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4379d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4379d-125">Accept</span></span>|<span data-ttu-id="4379d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4379d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4379d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4379d-127">Request body</span></span>
<span data-ttu-id="4379d-128">Geben Sie im Textkörper Anforderung für das Objekt [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="4379d-128">In the request body, supply a JSON representation for the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

<span data-ttu-id="4379d-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="4379d-129">The following table shows the properties that are required when you create the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md).</span></span>

|<span data-ttu-id="4379d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4379d-130">Property</span></span>|<span data-ttu-id="4379d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4379d-131">Type</span></span>|<span data-ttu-id="4379d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4379d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4379d-133">id</span><span class="sxs-lookup"><span data-stu-id="4379d-133">id</span></span>|<span data-ttu-id="4379d-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4379d-134">String</span></span>|<span data-ttu-id="4379d-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4379d-135">Key of the entity.</span></span> <span data-ttu-id="4379d-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4379d-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4379d-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4379d-137">displayName</span></span>|<span data-ttu-id="4379d-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4379d-138">String</span></span>|<span data-ttu-id="4379d-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="4379d-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4379d-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4379d-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4379d-141">description</span><span class="sxs-lookup"><span data-stu-id="4379d-141">description</span></span>|<span data-ttu-id="4379d-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4379d-142">String</span></span>|<span data-ttu-id="4379d-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="4379d-143">The description of the app.</span></span> <span data-ttu-id="4379d-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4379d-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4379d-145">publisher</span><span class="sxs-lookup"><span data-stu-id="4379d-145">publisher</span></span>|<span data-ttu-id="4379d-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4379d-146">String</span></span>|<span data-ttu-id="4379d-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="4379d-147">The publisher of the app.</span></span> <span data-ttu-id="4379d-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4379d-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4379d-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4379d-149">largeIcon</span></span>|[<span data-ttu-id="4379d-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4379d-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4379d-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="4379d-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4379d-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4379d-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4379d-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4379d-153">createdDateTime</span></span>|<span data-ttu-id="4379d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4379d-154">DateTimeOffset</span></span>|<span data-ttu-id="4379d-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="4379d-155">The date and time the app was created.</span></span> <span data-ttu-id="4379d-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4379d-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4379d-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4379d-157">lastModifiedDateTime</span></span>|<span data-ttu-id="4379d-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4379d-158">DateTimeOffset</span></span>|<span data-ttu-id="4379d-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="4379d-159">The date and time the app was last modified.</span></span> <span data-ttu-id="4379d-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4379d-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4379d-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4379d-161">isFeatured</span></span>|<span data-ttu-id="4379d-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4379d-162">Boolean</span></span>|<span data-ttu-id="4379d-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4379d-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4379d-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4379d-164">privacyInformationUrl</span></span>|<span data-ttu-id="4379d-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4379d-165">String</span></span>|<span data-ttu-id="4379d-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="4379d-166">The privacy statement Url.</span></span> <span data-ttu-id="4379d-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4379d-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4379d-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4379d-168">informationUrl</span></span>|<span data-ttu-id="4379d-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4379d-169">String</span></span>|<span data-ttu-id="4379d-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="4379d-170">The more information Url.</span></span> <span data-ttu-id="4379d-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4379d-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4379d-172">owner</span><span class="sxs-lookup"><span data-stu-id="4379d-172">owner</span></span>|<span data-ttu-id="4379d-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4379d-173">String</span></span>|<span data-ttu-id="4379d-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="4379d-174">The owner of the app.</span></span> <span data-ttu-id="4379d-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4379d-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4379d-176">developer</span><span class="sxs-lookup"><span data-stu-id="4379d-176">developer</span></span>|<span data-ttu-id="4379d-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4379d-177">String</span></span>|<span data-ttu-id="4379d-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="4379d-178">The developer of the app.</span></span> <span data-ttu-id="4379d-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4379d-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4379d-180">notes</span><span class="sxs-lookup"><span data-stu-id="4379d-180">notes</span></span>|<span data-ttu-id="4379d-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4379d-181">String</span></span>|<span data-ttu-id="4379d-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="4379d-182">Notes for the app.</span></span> <span data-ttu-id="4379d-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4379d-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4379d-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="4379d-184">uploadState</span></span>|<span data-ttu-id="4379d-185">Int32</span><span class="sxs-lookup"><span data-stu-id="4379d-185">Int32</span></span>|<span data-ttu-id="4379d-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="4379d-186">The upload state.</span></span> <span data-ttu-id="4379d-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4379d-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4379d-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="4379d-188">publishingState</span></span>|[<span data-ttu-id="4379d-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4379d-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4379d-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="4379d-190">The publishing state for the app.</span></span> <span data-ttu-id="4379d-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="4379d-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4379d-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4379d-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="4379d-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="4379d-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4379d-194">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="4379d-194">appStoreUrl</span></span>|<span data-ttu-id="4379d-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4379d-195">String</span></span>|<span data-ttu-id="4379d-196">Die URL der 8.1 für Windows Phone-app-Store.</span><span class="sxs-lookup"><span data-stu-id="4379d-196">The Windows Phone 8.1 app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="4379d-197">Antwort</span><span class="sxs-lookup"><span data-stu-id="4379d-197">Response</span></span>
<span data-ttu-id="4379d-198">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4379d-198">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4379d-199">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4379d-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="4379d-200">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4379d-200">Request</span></span>
<span data-ttu-id="4379d-201">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4379d-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4379d-202">Antwort</span><span class="sxs-lookup"><span data-stu-id="4379d-202">Response</span></span>
<span data-ttu-id="4379d-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4379d-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





