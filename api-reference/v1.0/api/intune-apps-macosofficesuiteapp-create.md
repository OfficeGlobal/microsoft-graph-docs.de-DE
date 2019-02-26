---
title: Erstellen von „macOSOfficeSuiteApp“
description: Diese Methode erstellt ein neues Objekt des Typs macOSOfficeSuiteApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2df408fe4c5d571789896a93e7b2387f7263a590
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260452"
---
# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="6d3a5-103">Erstellen von „macOSOfficeSuiteApp“</span><span class="sxs-lookup"><span data-stu-id="6d3a5-103">Create macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="6d3a5-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6d3a5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d3a5-105">Diese Methode erstellt ein neues Objekt des Typs [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="6d3a5-105">Create a new [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d3a5-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6d3a5-106">Prerequisites</span></span>
<span data-ttu-id="6d3a5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6d3a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6d3a5-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6d3a5-109">Permission type</span></span>|<span data-ttu-id="6d3a5-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6d3a5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d3a5-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6d3a5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6d3a5-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d3a5-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6d3a5-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6d3a5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d3a5-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6d3a5-114">Not supported.</span></span>|
|<span data-ttu-id="6d3a5-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6d3a5-115">Application</span></span>|<span data-ttu-id="6d3a5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6d3a5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d3a5-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d3a5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="6d3a5-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6d3a5-118">Request headers</span></span>
|<span data-ttu-id="6d3a5-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6d3a5-119">Header</span></span>|<span data-ttu-id="6d3a5-120">Wert</span><span class="sxs-lookup"><span data-stu-id="6d3a5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d3a5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d3a5-121">Authorization</span></span>|<span data-ttu-id="6d3a5-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6d3a5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d3a5-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6d3a5-123">Accept</span></span>|<span data-ttu-id="6d3a5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6d3a5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d3a5-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6d3a5-125">Request body</span></span>
<span data-ttu-id="6d3a5-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekt des Typs „macOSOfficeSuiteApp“ an.</span><span class="sxs-lookup"><span data-stu-id="6d3a5-126">In the request body, supply a JSON representation for the macOSOfficeSuiteApp object.</span></span>

<span data-ttu-id="6d3a5-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „macOSOfficeSuiteApp“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="6d3a5-127">The following table shows the properties that are required when you create the macOSOfficeSuiteApp.</span></span>

|<span data-ttu-id="6d3a5-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6d3a5-128">Property</span></span>|<span data-ttu-id="6d3a5-129">Typ</span><span class="sxs-lookup"><span data-stu-id="6d3a5-129">Type</span></span>|<span data-ttu-id="6d3a5-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d3a5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d3a5-131">id</span><span class="sxs-lookup"><span data-stu-id="6d3a5-131">id</span></span>|<span data-ttu-id="6d3a5-132">string</span><span class="sxs-lookup"><span data-stu-id="6d3a5-132">String</span></span>|<span data-ttu-id="6d3a5-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6d3a5-133">Key of the entity.</span></span> <span data-ttu-id="6d3a5-134">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6d3a5-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6d3a5-135">displayName</span><span class="sxs-lookup"><span data-stu-id="6d3a5-135">displayName</span></span>|<span data-ttu-id="6d3a5-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6d3a5-136">String</span></span>|<span data-ttu-id="6d3a5-137">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="6d3a5-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6d3a5-138">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6d3a5-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6d3a5-139">description</span><span class="sxs-lookup"><span data-stu-id="6d3a5-139">description</span></span>|<span data-ttu-id="6d3a5-140">String</span><span class="sxs-lookup"><span data-stu-id="6d3a5-140">String</span></span>|<span data-ttu-id="6d3a5-141">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="6d3a5-141">The description of the app.</span></span> <span data-ttu-id="6d3a5-142">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6d3a5-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6d3a5-143">publisher</span><span class="sxs-lookup"><span data-stu-id="6d3a5-143">publisher</span></span>|<span data-ttu-id="6d3a5-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6d3a5-144">String</span></span>|<span data-ttu-id="6d3a5-145">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="6d3a5-145">The publisher of the app.</span></span> <span data-ttu-id="6d3a5-146">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6d3a5-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6d3a5-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6d3a5-147">largeIcon</span></span>|[<span data-ttu-id="6d3a5-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6d3a5-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6d3a5-149">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="6d3a5-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6d3a5-150">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6d3a5-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6d3a5-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6d3a5-151">createdDateTime</span></span>|<span data-ttu-id="6d3a5-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d3a5-152">DateTimeOffset</span></span>|<span data-ttu-id="6d3a5-153">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="6d3a5-153">The date and time the app was created.</span></span> <span data-ttu-id="6d3a5-154">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6d3a5-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6d3a5-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d3a5-155">lastModifiedDateTime</span></span>|<span data-ttu-id="6d3a5-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d3a5-156">DateTimeOffset</span></span>|<span data-ttu-id="6d3a5-157">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="6d3a5-157">The date and time the app was last modified.</span></span> <span data-ttu-id="6d3a5-158">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6d3a5-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6d3a5-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6d3a5-159">isFeatured</span></span>|<span data-ttu-id="6d3a5-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d3a5-160">Boolean</span></span>|<span data-ttu-id="6d3a5-161">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6d3a5-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6d3a5-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6d3a5-162">privacyInformationUrl</span></span>|<span data-ttu-id="6d3a5-163">String</span><span class="sxs-lookup"><span data-stu-id="6d3a5-163">String</span></span>|<span data-ttu-id="6d3a5-164">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="6d3a5-164">The privacy statement Url.</span></span> <span data-ttu-id="6d3a5-165">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6d3a5-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6d3a5-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6d3a5-166">informationUrl</span></span>|<span data-ttu-id="6d3a5-167">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6d3a5-167">String</span></span>|<span data-ttu-id="6d3a5-168">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="6d3a5-168">The more information Url.</span></span> <span data-ttu-id="6d3a5-169">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6d3a5-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6d3a5-170">owner</span><span class="sxs-lookup"><span data-stu-id="6d3a5-170">owner</span></span>|<span data-ttu-id="6d3a5-171">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6d3a5-171">String</span></span>|<span data-ttu-id="6d3a5-172">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="6d3a5-172">The owner of the app.</span></span> <span data-ttu-id="6d3a5-173">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6d3a5-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6d3a5-174">developer</span><span class="sxs-lookup"><span data-stu-id="6d3a5-174">developer</span></span>|<span data-ttu-id="6d3a5-175">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6d3a5-175">String</span></span>|<span data-ttu-id="6d3a5-176">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="6d3a5-176">The developer of the app.</span></span> <span data-ttu-id="6d3a5-177">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6d3a5-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6d3a5-178">notes</span><span class="sxs-lookup"><span data-stu-id="6d3a5-178">notes</span></span>|<span data-ttu-id="6d3a5-179">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6d3a5-179">String</span></span>|<span data-ttu-id="6d3a5-180">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="6d3a5-180">Notes for the app.</span></span> <span data-ttu-id="6d3a5-181">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6d3a5-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6d3a5-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="6d3a5-182">publishingState</span></span>|[<span data-ttu-id="6d3a5-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="6d3a5-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="6d3a5-184">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="6d3a5-184">The publishing state for the app.</span></span> <span data-ttu-id="6d3a5-185">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="6d3a5-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6d3a5-186">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="6d3a5-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="6d3a5-187">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="6d3a5-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="6d3a5-188">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d3a5-188">Response</span></span>
<span data-ttu-id="6d3a5-189">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6d3a5-189">If successful, this method returns a `201 Created` response code and a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d3a5-190">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6d3a5-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d3a5-191">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d3a5-191">Request</span></span>
<span data-ttu-id="6d3a5-192">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6d3a5-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="6d3a5-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d3a5-193">Response</span></span>
<span data-ttu-id="6d3a5-p115">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6d3a5-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



