---
title: Aktualisieren von „macOSOfficeSuiteApp“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs macOSOfficeSuiteApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f2d16ac32245c5d8964e591f251ab88bb2984772
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968266"
---
# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="f05f0-103">Aktualisieren von „macOSOfficeSuiteApp“</span><span class="sxs-lookup"><span data-stu-id="f05f0-103">Update macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="f05f0-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f05f0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f05f0-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f05f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f05f0-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="f05f0-106">Update the properties of a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f05f0-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f05f0-107">Prerequisites</span></span>
<span data-ttu-id="f05f0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f05f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f05f0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f05f0-110">Permission type</span></span>|<span data-ttu-id="f05f0-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f05f0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f05f0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f05f0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f05f0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f05f0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f05f0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f05f0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f05f0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f05f0-115">Not supported.</span></span>|
|<span data-ttu-id="f05f0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f05f0-116">Application</span></span>|<span data-ttu-id="f05f0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f05f0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f05f0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f05f0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="f05f0-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f05f0-119">Request headers</span></span>
|<span data-ttu-id="f05f0-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f05f0-120">Header</span></span>|<span data-ttu-id="f05f0-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f05f0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f05f0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f05f0-122">Authorization</span></span>|<span data-ttu-id="f05f0-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f05f0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f05f0-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f05f0-124">Accept</span></span>|<span data-ttu-id="f05f0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f05f0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f05f0-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f05f0-126">Request body</span></span>
<span data-ttu-id="f05f0-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekt des Typs [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) an.</span><span class="sxs-lookup"><span data-stu-id="f05f0-127">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="f05f0-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="f05f0-128">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="f05f0-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f05f0-129">Property</span></span>|<span data-ttu-id="f05f0-130">Typ</span><span class="sxs-lookup"><span data-stu-id="f05f0-130">Type</span></span>|<span data-ttu-id="f05f0-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f05f0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f05f0-132">id</span><span class="sxs-lookup"><span data-stu-id="f05f0-132">id</span></span>|<span data-ttu-id="f05f0-133">String</span><span class="sxs-lookup"><span data-stu-id="f05f0-133">String</span></span>|<span data-ttu-id="f05f0-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f05f0-134">Key of the entity.</span></span> <span data-ttu-id="f05f0-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f05f0-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f05f0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f05f0-136">displayName</span></span>|<span data-ttu-id="f05f0-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f05f0-137">String</span></span>|<span data-ttu-id="f05f0-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="f05f0-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f05f0-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f05f0-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f05f0-140">description</span><span class="sxs-lookup"><span data-stu-id="f05f0-140">description</span></span>|<span data-ttu-id="f05f0-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f05f0-141">String</span></span>|<span data-ttu-id="f05f0-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="f05f0-142">The description of the app.</span></span> <span data-ttu-id="f05f0-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f05f0-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f05f0-144">publisher</span><span class="sxs-lookup"><span data-stu-id="f05f0-144">publisher</span></span>|<span data-ttu-id="f05f0-145">String</span><span class="sxs-lookup"><span data-stu-id="f05f0-145">String</span></span>|<span data-ttu-id="f05f0-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="f05f0-146">The publisher of the app.</span></span> <span data-ttu-id="f05f0-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f05f0-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f05f0-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f05f0-148">largeIcon</span></span>|[<span data-ttu-id="f05f0-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f05f0-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f05f0-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="f05f0-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f05f0-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f05f0-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f05f0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f05f0-152">createdDateTime</span></span>|<span data-ttu-id="f05f0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f05f0-153">DateTimeOffset</span></span>|<span data-ttu-id="f05f0-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="f05f0-154">The date and time the app was created.</span></span> <span data-ttu-id="f05f0-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f05f0-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f05f0-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f05f0-156">lastModifiedDateTime</span></span>|<span data-ttu-id="f05f0-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f05f0-157">DateTimeOffset</span></span>|<span data-ttu-id="f05f0-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="f05f0-158">The date and time the app was last modified.</span></span> <span data-ttu-id="f05f0-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f05f0-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f05f0-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f05f0-160">isFeatured</span></span>|<span data-ttu-id="f05f0-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="f05f0-161">Boolean</span></span>|<span data-ttu-id="f05f0-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f05f0-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f05f0-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f05f0-163">privacyInformationUrl</span></span>|<span data-ttu-id="f05f0-164">String</span><span class="sxs-lookup"><span data-stu-id="f05f0-164">String</span></span>|<span data-ttu-id="f05f0-165">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="f05f0-165">The privacy statement Url.</span></span> <span data-ttu-id="f05f0-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f05f0-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f05f0-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f05f0-167">informationUrl</span></span>|<span data-ttu-id="f05f0-168">String</span><span class="sxs-lookup"><span data-stu-id="f05f0-168">String</span></span>|<span data-ttu-id="f05f0-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="f05f0-169">The more information Url.</span></span> <span data-ttu-id="f05f0-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f05f0-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f05f0-171">owner</span><span class="sxs-lookup"><span data-stu-id="f05f0-171">owner</span></span>|<span data-ttu-id="f05f0-172">String</span><span class="sxs-lookup"><span data-stu-id="f05f0-172">String</span></span>|<span data-ttu-id="f05f0-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="f05f0-173">The owner of the app.</span></span> <span data-ttu-id="f05f0-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f05f0-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f05f0-175">developer</span><span class="sxs-lookup"><span data-stu-id="f05f0-175">developer</span></span>|<span data-ttu-id="f05f0-176">String</span><span class="sxs-lookup"><span data-stu-id="f05f0-176">String</span></span>|<span data-ttu-id="f05f0-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="f05f0-177">The developer of the app.</span></span> <span data-ttu-id="f05f0-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f05f0-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f05f0-179">notes</span><span class="sxs-lookup"><span data-stu-id="f05f0-179">notes</span></span>|<span data-ttu-id="f05f0-180">String</span><span class="sxs-lookup"><span data-stu-id="f05f0-180">String</span></span>|<span data-ttu-id="f05f0-181">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="f05f0-181">Notes for the app.</span></span> <span data-ttu-id="f05f0-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f05f0-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f05f0-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="f05f0-183">uploadState</span></span>|<span data-ttu-id="f05f0-184">Int32</span><span class="sxs-lookup"><span data-stu-id="f05f0-184">Int32</span></span>|<span data-ttu-id="f05f0-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="f05f0-185">The upload state.</span></span> <span data-ttu-id="f05f0-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f05f0-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f05f0-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="f05f0-187">publishingState</span></span>|[<span data-ttu-id="f05f0-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f05f0-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f05f0-189">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="f05f0-189">The publishing state for the app.</span></span> <span data-ttu-id="f05f0-190">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="f05f0-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f05f0-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="f05f0-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f05f0-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="f05f0-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f05f0-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f05f0-193">isAssigned</span></span>|<span data-ttu-id="f05f0-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="f05f0-194">Boolean</span></span>|<span data-ttu-id="f05f0-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="f05f0-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f05f0-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f05f0-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f05f0-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="f05f0-197">roleScopeTagIds</span></span>|<span data-ttu-id="f05f0-198">String collection</span><span class="sxs-lookup"><span data-stu-id="f05f0-198">String collection</span></span>|<span data-ttu-id="f05f0-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="f05f0-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f05f0-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f05f0-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f05f0-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="f05f0-201">Response</span></span>
<span data-ttu-id="f05f0-202">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f05f0-202">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f05f0-203">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f05f0-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="f05f0-204">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f05f0-204">Request</span></span>
<span data-ttu-id="f05f0-205">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f05f0-205">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 691

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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="f05f0-206">Antwort</span><span class="sxs-lookup"><span data-stu-id="f05f0-206">Response</span></span>
<span data-ttu-id="f05f0-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f05f0-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 863

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
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




