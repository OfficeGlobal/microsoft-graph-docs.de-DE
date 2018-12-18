---
title: webApp erstellen
description: Erstellen eines neuen webApp-Objekts.
author: tfitzmac
ms.openlocfilehash: 75d26e735db898f6175aed3ce5999c3a47e6bcdb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343792"
---
# <a name="create-webapp"></a><span data-ttu-id="99b22-103">webApp erstellen</span><span class="sxs-lookup"><span data-stu-id="99b22-103">Create webApp</span></span>

> <span data-ttu-id="99b22-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="99b22-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99b22-105">Erstellen eines neuen [webApp](../resources/intune-apps-webapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="99b22-105">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="99b22-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="99b22-106">Prerequisites</span></span>
<span data-ttu-id="99b22-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99b22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99b22-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="99b22-109">Permission type</span></span>|<span data-ttu-id="99b22-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="99b22-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99b22-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="99b22-111">Delegated (work or school account)</span></span>|<span data-ttu-id="99b22-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99b22-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="99b22-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="99b22-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99b22-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="99b22-114">Not supported.</span></span>|
|<span data-ttu-id="99b22-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="99b22-115">Application</span></span>|<span data-ttu-id="99b22-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="99b22-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99b22-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="99b22-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="99b22-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="99b22-118">Request headers</span></span>
|<span data-ttu-id="99b22-119">Header</span><span class="sxs-lookup"><span data-stu-id="99b22-119">Header</span></span>|<span data-ttu-id="99b22-120">Wert</span><span class="sxs-lookup"><span data-stu-id="99b22-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99b22-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="99b22-121">Authorization</span></span>|<span data-ttu-id="99b22-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="99b22-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99b22-123">Accept</span><span class="sxs-lookup"><span data-stu-id="99b22-123">Accept</span></span>|<span data-ttu-id="99b22-124">application/json</span><span class="sxs-lookup"><span data-stu-id="99b22-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99b22-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="99b22-125">Request body</span></span>
<span data-ttu-id="99b22-126">Geben Sie im Anforderungstext eine JSON-Darstellung des webApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="99b22-126">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="99b22-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der webApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="99b22-127">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="99b22-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="99b22-128">Property</span></span>|<span data-ttu-id="99b22-129">Typ</span><span class="sxs-lookup"><span data-stu-id="99b22-129">Type</span></span>|<span data-ttu-id="99b22-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="99b22-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99b22-131">id</span><span class="sxs-lookup"><span data-stu-id="99b22-131">id</span></span>|<span data-ttu-id="99b22-132">String</span><span class="sxs-lookup"><span data-stu-id="99b22-132">String</span></span>|<span data-ttu-id="99b22-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="99b22-133">Key of the entity.</span></span> <span data-ttu-id="99b22-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b22-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b22-135">displayName</span><span class="sxs-lookup"><span data-stu-id="99b22-135">displayName</span></span>|<span data-ttu-id="99b22-136">String</span><span class="sxs-lookup"><span data-stu-id="99b22-136">String</span></span>|<span data-ttu-id="99b22-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="99b22-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="99b22-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b22-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b22-139">description</span><span class="sxs-lookup"><span data-stu-id="99b22-139">description</span></span>|<span data-ttu-id="99b22-140">String</span><span class="sxs-lookup"><span data-stu-id="99b22-140">String</span></span>|<span data-ttu-id="99b22-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="99b22-141">The description of the app.</span></span> <span data-ttu-id="99b22-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b22-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b22-143">publisher</span><span class="sxs-lookup"><span data-stu-id="99b22-143">publisher</span></span>|<span data-ttu-id="99b22-144">String</span><span class="sxs-lookup"><span data-stu-id="99b22-144">String</span></span>|<span data-ttu-id="99b22-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="99b22-145">The publisher of the app.</span></span> <span data-ttu-id="99b22-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b22-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b22-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="99b22-147">largeIcon</span></span>|[<span data-ttu-id="99b22-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="99b22-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="99b22-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="99b22-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="99b22-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b22-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b22-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="99b22-151">createdDateTime</span></span>|<span data-ttu-id="99b22-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99b22-152">DateTimeOffset</span></span>|<span data-ttu-id="99b22-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="99b22-153">The date and time the app was created.</span></span> <span data-ttu-id="99b22-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b22-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b22-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99b22-155">lastModifiedDateTime</span></span>|<span data-ttu-id="99b22-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99b22-156">DateTimeOffset</span></span>|<span data-ttu-id="99b22-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="99b22-157">The date and time the app was last modified.</span></span> <span data-ttu-id="99b22-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b22-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b22-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="99b22-159">isFeatured</span></span>|<span data-ttu-id="99b22-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="99b22-160">Boolean</span></span>|<span data-ttu-id="99b22-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b22-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b22-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="99b22-162">privacyInformationUrl</span></span>|<span data-ttu-id="99b22-163">String</span><span class="sxs-lookup"><span data-stu-id="99b22-163">String</span></span>|<span data-ttu-id="99b22-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="99b22-164">The privacy statement Url.</span></span> <span data-ttu-id="99b22-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b22-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b22-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="99b22-166">informationUrl</span></span>|<span data-ttu-id="99b22-167">String</span><span class="sxs-lookup"><span data-stu-id="99b22-167">String</span></span>|<span data-ttu-id="99b22-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="99b22-168">The more information Url.</span></span> <span data-ttu-id="99b22-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b22-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b22-170">owner</span><span class="sxs-lookup"><span data-stu-id="99b22-170">owner</span></span>|<span data-ttu-id="99b22-171">String</span><span class="sxs-lookup"><span data-stu-id="99b22-171">String</span></span>|<span data-ttu-id="99b22-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="99b22-172">The owner of the app.</span></span> <span data-ttu-id="99b22-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b22-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b22-174">developer</span><span class="sxs-lookup"><span data-stu-id="99b22-174">developer</span></span>|<span data-ttu-id="99b22-175">String</span><span class="sxs-lookup"><span data-stu-id="99b22-175">String</span></span>|<span data-ttu-id="99b22-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="99b22-176">The developer of the app.</span></span> <span data-ttu-id="99b22-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b22-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b22-178">notes</span><span class="sxs-lookup"><span data-stu-id="99b22-178">notes</span></span>|<span data-ttu-id="99b22-179">String</span><span class="sxs-lookup"><span data-stu-id="99b22-179">String</span></span>|<span data-ttu-id="99b22-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="99b22-180">Notes for the app.</span></span> <span data-ttu-id="99b22-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b22-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99b22-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="99b22-182">publishingState</span></span>|[<span data-ttu-id="99b22-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="99b22-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="99b22-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="99b22-184">The publishing state for the app.</span></span> <span data-ttu-id="99b22-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="99b22-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="99b22-186">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99b22-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="99b22-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="99b22-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="99b22-188">appUrl</span><span class="sxs-lookup"><span data-stu-id="99b22-188">appUrl</span></span>|<span data-ttu-id="99b22-189">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="99b22-189">String</span></span>|<span data-ttu-id="99b22-190">Die URL der Web-App.</span><span class="sxs-lookup"><span data-stu-id="99b22-190">The web app URL.</span></span>|
|<span data-ttu-id="99b22-191">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="99b22-191">useManagedBrowser</span></span>|<span data-ttu-id="99b22-192">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="99b22-192">Boolean</span></span>|<span data-ttu-id="99b22-193">Gibt an, ob ein verwalteter Browser verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="99b22-193">Whether or not to use managed browser.</span></span> <span data-ttu-id="99b22-194">Diese Eigenschaft ist nur für Android und IOS möglich.</span><span class="sxs-lookup"><span data-stu-id="99b22-194">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="99b22-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="99b22-195">Response</span></span>
<span data-ttu-id="99b22-196">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [webApp](../resources/intune-apps-webapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="99b22-196">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99b22-197">Beispiel</span><span class="sxs-lookup"><span data-stu-id="99b22-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="99b22-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="99b22-198">Request</span></span>
<span data-ttu-id="99b22-199">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="99b22-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 645

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
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="99b22-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="99b22-200">Response</span></span>
<span data-ttu-id="99b22-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="99b22-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 817

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
  "publishingState": "processing",
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```



