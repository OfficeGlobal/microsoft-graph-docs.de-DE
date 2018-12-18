---
title: webApp erstellen
description: Erstellen eines neuen webApp-Objekts.
author: tfitzmac
ms.openlocfilehash: 0ebe226b42fb0a35658a08107c9826a7401825db
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330926"
---
# <a name="create-webapp"></a><span data-ttu-id="413af-103">webApp erstellen</span><span class="sxs-lookup"><span data-stu-id="413af-103">Create webApp</span></span>

> <span data-ttu-id="413af-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="413af-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="413af-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="413af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="413af-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="413af-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="413af-107">Erstellen eines neuen [webApp](../resources/intune-apps-webapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="413af-107">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="413af-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="413af-108">Prerequisites</span></span>
<span data-ttu-id="413af-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="413af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="413af-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="413af-111">Permission type</span></span>|<span data-ttu-id="413af-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="413af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="413af-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="413af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="413af-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="413af-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="413af-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="413af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="413af-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="413af-116">Not supported.</span></span>|
|<span data-ttu-id="413af-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="413af-117">Application</span></span>|<span data-ttu-id="413af-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="413af-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="413af-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="413af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="413af-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="413af-120">Request headers</span></span>
|<span data-ttu-id="413af-121">Header</span><span class="sxs-lookup"><span data-stu-id="413af-121">Header</span></span>|<span data-ttu-id="413af-122">Wert</span><span class="sxs-lookup"><span data-stu-id="413af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="413af-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="413af-123">Authorization</span></span>|<span data-ttu-id="413af-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="413af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="413af-125">Accept</span><span class="sxs-lookup"><span data-stu-id="413af-125">Accept</span></span>|<span data-ttu-id="413af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="413af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="413af-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="413af-127">Request body</span></span>
<span data-ttu-id="413af-128">Geben Sie im Anforderungstext eine JSON-Darstellung des webApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="413af-128">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="413af-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der webApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="413af-129">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="413af-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="413af-130">Property</span></span>|<span data-ttu-id="413af-131">Typ</span><span class="sxs-lookup"><span data-stu-id="413af-131">Type</span></span>|<span data-ttu-id="413af-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="413af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="413af-133">id</span><span class="sxs-lookup"><span data-stu-id="413af-133">id</span></span>|<span data-ttu-id="413af-134">String</span><span class="sxs-lookup"><span data-stu-id="413af-134">String</span></span>|<span data-ttu-id="413af-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="413af-135">Key of the entity.</span></span> <span data-ttu-id="413af-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="413af-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="413af-137">displayName</span><span class="sxs-lookup"><span data-stu-id="413af-137">displayName</span></span>|<span data-ttu-id="413af-138">String</span><span class="sxs-lookup"><span data-stu-id="413af-138">String</span></span>|<span data-ttu-id="413af-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="413af-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="413af-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="413af-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="413af-141">description</span><span class="sxs-lookup"><span data-stu-id="413af-141">description</span></span>|<span data-ttu-id="413af-142">String</span><span class="sxs-lookup"><span data-stu-id="413af-142">String</span></span>|<span data-ttu-id="413af-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="413af-143">The description of the app.</span></span> <span data-ttu-id="413af-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="413af-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="413af-145">publisher</span><span class="sxs-lookup"><span data-stu-id="413af-145">publisher</span></span>|<span data-ttu-id="413af-146">String</span><span class="sxs-lookup"><span data-stu-id="413af-146">String</span></span>|<span data-ttu-id="413af-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="413af-147">The publisher of the app.</span></span> <span data-ttu-id="413af-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="413af-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="413af-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="413af-149">largeIcon</span></span>|[<span data-ttu-id="413af-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="413af-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="413af-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="413af-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="413af-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="413af-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="413af-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="413af-153">createdDateTime</span></span>|<span data-ttu-id="413af-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="413af-154">DateTimeOffset</span></span>|<span data-ttu-id="413af-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="413af-155">The date and time the app was created.</span></span> <span data-ttu-id="413af-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="413af-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="413af-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="413af-157">lastModifiedDateTime</span></span>|<span data-ttu-id="413af-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="413af-158">DateTimeOffset</span></span>|<span data-ttu-id="413af-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="413af-159">The date and time the app was last modified.</span></span> <span data-ttu-id="413af-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="413af-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="413af-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="413af-161">isFeatured</span></span>|<span data-ttu-id="413af-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="413af-162">Boolean</span></span>|<span data-ttu-id="413af-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="413af-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="413af-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="413af-164">privacyInformationUrl</span></span>|<span data-ttu-id="413af-165">String</span><span class="sxs-lookup"><span data-stu-id="413af-165">String</span></span>|<span data-ttu-id="413af-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="413af-166">The privacy statement Url.</span></span> <span data-ttu-id="413af-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="413af-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="413af-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="413af-168">informationUrl</span></span>|<span data-ttu-id="413af-169">String</span><span class="sxs-lookup"><span data-stu-id="413af-169">String</span></span>|<span data-ttu-id="413af-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="413af-170">The more information Url.</span></span> <span data-ttu-id="413af-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="413af-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="413af-172">owner</span><span class="sxs-lookup"><span data-stu-id="413af-172">owner</span></span>|<span data-ttu-id="413af-173">String</span><span class="sxs-lookup"><span data-stu-id="413af-173">String</span></span>|<span data-ttu-id="413af-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="413af-174">The owner of the app.</span></span> <span data-ttu-id="413af-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="413af-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="413af-176">developer</span><span class="sxs-lookup"><span data-stu-id="413af-176">developer</span></span>|<span data-ttu-id="413af-177">String</span><span class="sxs-lookup"><span data-stu-id="413af-177">String</span></span>|<span data-ttu-id="413af-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="413af-178">The developer of the app.</span></span> <span data-ttu-id="413af-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="413af-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="413af-180">notes</span><span class="sxs-lookup"><span data-stu-id="413af-180">notes</span></span>|<span data-ttu-id="413af-181">String</span><span class="sxs-lookup"><span data-stu-id="413af-181">String</span></span>|<span data-ttu-id="413af-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="413af-182">Notes for the app.</span></span> <span data-ttu-id="413af-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="413af-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="413af-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="413af-184">uploadState</span></span>|<span data-ttu-id="413af-185">Int32</span><span class="sxs-lookup"><span data-stu-id="413af-185">Int32</span></span>|<span data-ttu-id="413af-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="413af-186">The upload state.</span></span> <span data-ttu-id="413af-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="413af-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="413af-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="413af-188">publishingState</span></span>|[<span data-ttu-id="413af-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="413af-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="413af-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="413af-190">The publishing state for the app.</span></span> <span data-ttu-id="413af-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="413af-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="413af-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="413af-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="413af-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="413af-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="413af-194">appUrl</span><span class="sxs-lookup"><span data-stu-id="413af-194">appUrl</span></span>|<span data-ttu-id="413af-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="413af-195">String</span></span>|<span data-ttu-id="413af-196">Die URL der Web-App.</span><span class="sxs-lookup"><span data-stu-id="413af-196">The web app URL.</span></span>|
|<span data-ttu-id="413af-197">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="413af-197">useManagedBrowser</span></span>|<span data-ttu-id="413af-198">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="413af-198">Boolean</span></span>|<span data-ttu-id="413af-199">Gibt an, ob ein verwalteter Browser verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="413af-199">Whether or not to use managed browser.</span></span> <span data-ttu-id="413af-200">Diese Eigenschaft ist nur für Android und IOS möglich.</span><span class="sxs-lookup"><span data-stu-id="413af-200">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="413af-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="413af-201">Response</span></span>
<span data-ttu-id="413af-202">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [webApp](../resources/intune-apps-webapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="413af-202">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="413af-203">Beispiel</span><span class="sxs-lookup"><span data-stu-id="413af-203">Example</span></span>
### <a name="request"></a><span data-ttu-id="413af-204">Anforderung</span><span class="sxs-lookup"><span data-stu-id="413af-204">Request</span></span>
<span data-ttu-id="413af-205">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="413af-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 731

{
  "@odata.type": "#microsoft.graph.webApp",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="413af-206">Antwort</span><span class="sxs-lookup"><span data-stu-id="413af-206">Response</span></span>
<span data-ttu-id="413af-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="413af-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 839

{
  "@odata.type": "#microsoft.graph.webApp",
  "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```





