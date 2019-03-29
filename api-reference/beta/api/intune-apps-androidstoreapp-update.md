---
title: androidStoreApp aktualisieren
description: Aktualisieren der Eigenschaften eines androidStoreApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e895082061cac0c572ac9fd240d7eff18f096202
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972452"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="deb8e-103">androidStoreApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="deb8e-103">Update androidStoreApp</span></span>

> <span data-ttu-id="deb8e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="deb8e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="deb8e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="deb8e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="deb8e-106">Aktualisieren der Eigenschaften eines [androidStoreApp](../resources/intune-apps-androidstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="deb8e-106">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="deb8e-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="deb8e-107">Prerequisites</span></span>
<span data-ttu-id="deb8e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="deb8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="deb8e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="deb8e-110">Permission type</span></span>|<span data-ttu-id="deb8e-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="deb8e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="deb8e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="deb8e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="deb8e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deb8e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="deb8e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="deb8e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="deb8e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="deb8e-115">Not supported.</span></span>|
|<span data-ttu-id="deb8e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="deb8e-116">Application</span></span>|<span data-ttu-id="deb8e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="deb8e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="deb8e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="deb8e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="deb8e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="deb8e-119">Request headers</span></span>
|<span data-ttu-id="deb8e-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="deb8e-120">Header</span></span>|<span data-ttu-id="deb8e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="deb8e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="deb8e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="deb8e-122">Authorization</span></span>|<span data-ttu-id="deb8e-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="deb8e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="deb8e-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="deb8e-124">Accept</span></span>|<span data-ttu-id="deb8e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="deb8e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="deb8e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="deb8e-126">Request body</span></span>
<span data-ttu-id="deb8e-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [androidStoreApp](../resources/intune-apps-androidstoreapp.md) an.</span><span class="sxs-lookup"><span data-stu-id="deb8e-127">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="deb8e-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [androidStoreApp](../resources/intune-apps-androidstoreapp.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="deb8e-128">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="deb8e-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="deb8e-129">Property</span></span>|<span data-ttu-id="deb8e-130">Typ</span><span class="sxs-lookup"><span data-stu-id="deb8e-130">Type</span></span>|<span data-ttu-id="deb8e-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="deb8e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="deb8e-132">id</span><span class="sxs-lookup"><span data-stu-id="deb8e-132">id</span></span>|<span data-ttu-id="deb8e-133">String</span><span class="sxs-lookup"><span data-stu-id="deb8e-133">String</span></span>|<span data-ttu-id="deb8e-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="deb8e-134">Key of the entity.</span></span> <span data-ttu-id="deb8e-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="deb8e-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="deb8e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="deb8e-136">displayName</span></span>|<span data-ttu-id="deb8e-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="deb8e-137">String</span></span>|<span data-ttu-id="deb8e-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="deb8e-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="deb8e-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="deb8e-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="deb8e-140">description</span><span class="sxs-lookup"><span data-stu-id="deb8e-140">description</span></span>|<span data-ttu-id="deb8e-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="deb8e-141">String</span></span>|<span data-ttu-id="deb8e-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="deb8e-142">The description of the app.</span></span> <span data-ttu-id="deb8e-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="deb8e-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="deb8e-144">publisher</span><span class="sxs-lookup"><span data-stu-id="deb8e-144">publisher</span></span>|<span data-ttu-id="deb8e-145">String</span><span class="sxs-lookup"><span data-stu-id="deb8e-145">String</span></span>|<span data-ttu-id="deb8e-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="deb8e-146">The publisher of the app.</span></span> <span data-ttu-id="deb8e-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="deb8e-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="deb8e-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="deb8e-148">largeIcon</span></span>|[<span data-ttu-id="deb8e-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="deb8e-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="deb8e-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="deb8e-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="deb8e-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="deb8e-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="deb8e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="deb8e-152">createdDateTime</span></span>|<span data-ttu-id="deb8e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="deb8e-153">DateTimeOffset</span></span>|<span data-ttu-id="deb8e-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="deb8e-154">The date and time the app was created.</span></span> <span data-ttu-id="deb8e-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="deb8e-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="deb8e-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="deb8e-156">lastModifiedDateTime</span></span>|<span data-ttu-id="deb8e-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="deb8e-157">DateTimeOffset</span></span>|<span data-ttu-id="deb8e-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="deb8e-158">The date and time the app was last modified.</span></span> <span data-ttu-id="deb8e-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="deb8e-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="deb8e-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="deb8e-160">isFeatured</span></span>|<span data-ttu-id="deb8e-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="deb8e-161">Boolean</span></span>|<span data-ttu-id="deb8e-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="deb8e-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="deb8e-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="deb8e-163">privacyInformationUrl</span></span>|<span data-ttu-id="deb8e-164">String</span><span class="sxs-lookup"><span data-stu-id="deb8e-164">String</span></span>|<span data-ttu-id="deb8e-165">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="deb8e-165">The privacy statement Url.</span></span> <span data-ttu-id="deb8e-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="deb8e-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="deb8e-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="deb8e-167">informationUrl</span></span>|<span data-ttu-id="deb8e-168">String</span><span class="sxs-lookup"><span data-stu-id="deb8e-168">String</span></span>|<span data-ttu-id="deb8e-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="deb8e-169">The more information Url.</span></span> <span data-ttu-id="deb8e-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="deb8e-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="deb8e-171">owner</span><span class="sxs-lookup"><span data-stu-id="deb8e-171">owner</span></span>|<span data-ttu-id="deb8e-172">String</span><span class="sxs-lookup"><span data-stu-id="deb8e-172">String</span></span>|<span data-ttu-id="deb8e-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="deb8e-173">The owner of the app.</span></span> <span data-ttu-id="deb8e-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="deb8e-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="deb8e-175">developer</span><span class="sxs-lookup"><span data-stu-id="deb8e-175">developer</span></span>|<span data-ttu-id="deb8e-176">String</span><span class="sxs-lookup"><span data-stu-id="deb8e-176">String</span></span>|<span data-ttu-id="deb8e-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="deb8e-177">The developer of the app.</span></span> <span data-ttu-id="deb8e-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="deb8e-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="deb8e-179">notes</span><span class="sxs-lookup"><span data-stu-id="deb8e-179">notes</span></span>|<span data-ttu-id="deb8e-180">String</span><span class="sxs-lookup"><span data-stu-id="deb8e-180">String</span></span>|<span data-ttu-id="deb8e-181">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="deb8e-181">Notes for the app.</span></span> <span data-ttu-id="deb8e-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="deb8e-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="deb8e-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="deb8e-183">uploadState</span></span>|<span data-ttu-id="deb8e-184">Int32</span><span class="sxs-lookup"><span data-stu-id="deb8e-184">Int32</span></span>|<span data-ttu-id="deb8e-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="deb8e-185">The upload state.</span></span> <span data-ttu-id="deb8e-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="deb8e-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="deb8e-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="deb8e-187">publishingState</span></span>|[<span data-ttu-id="deb8e-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="deb8e-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="deb8e-189">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="deb8e-189">The publishing state for the app.</span></span> <span data-ttu-id="deb8e-190">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="deb8e-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="deb8e-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="deb8e-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="deb8e-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="deb8e-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="deb8e-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="deb8e-193">isAssigned</span></span>|<span data-ttu-id="deb8e-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="deb8e-194">Boolean</span></span>|<span data-ttu-id="deb8e-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="deb8e-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="deb8e-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="deb8e-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="deb8e-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="deb8e-197">roleScopeTagIds</span></span>|<span data-ttu-id="deb8e-198">String collection</span><span class="sxs-lookup"><span data-stu-id="deb8e-198">String collection</span></span>|<span data-ttu-id="deb8e-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="deb8e-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="deb8e-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="deb8e-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="deb8e-201">packageId</span><span class="sxs-lookup"><span data-stu-id="deb8e-201">packageId</span></span>|<span data-ttu-id="deb8e-202">String</span><span class="sxs-lookup"><span data-stu-id="deb8e-202">String</span></span>|<span data-ttu-id="deb8e-203">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="deb8e-203">The package identifier.</span></span>|
|<span data-ttu-id="deb8e-204">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="deb8e-204">appIdentifier</span></span>|<span data-ttu-id="deb8e-205">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="deb8e-205">String</span></span>|<span data-ttu-id="deb8e-206">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="deb8e-206">The Identity Name.</span></span>|
|<span data-ttu-id="deb8e-207">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="deb8e-207">appStoreUrl</span></span>|<span data-ttu-id="deb8e-208">String</span><span class="sxs-lookup"><span data-stu-id="deb8e-208">String</span></span>|<span data-ttu-id="deb8e-209">URL zum App-Store von Android</span><span class="sxs-lookup"><span data-stu-id="deb8e-209">The Android app store URL.</span></span>|
|<span data-ttu-id="deb8e-210">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="deb8e-210">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="deb8e-211">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="deb8e-211">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="deb8e-212">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="deb8e-212">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="deb8e-213">Antwort</span><span class="sxs-lookup"><span data-stu-id="deb8e-213">Response</span></span>
<span data-ttu-id="deb8e-214">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [androidStoreApp](../resources/intune-apps-androidstoreapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="deb8e-214">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="deb8e-215">Beispiel</span><span class="sxs-lookup"><span data-stu-id="deb8e-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="deb8e-216">Anforderung</span><span class="sxs-lookup"><span data-stu-id="deb8e-216">Request</span></span>
<span data-ttu-id="deb8e-217">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="deb8e-217">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1203

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="deb8e-218">Antwort</span><span class="sxs-lookup"><span data-stu-id="deb8e-218">Response</span></span>
<span data-ttu-id="deb8e-p118">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="deb8e-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1375

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```




