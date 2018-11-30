---
title: Erstellen von windowsStoreApp
description: Erstellen eines neuen WindowsStoreApp-Objekts.
ms.openlocfilehash: 97b791e89752cc059f1adf77691b0a50edee4dc4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063425"
---
# <a name="create-windowsstoreapp"></a><span data-ttu-id="29afd-103">Erstellen von windowsStoreApp</span><span class="sxs-lookup"><span data-stu-id="29afd-103">Create windowsStoreApp</span></span>

> <span data-ttu-id="29afd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="29afd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29afd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="29afd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29afd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="29afd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29afd-107">Erstellen eines neuen [WindowsStoreApp](../resources/intune-apps-windowsstoreapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="29afd-107">Create a new [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="29afd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="29afd-108">Prerequisites</span></span>
<span data-ttu-id="29afd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29afd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29afd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="29afd-111">Permission type</span></span>|<span data-ttu-id="29afd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="29afd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29afd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="29afd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29afd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29afd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="29afd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="29afd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29afd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="29afd-116">Not supported.</span></span>|
|<span data-ttu-id="29afd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="29afd-117">Application</span></span>|<span data-ttu-id="29afd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="29afd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29afd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="29afd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="29afd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="29afd-120">Request headers</span></span>
|<span data-ttu-id="29afd-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="29afd-121">Header</span></span>|<span data-ttu-id="29afd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="29afd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29afd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="29afd-123">Authorization</span></span>|<span data-ttu-id="29afd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="29afd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29afd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="29afd-125">Accept</span></span>|<span data-ttu-id="29afd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="29afd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29afd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="29afd-127">Request body</span></span>
<span data-ttu-id="29afd-128">Geben Sie im Textkörper Anforderung für das Objekt WindowsStoreApp eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="29afd-128">In the request body, supply a JSON representation for the windowsStoreApp object.</span></span>

<span data-ttu-id="29afd-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die WindowsStoreApp erstellen.</span><span class="sxs-lookup"><span data-stu-id="29afd-129">The following table shows the properties that are required when you create the windowsStoreApp.</span></span>

|<span data-ttu-id="29afd-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="29afd-130">Property</span></span>|<span data-ttu-id="29afd-131">Typ</span><span class="sxs-lookup"><span data-stu-id="29afd-131">Type</span></span>|<span data-ttu-id="29afd-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="29afd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29afd-133">id</span><span class="sxs-lookup"><span data-stu-id="29afd-133">id</span></span>|<span data-ttu-id="29afd-134">String</span><span class="sxs-lookup"><span data-stu-id="29afd-134">String</span></span>|<span data-ttu-id="29afd-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="29afd-135">Key of the entity.</span></span> <span data-ttu-id="29afd-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="29afd-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29afd-137">displayName</span><span class="sxs-lookup"><span data-stu-id="29afd-137">displayName</span></span>|<span data-ttu-id="29afd-138">String</span><span class="sxs-lookup"><span data-stu-id="29afd-138">String</span></span>|<span data-ttu-id="29afd-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="29afd-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="29afd-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="29afd-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29afd-141">description</span><span class="sxs-lookup"><span data-stu-id="29afd-141">description</span></span>|<span data-ttu-id="29afd-142">String</span><span class="sxs-lookup"><span data-stu-id="29afd-142">String</span></span>|<span data-ttu-id="29afd-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="29afd-143">The description of the app.</span></span> <span data-ttu-id="29afd-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="29afd-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29afd-145">publisher</span><span class="sxs-lookup"><span data-stu-id="29afd-145">publisher</span></span>|<span data-ttu-id="29afd-146">String</span><span class="sxs-lookup"><span data-stu-id="29afd-146">String</span></span>|<span data-ttu-id="29afd-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="29afd-147">The publisher of the app.</span></span> <span data-ttu-id="29afd-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="29afd-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29afd-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="29afd-149">largeIcon</span></span>|[<span data-ttu-id="29afd-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="29afd-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="29afd-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="29afd-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="29afd-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="29afd-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29afd-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29afd-153">createdDateTime</span></span>|<span data-ttu-id="29afd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29afd-154">DateTimeOffset</span></span>|<span data-ttu-id="29afd-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="29afd-155">The date and time the app was created.</span></span> <span data-ttu-id="29afd-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="29afd-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29afd-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29afd-157">lastModifiedDateTime</span></span>|<span data-ttu-id="29afd-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29afd-158">DateTimeOffset</span></span>|<span data-ttu-id="29afd-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="29afd-159">The date and time the app was last modified.</span></span> <span data-ttu-id="29afd-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="29afd-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29afd-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="29afd-161">isFeatured</span></span>|<span data-ttu-id="29afd-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="29afd-162">Boolean</span></span>|<span data-ttu-id="29afd-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="29afd-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29afd-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="29afd-164">privacyInformationUrl</span></span>|<span data-ttu-id="29afd-165">String</span><span class="sxs-lookup"><span data-stu-id="29afd-165">String</span></span>|<span data-ttu-id="29afd-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="29afd-166">The privacy statement Url.</span></span> <span data-ttu-id="29afd-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="29afd-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29afd-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="29afd-168">informationUrl</span></span>|<span data-ttu-id="29afd-169">String</span><span class="sxs-lookup"><span data-stu-id="29afd-169">String</span></span>|<span data-ttu-id="29afd-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="29afd-170">The more information Url.</span></span> <span data-ttu-id="29afd-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="29afd-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29afd-172">owner</span><span class="sxs-lookup"><span data-stu-id="29afd-172">owner</span></span>|<span data-ttu-id="29afd-173">String</span><span class="sxs-lookup"><span data-stu-id="29afd-173">String</span></span>|<span data-ttu-id="29afd-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="29afd-174">The owner of the app.</span></span> <span data-ttu-id="29afd-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="29afd-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29afd-176">developer</span><span class="sxs-lookup"><span data-stu-id="29afd-176">developer</span></span>|<span data-ttu-id="29afd-177">String</span><span class="sxs-lookup"><span data-stu-id="29afd-177">String</span></span>|<span data-ttu-id="29afd-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="29afd-178">The developer of the app.</span></span> <span data-ttu-id="29afd-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="29afd-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29afd-180">notes</span><span class="sxs-lookup"><span data-stu-id="29afd-180">notes</span></span>|<span data-ttu-id="29afd-181">String</span><span class="sxs-lookup"><span data-stu-id="29afd-181">String</span></span>|<span data-ttu-id="29afd-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="29afd-182">Notes for the app.</span></span> <span data-ttu-id="29afd-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="29afd-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29afd-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="29afd-184">uploadState</span></span>|<span data-ttu-id="29afd-185">Int32</span><span class="sxs-lookup"><span data-stu-id="29afd-185">Int32</span></span>|<span data-ttu-id="29afd-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="29afd-186">The upload state.</span></span> <span data-ttu-id="29afd-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="29afd-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29afd-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="29afd-188">publishingState</span></span>|[<span data-ttu-id="29afd-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="29afd-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="29afd-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="29afd-190">The publishing state for the app.</span></span> <span data-ttu-id="29afd-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="29afd-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="29afd-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="29afd-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="29afd-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="29afd-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="29afd-194">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="29afd-194">appStoreUrl</span></span>|<span data-ttu-id="29afd-195">String</span><span class="sxs-lookup"><span data-stu-id="29afd-195">String</span></span>|<span data-ttu-id="29afd-196">Die URL der Windows-app-Store.</span><span class="sxs-lookup"><span data-stu-id="29afd-196">The Windows app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="29afd-197">Antwort</span><span class="sxs-lookup"><span data-stu-id="29afd-197">Response</span></span>
<span data-ttu-id="29afd-198">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [WindowsStoreApp](../resources/intune-apps-windowsstoreapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="29afd-198">If successful, this method returns a `201 Created` response code and a [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29afd-199">Beispiel</span><span class="sxs-lookup"><span data-stu-id="29afd-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="29afd-200">Anforderung</span><span class="sxs-lookup"><span data-stu-id="29afd-200">Request</span></span>
<span data-ttu-id="29afd-201">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="29afd-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 720

{
  "@odata.type": "#microsoft.graph.windowsStoreApp",
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

### <a name="response"></a><span data-ttu-id="29afd-202">Antwort</span><span class="sxs-lookup"><span data-stu-id="29afd-202">Response</span></span>
<span data-ttu-id="29afd-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="29afd-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 828

{
  "@odata.type": "#microsoft.graph.windowsStoreApp",
  "id": "fd4a5f8a-5f8a-fd4a-8a5f-4afd8a5f4afd",
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





