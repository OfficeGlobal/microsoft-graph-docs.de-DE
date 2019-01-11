---
title: Aktualisieren von „macOSOfficeSuiteApp“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs macOSOfficeSuiteApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 545a9e6e36ec7860b3cad4f0865d59f397b64079
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813895"
---
# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="ec475-103">Aktualisieren von „macOSOfficeSuiteApp“</span><span class="sxs-lookup"><span data-stu-id="ec475-103">Update macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="ec475-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ec475-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec475-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ec475-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ec475-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ec475-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ec475-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="ec475-107">Update the properties of a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ec475-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ec475-108">Prerequisites</span></span>
<span data-ttu-id="ec475-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec475-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec475-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ec475-111">Permission type</span></span>|<span data-ttu-id="ec475-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ec475-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec475-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ec475-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ec475-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec475-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ec475-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ec475-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec475-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ec475-116">Not supported.</span></span>|
|<span data-ttu-id="ec475-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ec475-117">Application</span></span>|<span data-ttu-id="ec475-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ec475-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec475-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec475-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="ec475-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ec475-120">Request headers</span></span>
|<span data-ttu-id="ec475-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ec475-121">Header</span></span>|<span data-ttu-id="ec475-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ec475-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec475-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec475-123">Authorization</span></span>|<span data-ttu-id="ec475-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ec475-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec475-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ec475-125">Accept</span></span>|<span data-ttu-id="ec475-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ec475-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec475-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ec475-127">Request body</span></span>
<span data-ttu-id="ec475-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekt des Typs [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) an.</span><span class="sxs-lookup"><span data-stu-id="ec475-128">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="ec475-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="ec475-129">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="ec475-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ec475-130">Property</span></span>|<span data-ttu-id="ec475-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ec475-131">Type</span></span>|<span data-ttu-id="ec475-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ec475-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec475-133">id</span><span class="sxs-lookup"><span data-stu-id="ec475-133">id</span></span>|<span data-ttu-id="ec475-134">String</span><span class="sxs-lookup"><span data-stu-id="ec475-134">String</span></span>|<span data-ttu-id="ec475-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ec475-135">Key of the entity.</span></span> <span data-ttu-id="ec475-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ec475-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec475-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ec475-137">displayName</span></span>|<span data-ttu-id="ec475-138">String</span><span class="sxs-lookup"><span data-stu-id="ec475-138">String</span></span>|<span data-ttu-id="ec475-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="ec475-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ec475-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ec475-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec475-141">description</span><span class="sxs-lookup"><span data-stu-id="ec475-141">description</span></span>|<span data-ttu-id="ec475-142">String</span><span class="sxs-lookup"><span data-stu-id="ec475-142">String</span></span>|<span data-ttu-id="ec475-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="ec475-143">The description of the app.</span></span> <span data-ttu-id="ec475-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ec475-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec475-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ec475-145">publisher</span></span>|<span data-ttu-id="ec475-146">String</span><span class="sxs-lookup"><span data-stu-id="ec475-146">String</span></span>|<span data-ttu-id="ec475-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="ec475-147">The publisher of the app.</span></span> <span data-ttu-id="ec475-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ec475-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec475-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ec475-149">largeIcon</span></span>|[<span data-ttu-id="ec475-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ec475-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ec475-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="ec475-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ec475-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ec475-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec475-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ec475-153">createdDateTime</span></span>|<span data-ttu-id="ec475-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec475-154">DateTimeOffset</span></span>|<span data-ttu-id="ec475-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="ec475-155">The date and time the app was created.</span></span> <span data-ttu-id="ec475-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ec475-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec475-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ec475-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ec475-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec475-158">DateTimeOffset</span></span>|<span data-ttu-id="ec475-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="ec475-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ec475-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ec475-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec475-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ec475-161">isFeatured</span></span>|<span data-ttu-id="ec475-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec475-162">Boolean</span></span>|<span data-ttu-id="ec475-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ec475-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec475-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ec475-164">privacyInformationUrl</span></span>|<span data-ttu-id="ec475-165">String</span><span class="sxs-lookup"><span data-stu-id="ec475-165">String</span></span>|<span data-ttu-id="ec475-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="ec475-166">The privacy statement Url.</span></span> <span data-ttu-id="ec475-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ec475-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec475-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ec475-168">informationUrl</span></span>|<span data-ttu-id="ec475-169">String</span><span class="sxs-lookup"><span data-stu-id="ec475-169">String</span></span>|<span data-ttu-id="ec475-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="ec475-170">The more information Url.</span></span> <span data-ttu-id="ec475-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ec475-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec475-172">owner</span><span class="sxs-lookup"><span data-stu-id="ec475-172">owner</span></span>|<span data-ttu-id="ec475-173">String</span><span class="sxs-lookup"><span data-stu-id="ec475-173">String</span></span>|<span data-ttu-id="ec475-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="ec475-174">The owner of the app.</span></span> <span data-ttu-id="ec475-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ec475-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec475-176">developer</span><span class="sxs-lookup"><span data-stu-id="ec475-176">developer</span></span>|<span data-ttu-id="ec475-177">String</span><span class="sxs-lookup"><span data-stu-id="ec475-177">String</span></span>|<span data-ttu-id="ec475-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="ec475-178">The developer of the app.</span></span> <span data-ttu-id="ec475-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ec475-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec475-180">notes</span><span class="sxs-lookup"><span data-stu-id="ec475-180">notes</span></span>|<span data-ttu-id="ec475-181">String</span><span class="sxs-lookup"><span data-stu-id="ec475-181">String</span></span>|<span data-ttu-id="ec475-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="ec475-182">Notes for the app.</span></span> <span data-ttu-id="ec475-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ec475-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec475-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ec475-184">uploadState</span></span>|<span data-ttu-id="ec475-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ec475-185">Int32</span></span>|<span data-ttu-id="ec475-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="ec475-186">The upload state.</span></span> <span data-ttu-id="ec475-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ec475-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ec475-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="ec475-188">publishingState</span></span>|[<span data-ttu-id="ec475-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ec475-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ec475-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="ec475-190">The publishing state for the app.</span></span> <span data-ttu-id="ec475-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="ec475-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ec475-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ec475-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="ec475-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="ec475-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="ec475-194">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec475-194">Response</span></span>
<span data-ttu-id="ec475-195">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ec475-195">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec475-196">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ec475-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="ec475-197">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec475-197">Request</span></span>
<span data-ttu-id="ec475-198">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ec475-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 612

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
  "publishingState": "processing"
}
```

### <a name="response"></a><span data-ttu-id="ec475-199">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec475-199">Response</span></span>
<span data-ttu-id="ec475-p117">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ec475-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 778

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
  "id": "bf39e35d-e35d-bf39-5de3-39bf5de339bf",
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
  "publishingState": "processing"
}
```





