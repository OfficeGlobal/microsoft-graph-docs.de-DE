---
title: webApp aktualisieren
description: Aktualisieren der Eigenschaften eines webApp-Objekts.
ms.openlocfilehash: 666ce1d255cfe9fdd3f5ed2067a2e9fa7d7082ba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019191"
---
# <a name="update-webapp"></a><span data-ttu-id="53231-103">webApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="53231-103">Update webApp</span></span>

> <span data-ttu-id="53231-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="53231-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53231-105">Aktualisieren der Eigenschaften eines [webApp](../resources/intune-apps-webapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="53231-105">Update the properties of a [webApp](../resources/intune-apps-webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="53231-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="53231-106">Prerequisites</span></span>
<span data-ttu-id="53231-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53231-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53231-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="53231-109">Permission type</span></span>|<span data-ttu-id="53231-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="53231-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53231-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="53231-111">Delegated (work or school account)</span></span>|<span data-ttu-id="53231-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53231-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="53231-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="53231-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53231-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53231-114">Not supported.</span></span>|
|<span data-ttu-id="53231-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="53231-115">Application</span></span>|<span data-ttu-id="53231-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="53231-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53231-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="53231-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="53231-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="53231-118">Request headers</span></span>
|<span data-ttu-id="53231-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="53231-119">Header</span></span>|<span data-ttu-id="53231-120">Wert</span><span class="sxs-lookup"><span data-stu-id="53231-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53231-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="53231-121">Authorization</span></span>|<span data-ttu-id="53231-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="53231-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53231-123">Accept</span><span class="sxs-lookup"><span data-stu-id="53231-123">Accept</span></span>|<span data-ttu-id="53231-124">application/json</span><span class="sxs-lookup"><span data-stu-id="53231-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53231-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="53231-125">Request body</span></span>
<span data-ttu-id="53231-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [webApp](../resources/intune-apps-webapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="53231-126">In the request body, supply a JSON representation for the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

<span data-ttu-id="53231-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [webApp](../resources/intune-apps-webapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="53231-127">The following table shows the properties that are required when you create the [webApp](../resources/intune-apps-webapp.md).</span></span>

|<span data-ttu-id="53231-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="53231-128">Property</span></span>|<span data-ttu-id="53231-129">Typ</span><span class="sxs-lookup"><span data-stu-id="53231-129">Type</span></span>|<span data-ttu-id="53231-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53231-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53231-131">id</span><span class="sxs-lookup"><span data-stu-id="53231-131">id</span></span>|<span data-ttu-id="53231-132">String</span><span class="sxs-lookup"><span data-stu-id="53231-132">String</span></span>|<span data-ttu-id="53231-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="53231-133">Key of the entity.</span></span> <span data-ttu-id="53231-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53231-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53231-135">displayName</span><span class="sxs-lookup"><span data-stu-id="53231-135">displayName</span></span>|<span data-ttu-id="53231-136">String</span><span class="sxs-lookup"><span data-stu-id="53231-136">String</span></span>|<span data-ttu-id="53231-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="53231-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="53231-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53231-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53231-139">description</span><span class="sxs-lookup"><span data-stu-id="53231-139">description</span></span>|<span data-ttu-id="53231-140">String</span><span class="sxs-lookup"><span data-stu-id="53231-140">String</span></span>|<span data-ttu-id="53231-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="53231-141">The description of the app.</span></span> <span data-ttu-id="53231-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53231-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53231-143">publisher</span><span class="sxs-lookup"><span data-stu-id="53231-143">publisher</span></span>|<span data-ttu-id="53231-144">String</span><span class="sxs-lookup"><span data-stu-id="53231-144">String</span></span>|<span data-ttu-id="53231-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="53231-145">The publisher of the app.</span></span> <span data-ttu-id="53231-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53231-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53231-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="53231-147">largeIcon</span></span>|[<span data-ttu-id="53231-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="53231-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="53231-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="53231-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="53231-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53231-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53231-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="53231-151">createdDateTime</span></span>|<span data-ttu-id="53231-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53231-152">DateTimeOffset</span></span>|<span data-ttu-id="53231-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="53231-153">The date and time the app was created.</span></span> <span data-ttu-id="53231-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53231-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53231-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53231-155">lastModifiedDateTime</span></span>|<span data-ttu-id="53231-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53231-156">DateTimeOffset</span></span>|<span data-ttu-id="53231-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="53231-157">The date and time the app was last modified.</span></span> <span data-ttu-id="53231-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53231-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53231-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="53231-159">isFeatured</span></span>|<span data-ttu-id="53231-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="53231-160">Boolean</span></span>|<span data-ttu-id="53231-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53231-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53231-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="53231-162">privacyInformationUrl</span></span>|<span data-ttu-id="53231-163">String</span><span class="sxs-lookup"><span data-stu-id="53231-163">String</span></span>|<span data-ttu-id="53231-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="53231-164">The privacy statement Url.</span></span> <span data-ttu-id="53231-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53231-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53231-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="53231-166">informationUrl</span></span>|<span data-ttu-id="53231-167">String</span><span class="sxs-lookup"><span data-stu-id="53231-167">String</span></span>|<span data-ttu-id="53231-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="53231-168">The more information Url.</span></span> <span data-ttu-id="53231-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53231-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53231-170">owner</span><span class="sxs-lookup"><span data-stu-id="53231-170">owner</span></span>|<span data-ttu-id="53231-171">String</span><span class="sxs-lookup"><span data-stu-id="53231-171">String</span></span>|<span data-ttu-id="53231-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="53231-172">The owner of the app.</span></span> <span data-ttu-id="53231-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53231-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53231-174">developer</span><span class="sxs-lookup"><span data-stu-id="53231-174">developer</span></span>|<span data-ttu-id="53231-175">String</span><span class="sxs-lookup"><span data-stu-id="53231-175">String</span></span>|<span data-ttu-id="53231-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="53231-176">The developer of the app.</span></span> <span data-ttu-id="53231-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53231-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53231-178">notes</span><span class="sxs-lookup"><span data-stu-id="53231-178">notes</span></span>|<span data-ttu-id="53231-179">String</span><span class="sxs-lookup"><span data-stu-id="53231-179">String</span></span>|<span data-ttu-id="53231-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="53231-180">Notes for the app.</span></span> <span data-ttu-id="53231-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53231-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="53231-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="53231-182">publishingState</span></span>|[<span data-ttu-id="53231-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="53231-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="53231-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="53231-184">The publishing state for the app.</span></span> <span data-ttu-id="53231-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="53231-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="53231-186">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53231-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="53231-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="53231-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="53231-188">appUrl</span><span class="sxs-lookup"><span data-stu-id="53231-188">appUrl</span></span>|<span data-ttu-id="53231-189">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="53231-189">String</span></span>|<span data-ttu-id="53231-190">Die URL der Web-App.</span><span class="sxs-lookup"><span data-stu-id="53231-190">The web app URL.</span></span>|
|<span data-ttu-id="53231-191">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="53231-191">useManagedBrowser</span></span>|<span data-ttu-id="53231-192">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="53231-192">Boolean</span></span>|<span data-ttu-id="53231-193">Gibt an, ob ein verwalteter Browser verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="53231-193">Whether or not to use managed browser.</span></span> <span data-ttu-id="53231-194">Diese Eigenschaft ist nur für Android und IOS möglich.</span><span class="sxs-lookup"><span data-stu-id="53231-194">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="53231-195">Antwort</span><span class="sxs-lookup"><span data-stu-id="53231-195">Response</span></span>
<span data-ttu-id="53231-196">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [webApp](../resources/intune-apps-webapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53231-196">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53231-197">Beispiel</span><span class="sxs-lookup"><span data-stu-id="53231-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="53231-198">Anforderung</span><span class="sxs-lookup"><span data-stu-id="53231-198">Request</span></span>
<span data-ttu-id="53231-199">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="53231-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="53231-200">Antwort</span><span class="sxs-lookup"><span data-stu-id="53231-200">Response</span></span>
<span data-ttu-id="53231-p116">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="53231-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



