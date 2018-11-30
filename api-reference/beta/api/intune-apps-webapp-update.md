---
title: webApp aktualisieren
description: Aktualisieren der Eigenschaften eines webApp-Objekts.
ms.openlocfilehash: cdd5269257a52e3aa4c378743771dfd482ac224e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064606"
---
# <a name="update-webapp"></a><span data-ttu-id="e76eb-103">webApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e76eb-103">Update webApp</span></span>

> <span data-ttu-id="e76eb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e76eb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e76eb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e76eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e76eb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e76eb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e76eb-107">Aktualisieren der Eigenschaften eines [webApp](../resources/intune-apps-webapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e76eb-107">Update the properties of a [webApp](../resources/intune-apps-webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e76eb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e76eb-108">Prerequisites</span></span>
<span data-ttu-id="e76eb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e76eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e76eb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e76eb-111">Permission type</span></span>|<span data-ttu-id="e76eb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e76eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e76eb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e76eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e76eb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e76eb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e76eb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e76eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e76eb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e76eb-116">Not supported.</span></span>|
|<span data-ttu-id="e76eb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e76eb-117">Application</span></span>|<span data-ttu-id="e76eb-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e76eb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e76eb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e76eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="e76eb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e76eb-120">Request headers</span></span>
|<span data-ttu-id="e76eb-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e76eb-121">Header</span></span>|<span data-ttu-id="e76eb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e76eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e76eb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e76eb-123">Authorization</span></span>|<span data-ttu-id="e76eb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e76eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e76eb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e76eb-125">Accept</span></span>|<span data-ttu-id="e76eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e76eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e76eb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e76eb-127">Request body</span></span>
<span data-ttu-id="e76eb-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [webApp](../resources/intune-apps-webapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e76eb-128">In the request body, supply a JSON representation for the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

<span data-ttu-id="e76eb-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [webApp](../resources/intune-apps-webapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e76eb-129">The following table shows the properties that are required when you create the [webApp](../resources/intune-apps-webapp.md).</span></span>

|<span data-ttu-id="e76eb-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e76eb-130">Property</span></span>|<span data-ttu-id="e76eb-131">Typ</span><span class="sxs-lookup"><span data-stu-id="e76eb-131">Type</span></span>|<span data-ttu-id="e76eb-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e76eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e76eb-133">id</span><span class="sxs-lookup"><span data-stu-id="e76eb-133">id</span></span>|<span data-ttu-id="e76eb-134">String</span><span class="sxs-lookup"><span data-stu-id="e76eb-134">String</span></span>|<span data-ttu-id="e76eb-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e76eb-135">Key of the entity.</span></span> <span data-ttu-id="e76eb-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e76eb-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e76eb-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e76eb-137">displayName</span></span>|<span data-ttu-id="e76eb-138">String</span><span class="sxs-lookup"><span data-stu-id="e76eb-138">String</span></span>|<span data-ttu-id="e76eb-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="e76eb-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e76eb-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e76eb-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e76eb-141">description</span><span class="sxs-lookup"><span data-stu-id="e76eb-141">description</span></span>|<span data-ttu-id="e76eb-142">String</span><span class="sxs-lookup"><span data-stu-id="e76eb-142">String</span></span>|<span data-ttu-id="e76eb-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="e76eb-143">The description of the app.</span></span> <span data-ttu-id="e76eb-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e76eb-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e76eb-145">publisher</span><span class="sxs-lookup"><span data-stu-id="e76eb-145">publisher</span></span>|<span data-ttu-id="e76eb-146">String</span><span class="sxs-lookup"><span data-stu-id="e76eb-146">String</span></span>|<span data-ttu-id="e76eb-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="e76eb-147">The publisher of the app.</span></span> <span data-ttu-id="e76eb-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e76eb-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e76eb-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e76eb-149">largeIcon</span></span>|[<span data-ttu-id="e76eb-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e76eb-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e76eb-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="e76eb-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e76eb-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e76eb-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e76eb-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e76eb-153">createdDateTime</span></span>|<span data-ttu-id="e76eb-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e76eb-154">DateTimeOffset</span></span>|<span data-ttu-id="e76eb-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="e76eb-155">The date and time the app was created.</span></span> <span data-ttu-id="e76eb-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e76eb-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e76eb-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e76eb-157">lastModifiedDateTime</span></span>|<span data-ttu-id="e76eb-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e76eb-158">DateTimeOffset</span></span>|<span data-ttu-id="e76eb-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="e76eb-159">The date and time the app was last modified.</span></span> <span data-ttu-id="e76eb-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e76eb-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e76eb-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e76eb-161">isFeatured</span></span>|<span data-ttu-id="e76eb-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e76eb-162">Boolean</span></span>|<span data-ttu-id="e76eb-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e76eb-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e76eb-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e76eb-164">privacyInformationUrl</span></span>|<span data-ttu-id="e76eb-165">String</span><span class="sxs-lookup"><span data-stu-id="e76eb-165">String</span></span>|<span data-ttu-id="e76eb-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="e76eb-166">The privacy statement Url.</span></span> <span data-ttu-id="e76eb-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e76eb-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e76eb-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e76eb-168">informationUrl</span></span>|<span data-ttu-id="e76eb-169">String</span><span class="sxs-lookup"><span data-stu-id="e76eb-169">String</span></span>|<span data-ttu-id="e76eb-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="e76eb-170">The more information Url.</span></span> <span data-ttu-id="e76eb-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e76eb-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e76eb-172">owner</span><span class="sxs-lookup"><span data-stu-id="e76eb-172">owner</span></span>|<span data-ttu-id="e76eb-173">String</span><span class="sxs-lookup"><span data-stu-id="e76eb-173">String</span></span>|<span data-ttu-id="e76eb-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="e76eb-174">The owner of the app.</span></span> <span data-ttu-id="e76eb-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e76eb-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e76eb-176">developer</span><span class="sxs-lookup"><span data-stu-id="e76eb-176">developer</span></span>|<span data-ttu-id="e76eb-177">String</span><span class="sxs-lookup"><span data-stu-id="e76eb-177">String</span></span>|<span data-ttu-id="e76eb-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="e76eb-178">The developer of the app.</span></span> <span data-ttu-id="e76eb-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e76eb-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e76eb-180">notes</span><span class="sxs-lookup"><span data-stu-id="e76eb-180">notes</span></span>|<span data-ttu-id="e76eb-181">String</span><span class="sxs-lookup"><span data-stu-id="e76eb-181">String</span></span>|<span data-ttu-id="e76eb-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="e76eb-182">Notes for the app.</span></span> <span data-ttu-id="e76eb-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e76eb-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e76eb-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="e76eb-184">uploadState</span></span>|<span data-ttu-id="e76eb-185">Int32</span><span class="sxs-lookup"><span data-stu-id="e76eb-185">Int32</span></span>|<span data-ttu-id="e76eb-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="e76eb-186">The upload state.</span></span> <span data-ttu-id="e76eb-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e76eb-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e76eb-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="e76eb-188">publishingState</span></span>|[<span data-ttu-id="e76eb-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e76eb-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e76eb-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="e76eb-190">The publishing state for the app.</span></span> <span data-ttu-id="e76eb-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="e76eb-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e76eb-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e76eb-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e76eb-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="e76eb-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e76eb-194">appUrl</span><span class="sxs-lookup"><span data-stu-id="e76eb-194">appUrl</span></span>|<span data-ttu-id="e76eb-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e76eb-195">String</span></span>|<span data-ttu-id="e76eb-196">Die URL der Web-App.</span><span class="sxs-lookup"><span data-stu-id="e76eb-196">The web app URL.</span></span>|
|<span data-ttu-id="e76eb-197">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="e76eb-197">useManagedBrowser</span></span>|<span data-ttu-id="e76eb-198">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e76eb-198">Boolean</span></span>|<span data-ttu-id="e76eb-199">Gibt an, ob ein verwalteter Browser verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="e76eb-199">Whether or not to use managed browser.</span></span> <span data-ttu-id="e76eb-200">Diese Eigenschaft ist nur für Android und IOS möglich.</span><span class="sxs-lookup"><span data-stu-id="e76eb-200">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="e76eb-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="e76eb-201">Response</span></span>
<span data-ttu-id="e76eb-202">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [webApp](../resources/intune-apps-webapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e76eb-202">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e76eb-203">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e76eb-203">Example</span></span>
### <a name="request"></a><span data-ttu-id="e76eb-204">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e76eb-204">Request</span></span>
<span data-ttu-id="e76eb-205">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e76eb-205">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 686

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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="e76eb-206">Antwort</span><span class="sxs-lookup"><span data-stu-id="e76eb-206">Response</span></span>
<span data-ttu-id="e76eb-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e76eb-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





