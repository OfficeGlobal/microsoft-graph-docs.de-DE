---
title: Aktualisieren von „macOSOfficeSuiteApp“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs macOSOfficeSuiteApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 020f5090c85458619eb599e519dae0605ccb310a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830569"
---
# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="b29c2-103">Aktualisieren von „macOSOfficeSuiteApp“</span><span class="sxs-lookup"><span data-stu-id="b29c2-103">Update macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="b29c2-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b29c2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b29c2-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="b29c2-105">Update the properties of a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b29c2-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b29c2-106">Prerequisites</span></span>
<span data-ttu-id="b29c2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b29c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b29c2-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b29c2-109">Permission type</span></span>|<span data-ttu-id="b29c2-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b29c2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b29c2-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b29c2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b29c2-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b29c2-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b29c2-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b29c2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b29c2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b29c2-114">Not supported.</span></span>|
|<span data-ttu-id="b29c2-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b29c2-115">Application</span></span>|<span data-ttu-id="b29c2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b29c2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b29c2-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b29c2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="b29c2-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b29c2-118">Request headers</span></span>
|<span data-ttu-id="b29c2-119">Header</span><span class="sxs-lookup"><span data-stu-id="b29c2-119">Header</span></span>|<span data-ttu-id="b29c2-120">Wert</span><span class="sxs-lookup"><span data-stu-id="b29c2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b29c2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b29c2-121">Authorization</span></span>|<span data-ttu-id="b29c2-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b29c2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b29c2-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b29c2-123">Accept</span></span>|<span data-ttu-id="b29c2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b29c2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b29c2-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b29c2-125">Request body</span></span>
<span data-ttu-id="b29c2-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekt des Typs [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) an.</span><span class="sxs-lookup"><span data-stu-id="b29c2-126">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="b29c2-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="b29c2-127">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="b29c2-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b29c2-128">Property</span></span>|<span data-ttu-id="b29c2-129">Typ</span><span class="sxs-lookup"><span data-stu-id="b29c2-129">Type</span></span>|<span data-ttu-id="b29c2-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b29c2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b29c2-131">id</span><span class="sxs-lookup"><span data-stu-id="b29c2-131">id</span></span>|<span data-ttu-id="b29c2-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b29c2-132">String</span></span>|<span data-ttu-id="b29c2-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b29c2-133">Key of the entity.</span></span> <span data-ttu-id="b29c2-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b29c2-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b29c2-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b29c2-135">displayName</span></span>|<span data-ttu-id="b29c2-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b29c2-136">String</span></span>|<span data-ttu-id="b29c2-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="b29c2-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b29c2-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b29c2-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b29c2-139">description</span><span class="sxs-lookup"><span data-stu-id="b29c2-139">description</span></span>|<span data-ttu-id="b29c2-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b29c2-140">String</span></span>|<span data-ttu-id="b29c2-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="b29c2-141">The description of the app.</span></span> <span data-ttu-id="b29c2-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b29c2-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b29c2-143">publisher</span><span class="sxs-lookup"><span data-stu-id="b29c2-143">publisher</span></span>|<span data-ttu-id="b29c2-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b29c2-144">String</span></span>|<span data-ttu-id="b29c2-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="b29c2-145">The publisher of the app.</span></span> <span data-ttu-id="b29c2-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b29c2-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b29c2-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b29c2-147">largeIcon</span></span>|[<span data-ttu-id="b29c2-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b29c2-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b29c2-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="b29c2-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b29c2-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b29c2-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b29c2-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b29c2-151">createdDateTime</span></span>|<span data-ttu-id="b29c2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b29c2-152">DateTimeOffset</span></span>|<span data-ttu-id="b29c2-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="b29c2-153">The date and time the app was created.</span></span> <span data-ttu-id="b29c2-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b29c2-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b29c2-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b29c2-155">lastModifiedDateTime</span></span>|<span data-ttu-id="b29c2-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b29c2-156">DateTimeOffset</span></span>|<span data-ttu-id="b29c2-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="b29c2-157">The date and time the app was last modified.</span></span> <span data-ttu-id="b29c2-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b29c2-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b29c2-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b29c2-159">isFeatured</span></span>|<span data-ttu-id="b29c2-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b29c2-160">Boolean</span></span>|<span data-ttu-id="b29c2-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b29c2-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b29c2-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b29c2-162">privacyInformationUrl</span></span>|<span data-ttu-id="b29c2-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b29c2-163">String</span></span>|<span data-ttu-id="b29c2-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="b29c2-164">The privacy statement Url.</span></span> <span data-ttu-id="b29c2-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b29c2-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b29c2-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b29c2-166">informationUrl</span></span>|<span data-ttu-id="b29c2-167">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b29c2-167">String</span></span>|<span data-ttu-id="b29c2-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="b29c2-168">The more information Url.</span></span> <span data-ttu-id="b29c2-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b29c2-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b29c2-170">owner</span><span class="sxs-lookup"><span data-stu-id="b29c2-170">owner</span></span>|<span data-ttu-id="b29c2-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b29c2-171">String</span></span>|<span data-ttu-id="b29c2-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="b29c2-172">The owner of the app.</span></span> <span data-ttu-id="b29c2-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b29c2-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b29c2-174">developer</span><span class="sxs-lookup"><span data-stu-id="b29c2-174">developer</span></span>|<span data-ttu-id="b29c2-175">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b29c2-175">String</span></span>|<span data-ttu-id="b29c2-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="b29c2-176">The developer of the app.</span></span> <span data-ttu-id="b29c2-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b29c2-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b29c2-178">notes</span><span class="sxs-lookup"><span data-stu-id="b29c2-178">notes</span></span>|<span data-ttu-id="b29c2-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b29c2-179">String</span></span>|<span data-ttu-id="b29c2-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="b29c2-180">Notes for the app.</span></span> <span data-ttu-id="b29c2-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b29c2-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b29c2-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="b29c2-182">publishingState</span></span>|[<span data-ttu-id="b29c2-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b29c2-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b29c2-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="b29c2-184">The publishing state for the app.</span></span> <span data-ttu-id="b29c2-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="b29c2-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b29c2-186">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b29c2-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b29c2-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="b29c2-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="b29c2-188">Antwort</span><span class="sxs-lookup"><span data-stu-id="b29c2-188">Response</span></span>
<span data-ttu-id="b29c2-189">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b29c2-189">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b29c2-190">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b29c2-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="b29c2-191">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b29c2-191">Request</span></span>
<span data-ttu-id="b29c2-192">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b29c2-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 584

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
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
  "publishingState": "processing"
}
```

### <a name="response"></a><span data-ttu-id="b29c2-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="b29c2-193">Response</span></span>
<span data-ttu-id="b29c2-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b29c2-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

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
  "publishingState": "processing"
}
```



