---
title: AndroidManagedStoreApp aktualisieren
description: Aktualisieren der Eigenschaften eines androidManagedStoreApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1558994f71fbf62f7d401b64a61d687e39c8215a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964829"
---
# <a name="update-androidmanagedstoreapp"></a><span data-ttu-id="00527-103">AndroidManagedStoreApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="00527-103">Update androidManagedStoreApp</span></span>

> <span data-ttu-id="00527-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="00527-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00527-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="00527-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00527-106">Aktualisieren der Eigenschaften eines [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="00527-106">Update the properties of a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00527-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="00527-107">Prerequisites</span></span>
<span data-ttu-id="00527-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00527-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00527-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="00527-110">Permission type</span></span>|<span data-ttu-id="00527-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="00527-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00527-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="00527-112">Delegated (work or school account)</span></span>|<span data-ttu-id="00527-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00527-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="00527-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="00527-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00527-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="00527-115">Not supported.</span></span>|
|<span data-ttu-id="00527-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="00527-116">Application</span></span>|<span data-ttu-id="00527-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="00527-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00527-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="00527-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="00527-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="00527-119">Request headers</span></span>
|<span data-ttu-id="00527-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="00527-120">Header</span></span>|<span data-ttu-id="00527-121">Wert</span><span class="sxs-lookup"><span data-stu-id="00527-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00527-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="00527-122">Authorization</span></span>|<span data-ttu-id="00527-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="00527-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00527-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="00527-124">Accept</span></span>|<span data-ttu-id="00527-125">application/json</span><span class="sxs-lookup"><span data-stu-id="00527-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00527-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="00527-126">Request body</span></span>
<span data-ttu-id="00527-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="00527-127">In the request body, supply a JSON representation for the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

<span data-ttu-id="00527-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="00527-128">The following table shows the properties that are required when you create the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md).</span></span>

|<span data-ttu-id="00527-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="00527-129">Property</span></span>|<span data-ttu-id="00527-130">Typ</span><span class="sxs-lookup"><span data-stu-id="00527-130">Type</span></span>|<span data-ttu-id="00527-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00527-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00527-132">id</span><span class="sxs-lookup"><span data-stu-id="00527-132">id</span></span>|<span data-ttu-id="00527-133">String</span><span class="sxs-lookup"><span data-stu-id="00527-133">String</span></span>|<span data-ttu-id="00527-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="00527-134">Key of the entity.</span></span> <span data-ttu-id="00527-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00527-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00527-136">displayName</span><span class="sxs-lookup"><span data-stu-id="00527-136">displayName</span></span>|<span data-ttu-id="00527-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00527-137">String</span></span>|<span data-ttu-id="00527-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="00527-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="00527-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00527-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00527-140">description</span><span class="sxs-lookup"><span data-stu-id="00527-140">description</span></span>|<span data-ttu-id="00527-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00527-141">String</span></span>|<span data-ttu-id="00527-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="00527-142">The description of the app.</span></span> <span data-ttu-id="00527-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00527-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00527-144">publisher</span><span class="sxs-lookup"><span data-stu-id="00527-144">publisher</span></span>|<span data-ttu-id="00527-145">String</span><span class="sxs-lookup"><span data-stu-id="00527-145">String</span></span>|<span data-ttu-id="00527-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="00527-146">The publisher of the app.</span></span> <span data-ttu-id="00527-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00527-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00527-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="00527-148">largeIcon</span></span>|[<span data-ttu-id="00527-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="00527-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="00527-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="00527-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="00527-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00527-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00527-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="00527-152">createdDateTime</span></span>|<span data-ttu-id="00527-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00527-153">DateTimeOffset</span></span>|<span data-ttu-id="00527-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="00527-154">The date and time the app was created.</span></span> <span data-ttu-id="00527-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00527-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00527-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="00527-156">lastModifiedDateTime</span></span>|<span data-ttu-id="00527-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00527-157">DateTimeOffset</span></span>|<span data-ttu-id="00527-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="00527-158">The date and time the app was last modified.</span></span> <span data-ttu-id="00527-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00527-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00527-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="00527-160">isFeatured</span></span>|<span data-ttu-id="00527-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="00527-161">Boolean</span></span>|<span data-ttu-id="00527-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00527-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00527-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="00527-163">privacyInformationUrl</span></span>|<span data-ttu-id="00527-164">String</span><span class="sxs-lookup"><span data-stu-id="00527-164">String</span></span>|<span data-ttu-id="00527-165">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="00527-165">The privacy statement Url.</span></span> <span data-ttu-id="00527-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00527-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00527-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="00527-167">informationUrl</span></span>|<span data-ttu-id="00527-168">String</span><span class="sxs-lookup"><span data-stu-id="00527-168">String</span></span>|<span data-ttu-id="00527-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="00527-169">The more information Url.</span></span> <span data-ttu-id="00527-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00527-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00527-171">owner</span><span class="sxs-lookup"><span data-stu-id="00527-171">owner</span></span>|<span data-ttu-id="00527-172">String</span><span class="sxs-lookup"><span data-stu-id="00527-172">String</span></span>|<span data-ttu-id="00527-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="00527-173">The owner of the app.</span></span> <span data-ttu-id="00527-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00527-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00527-175">developer</span><span class="sxs-lookup"><span data-stu-id="00527-175">developer</span></span>|<span data-ttu-id="00527-176">String</span><span class="sxs-lookup"><span data-stu-id="00527-176">String</span></span>|<span data-ttu-id="00527-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="00527-177">The developer of the app.</span></span> <span data-ttu-id="00527-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00527-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00527-179">notes</span><span class="sxs-lookup"><span data-stu-id="00527-179">notes</span></span>|<span data-ttu-id="00527-180">String</span><span class="sxs-lookup"><span data-stu-id="00527-180">String</span></span>|<span data-ttu-id="00527-181">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="00527-181">Notes for the app.</span></span> <span data-ttu-id="00527-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00527-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00527-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="00527-183">uploadState</span></span>|<span data-ttu-id="00527-184">Int32</span><span class="sxs-lookup"><span data-stu-id="00527-184">Int32</span></span>|<span data-ttu-id="00527-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="00527-185">The upload state.</span></span> <span data-ttu-id="00527-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00527-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00527-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="00527-187">publishingState</span></span>|[<span data-ttu-id="00527-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="00527-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="00527-189">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="00527-189">The publishing state for the app.</span></span> <span data-ttu-id="00527-190">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="00527-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="00527-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="00527-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="00527-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="00527-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="00527-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="00527-193">isAssigned</span></span>|<span data-ttu-id="00527-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="00527-194">Boolean</span></span>|<span data-ttu-id="00527-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="00527-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="00527-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00527-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00527-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="00527-197">roleScopeTagIds</span></span>|<span data-ttu-id="00527-198">String collection</span><span class="sxs-lookup"><span data-stu-id="00527-198">String collection</span></span>|<span data-ttu-id="00527-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="00527-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="00527-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00527-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00527-201">packageId</span><span class="sxs-lookup"><span data-stu-id="00527-201">packageId</span></span>|<span data-ttu-id="00527-202">String</span><span class="sxs-lookup"><span data-stu-id="00527-202">String</span></span>|<span data-ttu-id="00527-203">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="00527-203">The package identifier.</span></span>|
|<span data-ttu-id="00527-204">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="00527-204">appIdentifier</span></span>|<span data-ttu-id="00527-205">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="00527-205">String</span></span>|<span data-ttu-id="00527-206">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="00527-206">The Identity Name.</span></span>|
|<span data-ttu-id="00527-207">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="00527-207">usedLicenseCount</span></span>|<span data-ttu-id="00527-208">Int32</span><span class="sxs-lookup"><span data-stu-id="00527-208">Int32</span></span>|<span data-ttu-id="00527-209">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="00527-209">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="00527-210">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="00527-210">totalLicenseCount</span></span>|<span data-ttu-id="00527-211">Int32</span><span class="sxs-lookup"><span data-stu-id="00527-211">Int32</span></span>|<span data-ttu-id="00527-212">Gesamtanzahl von VPP-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="00527-212">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="00527-213">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="00527-213">appStoreUrl</span></span>|<span data-ttu-id="00527-214">String</span><span class="sxs-lookup"><span data-stu-id="00527-214">String</span></span>|<span data-ttu-id="00527-215">Die App-URL für die Wiedergabe für Arbeitsspeicher.</span><span class="sxs-lookup"><span data-stu-id="00527-215">The Play for Work Store app URL.</span></span>|
|<span data-ttu-id="00527-216">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="00527-216">supportsOemConfig</span></span>|<span data-ttu-id="00527-217">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="00527-217">Boolean</span></span>|<span data-ttu-id="00527-218">Ob diese APP die OEMConfig-Richtlinie unterstützt.</span><span class="sxs-lookup"><span data-stu-id="00527-218">Whether this app supports OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="00527-219">Antwort</span><span class="sxs-lookup"><span data-stu-id="00527-219">Response</span></span>
<span data-ttu-id="00527-220">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="00527-220">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00527-221">Beispiel</span><span class="sxs-lookup"><span data-stu-id="00527-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="00527-222">Anforderung</span><span class="sxs-lookup"><span data-stu-id="00527-222">Request</span></span>
<span data-ttu-id="00527-223">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="00527-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 911

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
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
  ],
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="00527-224">Antwort</span><span class="sxs-lookup"><span data-stu-id="00527-224">Response</span></span>
<span data-ttu-id="00527-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="00527-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1083

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
  "id": "87247525-7525-8724-2575-248725752487",
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
  ],
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "supportsOemConfig": true
}
```




