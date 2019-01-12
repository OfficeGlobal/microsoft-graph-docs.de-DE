---
title: Erstellen von windowsStoreApp
description: Erstellen eines neuen WindowsStoreApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2ba7809c47cc90054829d5f6ef8ded3f3f58050b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945069"
---
# <a name="create-windowsstoreapp"></a><span data-ttu-id="9ed8e-103">Erstellen von windowsStoreApp</span><span class="sxs-lookup"><span data-stu-id="9ed8e-103">Create windowsStoreApp</span></span>

> <span data-ttu-id="9ed8e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ed8e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ed8e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ed8e-107">Erstellen eines neuen [WindowsStoreApp](../resources/intune-apps-windowsstoreapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-107">Create a new [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9ed8e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9ed8e-108">Prerequisites</span></span>
<span data-ttu-id="9ed8e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ed8e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ed8e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9ed8e-111">Permission type</span></span>|<span data-ttu-id="9ed8e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9ed8e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ed8e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9ed8e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ed8e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ed8e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9ed8e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9ed8e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ed8e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ed8e-116">Not supported.</span></span>|
|<span data-ttu-id="9ed8e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9ed8e-117">Application</span></span>|<span data-ttu-id="9ed8e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ed8e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ed8e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ed8e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="9ed8e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9ed8e-120">Request headers</span></span>
|<span data-ttu-id="9ed8e-121">Header</span><span class="sxs-lookup"><span data-stu-id="9ed8e-121">Header</span></span>|<span data-ttu-id="9ed8e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9ed8e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ed8e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ed8e-123">Authorization</span></span>|<span data-ttu-id="9ed8e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9ed8e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ed8e-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9ed8e-125">Accept</span></span>|<span data-ttu-id="9ed8e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ed8e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ed8e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9ed8e-127">Request body</span></span>
<span data-ttu-id="9ed8e-128">Geben Sie im Textkörper Anforderung für das Objekt WindowsStoreApp eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-128">In the request body, supply a JSON representation for the windowsStoreApp object.</span></span>

<span data-ttu-id="9ed8e-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die WindowsStoreApp erstellen.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-129">The following table shows the properties that are required when you create the windowsStoreApp.</span></span>

|<span data-ttu-id="9ed8e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9ed8e-130">Property</span></span>|<span data-ttu-id="9ed8e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="9ed8e-131">Type</span></span>|<span data-ttu-id="9ed8e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ed8e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ed8e-133">id</span><span class="sxs-lookup"><span data-stu-id="9ed8e-133">id</span></span>|<span data-ttu-id="9ed8e-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ed8e-134">String</span></span>|<span data-ttu-id="9ed8e-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9ed8e-135">Key of the entity.</span></span> <span data-ttu-id="9ed8e-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ed8e-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ed8e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9ed8e-137">displayName</span></span>|<span data-ttu-id="9ed8e-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ed8e-138">String</span></span>|<span data-ttu-id="9ed8e-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9ed8e-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ed8e-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ed8e-141">description</span><span class="sxs-lookup"><span data-stu-id="9ed8e-141">description</span></span>|<span data-ttu-id="9ed8e-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ed8e-142">String</span></span>|<span data-ttu-id="9ed8e-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-143">The description of the app.</span></span> <span data-ttu-id="9ed8e-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ed8e-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ed8e-145">publisher</span><span class="sxs-lookup"><span data-stu-id="9ed8e-145">publisher</span></span>|<span data-ttu-id="9ed8e-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ed8e-146">String</span></span>|<span data-ttu-id="9ed8e-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-147">The publisher of the app.</span></span> <span data-ttu-id="9ed8e-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ed8e-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ed8e-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9ed8e-149">largeIcon</span></span>|[<span data-ttu-id="9ed8e-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9ed8e-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9ed8e-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9ed8e-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ed8e-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ed8e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ed8e-153">createdDateTime</span></span>|<span data-ttu-id="9ed8e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ed8e-154">DateTimeOffset</span></span>|<span data-ttu-id="9ed8e-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-155">The date and time the app was created.</span></span> <span data-ttu-id="9ed8e-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ed8e-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ed8e-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ed8e-157">lastModifiedDateTime</span></span>|<span data-ttu-id="9ed8e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ed8e-158">DateTimeOffset</span></span>|<span data-ttu-id="9ed8e-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-159">The date and time the app was last modified.</span></span> <span data-ttu-id="9ed8e-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ed8e-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ed8e-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9ed8e-161">isFeatured</span></span>|<span data-ttu-id="9ed8e-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9ed8e-162">Boolean</span></span>|<span data-ttu-id="9ed8e-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ed8e-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ed8e-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9ed8e-164">privacyInformationUrl</span></span>|<span data-ttu-id="9ed8e-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ed8e-165">String</span></span>|<span data-ttu-id="9ed8e-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-166">The privacy statement Url.</span></span> <span data-ttu-id="9ed8e-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ed8e-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ed8e-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9ed8e-168">informationUrl</span></span>|<span data-ttu-id="9ed8e-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ed8e-169">String</span></span>|<span data-ttu-id="9ed8e-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-170">The more information Url.</span></span> <span data-ttu-id="9ed8e-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ed8e-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ed8e-172">owner</span><span class="sxs-lookup"><span data-stu-id="9ed8e-172">owner</span></span>|<span data-ttu-id="9ed8e-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ed8e-173">String</span></span>|<span data-ttu-id="9ed8e-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-174">The owner of the app.</span></span> <span data-ttu-id="9ed8e-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ed8e-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ed8e-176">developer</span><span class="sxs-lookup"><span data-stu-id="9ed8e-176">developer</span></span>|<span data-ttu-id="9ed8e-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ed8e-177">String</span></span>|<span data-ttu-id="9ed8e-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-178">The developer of the app.</span></span> <span data-ttu-id="9ed8e-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ed8e-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ed8e-180">notes</span><span class="sxs-lookup"><span data-stu-id="9ed8e-180">notes</span></span>|<span data-ttu-id="9ed8e-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ed8e-181">String</span></span>|<span data-ttu-id="9ed8e-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-182">Notes for the app.</span></span> <span data-ttu-id="9ed8e-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ed8e-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ed8e-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="9ed8e-184">uploadState</span></span>|<span data-ttu-id="9ed8e-185">Int32</span><span class="sxs-lookup"><span data-stu-id="9ed8e-185">Int32</span></span>|<span data-ttu-id="9ed8e-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-186">The upload state.</span></span> <span data-ttu-id="9ed8e-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ed8e-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9ed8e-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="9ed8e-188">publishingState</span></span>|[<span data-ttu-id="9ed8e-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9ed8e-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9ed8e-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-190">The publishing state for the app.</span></span> <span data-ttu-id="9ed8e-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9ed8e-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ed8e-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="9ed8e-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9ed8e-194">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="9ed8e-194">appStoreUrl</span></span>|<span data-ttu-id="9ed8e-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9ed8e-195">String</span></span>|<span data-ttu-id="9ed8e-196">Die URL der Windows-app-Store.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-196">The Windows app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="9ed8e-197">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ed8e-197">Response</span></span>
<span data-ttu-id="9ed8e-198">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [WindowsStoreApp](../resources/intune-apps-windowsstoreapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-198">If successful, this method returns a `201 Created` response code and a [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ed8e-199">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9ed8e-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="9ed8e-200">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ed8e-200">Request</span></span>
<span data-ttu-id="9ed8e-201">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9ed8e-202">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ed8e-202">Response</span></span>
<span data-ttu-id="9ed8e-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ed8e-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





