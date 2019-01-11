---
title: webApp erstellen
description: Erstellen eines neuen webApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5e6ee095d9c162f8fe738716b4c966d6560d24dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882089"
---
# <a name="create-webapp"></a><span data-ttu-id="e24b9-103">webApp erstellen</span><span class="sxs-lookup"><span data-stu-id="e24b9-103">Create webApp</span></span>

> <span data-ttu-id="e24b9-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e24b9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e24b9-105">Erstellen eines neuen [webApp](../resources/intune-apps-webapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e24b9-105">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e24b9-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e24b9-106">Prerequisites</span></span>
<span data-ttu-id="e24b9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e24b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e24b9-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e24b9-109">Permission type</span></span>|<span data-ttu-id="e24b9-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e24b9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e24b9-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e24b9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e24b9-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e24b9-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e24b9-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e24b9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e24b9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e24b9-114">Not supported.</span></span>|
|<span data-ttu-id="e24b9-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e24b9-115">Application</span></span>|<span data-ttu-id="e24b9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e24b9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e24b9-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e24b9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e24b9-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e24b9-118">Request headers</span></span>
|<span data-ttu-id="e24b9-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e24b9-119">Header</span></span>|<span data-ttu-id="e24b9-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e24b9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e24b9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e24b9-121">Authorization</span></span>|<span data-ttu-id="e24b9-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e24b9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e24b9-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e24b9-123">Accept</span></span>|<span data-ttu-id="e24b9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e24b9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e24b9-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e24b9-125">Request body</span></span>
<span data-ttu-id="e24b9-126">Geben Sie im Anforderungstext eine JSON-Darstellung des webApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e24b9-126">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="e24b9-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der webApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e24b9-127">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="e24b9-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e24b9-128">Property</span></span>|<span data-ttu-id="e24b9-129">Typ</span><span class="sxs-lookup"><span data-stu-id="e24b9-129">Type</span></span>|<span data-ttu-id="e24b9-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e24b9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e24b9-131">id</span><span class="sxs-lookup"><span data-stu-id="e24b9-131">id</span></span>|<span data-ttu-id="e24b9-132">String</span><span class="sxs-lookup"><span data-stu-id="e24b9-132">String</span></span>|<span data-ttu-id="e24b9-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e24b9-133">Key of the entity.</span></span> <span data-ttu-id="e24b9-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e24b9-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e24b9-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e24b9-135">displayName</span></span>|<span data-ttu-id="e24b9-136">String</span><span class="sxs-lookup"><span data-stu-id="e24b9-136">String</span></span>|<span data-ttu-id="e24b9-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="e24b9-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e24b9-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e24b9-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e24b9-139">description</span><span class="sxs-lookup"><span data-stu-id="e24b9-139">description</span></span>|<span data-ttu-id="e24b9-140">String</span><span class="sxs-lookup"><span data-stu-id="e24b9-140">String</span></span>|<span data-ttu-id="e24b9-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="e24b9-141">The description of the app.</span></span> <span data-ttu-id="e24b9-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e24b9-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e24b9-143">publisher</span><span class="sxs-lookup"><span data-stu-id="e24b9-143">publisher</span></span>|<span data-ttu-id="e24b9-144">String</span><span class="sxs-lookup"><span data-stu-id="e24b9-144">String</span></span>|<span data-ttu-id="e24b9-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="e24b9-145">The publisher of the app.</span></span> <span data-ttu-id="e24b9-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e24b9-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e24b9-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e24b9-147">largeIcon</span></span>|[<span data-ttu-id="e24b9-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e24b9-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e24b9-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="e24b9-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e24b9-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e24b9-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e24b9-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e24b9-151">createdDateTime</span></span>|<span data-ttu-id="e24b9-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e24b9-152">DateTimeOffset</span></span>|<span data-ttu-id="e24b9-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="e24b9-153">The date and time the app was created.</span></span> <span data-ttu-id="e24b9-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e24b9-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e24b9-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e24b9-155">lastModifiedDateTime</span></span>|<span data-ttu-id="e24b9-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e24b9-156">DateTimeOffset</span></span>|<span data-ttu-id="e24b9-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="e24b9-157">The date and time the app was last modified.</span></span> <span data-ttu-id="e24b9-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e24b9-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e24b9-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e24b9-159">isFeatured</span></span>|<span data-ttu-id="e24b9-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="e24b9-160">Boolean</span></span>|<span data-ttu-id="e24b9-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e24b9-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e24b9-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e24b9-162">privacyInformationUrl</span></span>|<span data-ttu-id="e24b9-163">String</span><span class="sxs-lookup"><span data-stu-id="e24b9-163">String</span></span>|<span data-ttu-id="e24b9-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="e24b9-164">The privacy statement Url.</span></span> <span data-ttu-id="e24b9-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e24b9-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e24b9-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e24b9-166">informationUrl</span></span>|<span data-ttu-id="e24b9-167">String</span><span class="sxs-lookup"><span data-stu-id="e24b9-167">String</span></span>|<span data-ttu-id="e24b9-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="e24b9-168">The more information Url.</span></span> <span data-ttu-id="e24b9-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e24b9-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e24b9-170">owner</span><span class="sxs-lookup"><span data-stu-id="e24b9-170">owner</span></span>|<span data-ttu-id="e24b9-171">String</span><span class="sxs-lookup"><span data-stu-id="e24b9-171">String</span></span>|<span data-ttu-id="e24b9-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="e24b9-172">The owner of the app.</span></span> <span data-ttu-id="e24b9-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e24b9-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e24b9-174">developer</span><span class="sxs-lookup"><span data-stu-id="e24b9-174">developer</span></span>|<span data-ttu-id="e24b9-175">String</span><span class="sxs-lookup"><span data-stu-id="e24b9-175">String</span></span>|<span data-ttu-id="e24b9-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="e24b9-176">The developer of the app.</span></span> <span data-ttu-id="e24b9-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e24b9-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e24b9-178">notes</span><span class="sxs-lookup"><span data-stu-id="e24b9-178">notes</span></span>|<span data-ttu-id="e24b9-179">String</span><span class="sxs-lookup"><span data-stu-id="e24b9-179">String</span></span>|<span data-ttu-id="e24b9-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="e24b9-180">Notes for the app.</span></span> <span data-ttu-id="e24b9-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e24b9-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e24b9-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="e24b9-182">publishingState</span></span>|[<span data-ttu-id="e24b9-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e24b9-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e24b9-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="e24b9-184">The publishing state for the app.</span></span> <span data-ttu-id="e24b9-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="e24b9-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e24b9-186">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e24b9-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e24b9-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="e24b9-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e24b9-188">appUrl</span><span class="sxs-lookup"><span data-stu-id="e24b9-188">appUrl</span></span>|<span data-ttu-id="e24b9-189">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e24b9-189">String</span></span>|<span data-ttu-id="e24b9-190">Die URL der Web-App.</span><span class="sxs-lookup"><span data-stu-id="e24b9-190">The web app URL.</span></span>|
|<span data-ttu-id="e24b9-191">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="e24b9-191">useManagedBrowser</span></span>|<span data-ttu-id="e24b9-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="e24b9-192">Boolean</span></span>|<span data-ttu-id="e24b9-193">Gibt an, ob ein verwalteter Browser verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="e24b9-193">Whether or not to use managed browser.</span></span> <span data-ttu-id="e24b9-194">Diese Eigenschaft ist nur für Android und IOS möglich.</span><span class="sxs-lookup"><span data-stu-id="e24b9-194">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="e24b9-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="e24b9-195">Response</span></span>
<span data-ttu-id="e24b9-196">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [webApp](../resources/intune-apps-webapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e24b9-196">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e24b9-197">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e24b9-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="e24b9-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e24b9-198">Request</span></span>
<span data-ttu-id="e24b9-199">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e24b9-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e24b9-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="e24b9-200">Response</span></span>
<span data-ttu-id="e24b9-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e24b9-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



