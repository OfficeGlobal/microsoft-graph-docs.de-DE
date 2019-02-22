---
title: AndroidManagedStoreApp aktualisieren
description: Aktualisieren der Eigenschaften eines androidManagedStoreApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4e050d8f7bb834224076a0f7fb7b84812ee8a3c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156658"
---
# <a name="update-androidmanagedstoreapp"></a><span data-ttu-id="c8456-103">AndroidManagedStoreApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c8456-103">Update androidManagedStoreApp</span></span>

> <span data-ttu-id="c8456-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c8456-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8456-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c8456-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8456-106">Aktualisieren der Eigenschaften eines [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c8456-106">Update the properties of a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8456-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c8456-107">Prerequisites</span></span>
<span data-ttu-id="c8456-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c8456-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c8456-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c8456-110">Permission type</span></span>|<span data-ttu-id="c8456-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c8456-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8456-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c8456-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c8456-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8456-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c8456-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c8456-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8456-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8456-115">Not supported.</span></span>|
|<span data-ttu-id="c8456-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c8456-116">Application</span></span>|<span data-ttu-id="c8456-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8456-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8456-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8456-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="c8456-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c8456-119">Request headers</span></span>
|<span data-ttu-id="c8456-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c8456-120">Header</span></span>|<span data-ttu-id="c8456-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c8456-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8456-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8456-122">Authorization</span></span>|<span data-ttu-id="c8456-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c8456-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8456-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c8456-124">Accept</span></span>|<span data-ttu-id="c8456-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c8456-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8456-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c8456-126">Request body</span></span>
<span data-ttu-id="c8456-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="c8456-127">In the request body, supply a JSON representation for the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

<span data-ttu-id="c8456-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c8456-128">The following table shows the properties that are required when you create the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md).</span></span>

|<span data-ttu-id="c8456-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c8456-129">Property</span></span>|<span data-ttu-id="c8456-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c8456-130">Type</span></span>|<span data-ttu-id="c8456-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c8456-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8456-132">id</span><span class="sxs-lookup"><span data-stu-id="c8456-132">id</span></span>|<span data-ttu-id="c8456-133">string</span><span class="sxs-lookup"><span data-stu-id="c8456-133">String</span></span>|<span data-ttu-id="c8456-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c8456-134">Key of the entity.</span></span> <span data-ttu-id="c8456-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c8456-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8456-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c8456-136">displayName</span></span>|<span data-ttu-id="c8456-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8456-137">String</span></span>|<span data-ttu-id="c8456-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="c8456-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c8456-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c8456-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8456-140">description</span><span class="sxs-lookup"><span data-stu-id="c8456-140">description</span></span>|<span data-ttu-id="c8456-141">String</span><span class="sxs-lookup"><span data-stu-id="c8456-141">String</span></span>|<span data-ttu-id="c8456-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="c8456-142">The description of the app.</span></span> <span data-ttu-id="c8456-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c8456-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8456-144">publisher</span><span class="sxs-lookup"><span data-stu-id="c8456-144">publisher</span></span>|<span data-ttu-id="c8456-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8456-145">String</span></span>|<span data-ttu-id="c8456-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="c8456-146">The publisher of the app.</span></span> <span data-ttu-id="c8456-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c8456-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8456-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c8456-148">largeIcon</span></span>|[<span data-ttu-id="c8456-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c8456-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c8456-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="c8456-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c8456-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c8456-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8456-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c8456-152">createdDateTime</span></span>|<span data-ttu-id="c8456-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8456-153">DateTimeOffset</span></span>|<span data-ttu-id="c8456-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="c8456-154">The date and time the app was created.</span></span> <span data-ttu-id="c8456-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c8456-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8456-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8456-156">lastModifiedDateTime</span></span>|<span data-ttu-id="c8456-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8456-157">DateTimeOffset</span></span>|<span data-ttu-id="c8456-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="c8456-158">The date and time the app was last modified.</span></span> <span data-ttu-id="c8456-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c8456-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8456-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c8456-160">isFeatured</span></span>|<span data-ttu-id="c8456-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c8456-161">Boolean</span></span>|<span data-ttu-id="c8456-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c8456-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8456-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c8456-163">privacyInformationUrl</span></span>|<span data-ttu-id="c8456-164">String</span><span class="sxs-lookup"><span data-stu-id="c8456-164">String</span></span>|<span data-ttu-id="c8456-165">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="c8456-165">The privacy statement Url.</span></span> <span data-ttu-id="c8456-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c8456-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8456-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c8456-167">informationUrl</span></span>|<span data-ttu-id="c8456-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8456-168">String</span></span>|<span data-ttu-id="c8456-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="c8456-169">The more information Url.</span></span> <span data-ttu-id="c8456-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c8456-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8456-171">owner</span><span class="sxs-lookup"><span data-stu-id="c8456-171">owner</span></span>|<span data-ttu-id="c8456-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8456-172">String</span></span>|<span data-ttu-id="c8456-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="c8456-173">The owner of the app.</span></span> <span data-ttu-id="c8456-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c8456-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8456-175">developer</span><span class="sxs-lookup"><span data-stu-id="c8456-175">developer</span></span>|<span data-ttu-id="c8456-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8456-176">String</span></span>|<span data-ttu-id="c8456-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="c8456-177">The developer of the app.</span></span> <span data-ttu-id="c8456-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c8456-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8456-179">notes</span><span class="sxs-lookup"><span data-stu-id="c8456-179">notes</span></span>|<span data-ttu-id="c8456-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8456-180">String</span></span>|<span data-ttu-id="c8456-181">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="c8456-181">Notes for the app.</span></span> <span data-ttu-id="c8456-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c8456-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8456-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="c8456-183">uploadState</span></span>|<span data-ttu-id="c8456-184">Int32</span><span class="sxs-lookup"><span data-stu-id="c8456-184">Int32</span></span>|<span data-ttu-id="c8456-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="c8456-185">The upload state.</span></span> <span data-ttu-id="c8456-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c8456-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8456-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="c8456-187">publishingState</span></span>|[<span data-ttu-id="c8456-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c8456-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c8456-189">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="c8456-189">The publishing state for the app.</span></span> <span data-ttu-id="c8456-190">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="c8456-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c8456-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="c8456-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c8456-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="c8456-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c8456-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c8456-193">isAssigned</span></span>|<span data-ttu-id="c8456-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8456-194">Boolean</span></span>|<span data-ttu-id="c8456-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="c8456-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="c8456-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c8456-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8456-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="c8456-197">roleScopeTagIds</span></span>|<span data-ttu-id="c8456-198">String collection</span><span class="sxs-lookup"><span data-stu-id="c8456-198">String collection</span></span>|<span data-ttu-id="c8456-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="c8456-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="c8456-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c8456-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c8456-201">packageId</span><span class="sxs-lookup"><span data-stu-id="c8456-201">packageId</span></span>|<span data-ttu-id="c8456-202">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8456-202">String</span></span>|<span data-ttu-id="c8456-203">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="c8456-203">The package identifier.</span></span>|
|<span data-ttu-id="c8456-204">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="c8456-204">appIdentifier</span></span>|<span data-ttu-id="c8456-205">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8456-205">String</span></span>|<span data-ttu-id="c8456-206">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="c8456-206">The Identity Name.</span></span>|
|<span data-ttu-id="c8456-207">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="c8456-207">usedLicenseCount</span></span>|<span data-ttu-id="c8456-208">Int32</span><span class="sxs-lookup"><span data-stu-id="c8456-208">Int32</span></span>|<span data-ttu-id="c8456-209">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="c8456-209">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="c8456-210">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="c8456-210">totalLicenseCount</span></span>|<span data-ttu-id="c8456-211">Int32</span><span class="sxs-lookup"><span data-stu-id="c8456-211">Int32</span></span>|<span data-ttu-id="c8456-212">Gesamtanzahl von VPP-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="c8456-212">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="c8456-213">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="c8456-213">appStoreUrl</span></span>|<span data-ttu-id="c8456-214">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c8456-214">String</span></span>|<span data-ttu-id="c8456-215">Die App-URL für die Wiedergabe für Arbeitsspeicher.</span><span class="sxs-lookup"><span data-stu-id="c8456-215">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="c8456-216">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8456-216">Response</span></span>
<span data-ttu-id="c8456-217">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c8456-217">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8456-218">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c8456-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8456-219">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8456-219">Request</span></span>
<span data-ttu-id="c8456-220">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c8456-220">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 881

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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="c8456-221">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8456-221">Response</span></span>
<span data-ttu-id="c8456-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8456-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1053

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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```




