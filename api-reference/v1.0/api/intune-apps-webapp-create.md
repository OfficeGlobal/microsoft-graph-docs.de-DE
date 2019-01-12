---
title: webApp erstellen
description: Erstellen eines neuen webApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7e527046d7ffc2c3fce99ec251a5aea21801c2ea
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933659"
---
# <a name="create-webapp"></a><span data-ttu-id="e3312-103">webApp erstellen</span><span class="sxs-lookup"><span data-stu-id="e3312-103">Create webApp</span></span>

> <span data-ttu-id="e3312-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e3312-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3312-105">Erstellen eines neuen [webApp](../resources/intune-apps-webapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e3312-105">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e3312-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e3312-106">Prerequisites</span></span>
<span data-ttu-id="e3312-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3312-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3312-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e3312-109">Permission type</span></span>|<span data-ttu-id="e3312-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e3312-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3312-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e3312-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e3312-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3312-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e3312-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e3312-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3312-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3312-114">Not supported.</span></span>|
|<span data-ttu-id="e3312-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e3312-115">Application</span></span>|<span data-ttu-id="e3312-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e3312-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3312-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3312-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e3312-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e3312-118">Request headers</span></span>
|<span data-ttu-id="e3312-119">Header</span><span class="sxs-lookup"><span data-stu-id="e3312-119">Header</span></span>|<span data-ttu-id="e3312-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e3312-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3312-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3312-121">Authorization</span></span>|<span data-ttu-id="e3312-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e3312-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3312-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e3312-123">Accept</span></span>|<span data-ttu-id="e3312-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e3312-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3312-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e3312-125">Request body</span></span>
<span data-ttu-id="e3312-126">Geben Sie im Anforderungstext eine JSON-Darstellung des webApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e3312-126">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="e3312-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der webApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e3312-127">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="e3312-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e3312-128">Property</span></span>|<span data-ttu-id="e3312-129">Typ</span><span class="sxs-lookup"><span data-stu-id="e3312-129">Type</span></span>|<span data-ttu-id="e3312-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3312-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3312-131">id</span><span class="sxs-lookup"><span data-stu-id="e3312-131">id</span></span>|<span data-ttu-id="e3312-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3312-132">String</span></span>|<span data-ttu-id="e3312-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e3312-133">Key of the entity.</span></span> <span data-ttu-id="e3312-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3312-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3312-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e3312-135">displayName</span></span>|<span data-ttu-id="e3312-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3312-136">String</span></span>|<span data-ttu-id="e3312-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="e3312-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e3312-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3312-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3312-139">description</span><span class="sxs-lookup"><span data-stu-id="e3312-139">description</span></span>|<span data-ttu-id="e3312-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3312-140">String</span></span>|<span data-ttu-id="e3312-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="e3312-141">The description of the app.</span></span> <span data-ttu-id="e3312-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3312-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3312-143">publisher</span><span class="sxs-lookup"><span data-stu-id="e3312-143">publisher</span></span>|<span data-ttu-id="e3312-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3312-144">String</span></span>|<span data-ttu-id="e3312-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="e3312-145">The publisher of the app.</span></span> <span data-ttu-id="e3312-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3312-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3312-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e3312-147">largeIcon</span></span>|[<span data-ttu-id="e3312-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e3312-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e3312-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="e3312-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e3312-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3312-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3312-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e3312-151">createdDateTime</span></span>|<span data-ttu-id="e3312-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3312-152">DateTimeOffset</span></span>|<span data-ttu-id="e3312-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="e3312-153">The date and time the app was created.</span></span> <span data-ttu-id="e3312-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3312-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3312-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3312-155">lastModifiedDateTime</span></span>|<span data-ttu-id="e3312-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3312-156">DateTimeOffset</span></span>|<span data-ttu-id="e3312-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="e3312-157">The date and time the app was last modified.</span></span> <span data-ttu-id="e3312-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3312-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3312-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e3312-159">isFeatured</span></span>|<span data-ttu-id="e3312-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e3312-160">Boolean</span></span>|<span data-ttu-id="e3312-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3312-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3312-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e3312-162">privacyInformationUrl</span></span>|<span data-ttu-id="e3312-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3312-163">String</span></span>|<span data-ttu-id="e3312-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="e3312-164">The privacy statement Url.</span></span> <span data-ttu-id="e3312-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3312-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3312-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e3312-166">informationUrl</span></span>|<span data-ttu-id="e3312-167">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3312-167">String</span></span>|<span data-ttu-id="e3312-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="e3312-168">The more information Url.</span></span> <span data-ttu-id="e3312-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3312-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3312-170">owner</span><span class="sxs-lookup"><span data-stu-id="e3312-170">owner</span></span>|<span data-ttu-id="e3312-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3312-171">String</span></span>|<span data-ttu-id="e3312-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="e3312-172">The owner of the app.</span></span> <span data-ttu-id="e3312-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3312-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3312-174">developer</span><span class="sxs-lookup"><span data-stu-id="e3312-174">developer</span></span>|<span data-ttu-id="e3312-175">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3312-175">String</span></span>|<span data-ttu-id="e3312-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="e3312-176">The developer of the app.</span></span> <span data-ttu-id="e3312-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3312-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3312-178">notes</span><span class="sxs-lookup"><span data-stu-id="e3312-178">notes</span></span>|<span data-ttu-id="e3312-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3312-179">String</span></span>|<span data-ttu-id="e3312-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="e3312-180">Notes for the app.</span></span> <span data-ttu-id="e3312-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3312-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3312-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="e3312-182">publishingState</span></span>|[<span data-ttu-id="e3312-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e3312-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e3312-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="e3312-184">The publishing state for the app.</span></span> <span data-ttu-id="e3312-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="e3312-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e3312-186">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3312-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e3312-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="e3312-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e3312-188">appUrl</span><span class="sxs-lookup"><span data-stu-id="e3312-188">appUrl</span></span>|<span data-ttu-id="e3312-189">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e3312-189">String</span></span>|<span data-ttu-id="e3312-190">Die URL der Web-App.</span><span class="sxs-lookup"><span data-stu-id="e3312-190">The web app URL.</span></span>|
|<span data-ttu-id="e3312-191">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="e3312-191">useManagedBrowser</span></span>|<span data-ttu-id="e3312-192">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e3312-192">Boolean</span></span>|<span data-ttu-id="e3312-193">Gibt an, ob ein verwalteter Browser verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="e3312-193">Whether or not to use managed browser.</span></span> <span data-ttu-id="e3312-194">Diese Eigenschaft ist nur für Android und IOS möglich.</span><span class="sxs-lookup"><span data-stu-id="e3312-194">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="e3312-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3312-195">Response</span></span>
<span data-ttu-id="e3312-196">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [webApp](../resources/intune-apps-webapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e3312-196">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3312-197">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e3312-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="e3312-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e3312-198">Request</span></span>
<span data-ttu-id="e3312-199">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e3312-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e3312-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="e3312-200">Response</span></span>
<span data-ttu-id="e3312-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e3312-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



