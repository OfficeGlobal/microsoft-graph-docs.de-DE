---
title: microsoftStoreForBusinessApp aktualisieren
description: Aktualisieren der Eigenschaften eines microsoftStoreForBusinessApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f206898bc37d16dfb987a3b91aa8d2a660c0209
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30963912"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="216c4-103">microsoftStoreForBusinessApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="216c4-103">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="216c4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="216c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="216c4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="216c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="216c4-106">Aktualisieren der Eigenschaften eines [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="216c4-106">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="216c4-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="216c4-107">Prerequisites</span></span>
<span data-ttu-id="216c4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="216c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="216c4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="216c4-110">Permission type</span></span>|<span data-ttu-id="216c4-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="216c4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="216c4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="216c4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="216c4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="216c4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="216c4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="216c4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="216c4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="216c4-115">Not supported.</span></span>|
|<span data-ttu-id="216c4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="216c4-116">Application</span></span>|<span data-ttu-id="216c4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="216c4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="216c4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="216c4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="216c4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="216c4-119">Request headers</span></span>
|<span data-ttu-id="216c4-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="216c4-120">Header</span></span>|<span data-ttu-id="216c4-121">Wert</span><span class="sxs-lookup"><span data-stu-id="216c4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="216c4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="216c4-122">Authorization</span></span>|<span data-ttu-id="216c4-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="216c4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="216c4-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="216c4-124">Accept</span></span>|<span data-ttu-id="216c4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="216c4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="216c4-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="216c4-126">Request body</span></span>
<span data-ttu-id="216c4-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="216c4-127">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="216c4-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="216c4-128">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="216c4-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="216c4-129">Property</span></span>|<span data-ttu-id="216c4-130">Typ</span><span class="sxs-lookup"><span data-stu-id="216c4-130">Type</span></span>|<span data-ttu-id="216c4-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="216c4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="216c4-132">id</span><span class="sxs-lookup"><span data-stu-id="216c4-132">id</span></span>|<span data-ttu-id="216c4-133">String</span><span class="sxs-lookup"><span data-stu-id="216c4-133">String</span></span>|<span data-ttu-id="216c4-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="216c4-134">Key of the entity.</span></span> <span data-ttu-id="216c4-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="216c4-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="216c4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="216c4-136">displayName</span></span>|<span data-ttu-id="216c4-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="216c4-137">String</span></span>|<span data-ttu-id="216c4-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="216c4-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="216c4-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="216c4-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="216c4-140">description</span><span class="sxs-lookup"><span data-stu-id="216c4-140">description</span></span>|<span data-ttu-id="216c4-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="216c4-141">String</span></span>|<span data-ttu-id="216c4-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="216c4-142">The description of the app.</span></span> <span data-ttu-id="216c4-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="216c4-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="216c4-144">publisher</span><span class="sxs-lookup"><span data-stu-id="216c4-144">publisher</span></span>|<span data-ttu-id="216c4-145">String</span><span class="sxs-lookup"><span data-stu-id="216c4-145">String</span></span>|<span data-ttu-id="216c4-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="216c4-146">The publisher of the app.</span></span> <span data-ttu-id="216c4-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="216c4-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="216c4-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="216c4-148">largeIcon</span></span>|[<span data-ttu-id="216c4-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="216c4-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="216c4-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="216c4-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="216c4-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="216c4-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="216c4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="216c4-152">createdDateTime</span></span>|<span data-ttu-id="216c4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="216c4-153">DateTimeOffset</span></span>|<span data-ttu-id="216c4-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="216c4-154">The date and time the app was created.</span></span> <span data-ttu-id="216c4-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="216c4-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="216c4-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="216c4-156">lastModifiedDateTime</span></span>|<span data-ttu-id="216c4-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="216c4-157">DateTimeOffset</span></span>|<span data-ttu-id="216c4-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="216c4-158">The date and time the app was last modified.</span></span> <span data-ttu-id="216c4-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="216c4-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="216c4-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="216c4-160">isFeatured</span></span>|<span data-ttu-id="216c4-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="216c4-161">Boolean</span></span>|<span data-ttu-id="216c4-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="216c4-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="216c4-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="216c4-163">privacyInformationUrl</span></span>|<span data-ttu-id="216c4-164">String</span><span class="sxs-lookup"><span data-stu-id="216c4-164">String</span></span>|<span data-ttu-id="216c4-165">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="216c4-165">The privacy statement Url.</span></span> <span data-ttu-id="216c4-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="216c4-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="216c4-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="216c4-167">informationUrl</span></span>|<span data-ttu-id="216c4-168">String</span><span class="sxs-lookup"><span data-stu-id="216c4-168">String</span></span>|<span data-ttu-id="216c4-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="216c4-169">The more information Url.</span></span> <span data-ttu-id="216c4-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="216c4-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="216c4-171">owner</span><span class="sxs-lookup"><span data-stu-id="216c4-171">owner</span></span>|<span data-ttu-id="216c4-172">String</span><span class="sxs-lookup"><span data-stu-id="216c4-172">String</span></span>|<span data-ttu-id="216c4-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="216c4-173">The owner of the app.</span></span> <span data-ttu-id="216c4-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="216c4-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="216c4-175">developer</span><span class="sxs-lookup"><span data-stu-id="216c4-175">developer</span></span>|<span data-ttu-id="216c4-176">String</span><span class="sxs-lookup"><span data-stu-id="216c4-176">String</span></span>|<span data-ttu-id="216c4-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="216c4-177">The developer of the app.</span></span> <span data-ttu-id="216c4-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="216c4-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="216c4-179">notes</span><span class="sxs-lookup"><span data-stu-id="216c4-179">notes</span></span>|<span data-ttu-id="216c4-180">String</span><span class="sxs-lookup"><span data-stu-id="216c4-180">String</span></span>|<span data-ttu-id="216c4-181">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="216c4-181">Notes for the app.</span></span> <span data-ttu-id="216c4-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="216c4-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="216c4-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="216c4-183">uploadState</span></span>|<span data-ttu-id="216c4-184">Int32</span><span class="sxs-lookup"><span data-stu-id="216c4-184">Int32</span></span>|<span data-ttu-id="216c4-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="216c4-185">The upload state.</span></span> <span data-ttu-id="216c4-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="216c4-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="216c4-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="216c4-187">publishingState</span></span>|[<span data-ttu-id="216c4-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="216c4-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="216c4-189">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="216c4-189">The publishing state for the app.</span></span> <span data-ttu-id="216c4-190">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="216c4-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="216c4-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="216c4-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="216c4-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="216c4-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="216c4-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="216c4-193">isAssigned</span></span>|<span data-ttu-id="216c4-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="216c4-194">Boolean</span></span>|<span data-ttu-id="216c4-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="216c4-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="216c4-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="216c4-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="216c4-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="216c4-197">roleScopeTagIds</span></span>|<span data-ttu-id="216c4-198">String collection</span><span class="sxs-lookup"><span data-stu-id="216c4-198">String collection</span></span>|<span data-ttu-id="216c4-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="216c4-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="216c4-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="216c4-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="216c4-201">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="216c4-201">usedLicenseCount</span></span>|<span data-ttu-id="216c4-202">Int32</span><span class="sxs-lookup"><span data-stu-id="216c4-202">Int32</span></span>|<span data-ttu-id="216c4-203">Die Anzahl von verwendeten Microsoft Store für Unternehmen-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="216c4-203">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="216c4-204">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="216c4-204">totalLicenseCount</span></span>|<span data-ttu-id="216c4-205">Int32</span><span class="sxs-lookup"><span data-stu-id="216c4-205">Int32</span></span>|<span data-ttu-id="216c4-206">Die Gesamtzahl der Microsoft Store für Unternehmen-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="216c4-206">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="216c4-207">productKey</span><span class="sxs-lookup"><span data-stu-id="216c4-207">productKey</span></span>|<span data-ttu-id="216c4-208">String</span><span class="sxs-lookup"><span data-stu-id="216c4-208">String</span></span>|<span data-ttu-id="216c4-209">Der Product Key der App</span><span class="sxs-lookup"><span data-stu-id="216c4-209">The app product key</span></span>|
|<span data-ttu-id="216c4-210">licenseType</span><span class="sxs-lookup"><span data-stu-id="216c4-210">licenseType</span></span>|[<span data-ttu-id="216c4-211">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="216c4-211">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="216c4-212">Der APP-Lizenztyp.</span><span class="sxs-lookup"><span data-stu-id="216c4-212">The app license type.</span></span> <span data-ttu-id="216c4-213">Mögliche Werte sind: `offline` und `online`.</span><span class="sxs-lookup"><span data-stu-id="216c4-213">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="216c4-214">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="216c4-214">packageIdentityName</span></span>|<span data-ttu-id="216c4-215">String</span><span class="sxs-lookup"><span data-stu-id="216c4-215">String</span></span>|<span data-ttu-id="216c4-216">Bezeichner des App-Pakets</span><span class="sxs-lookup"><span data-stu-id="216c4-216">The app package identifier</span></span>|
|<span data-ttu-id="216c4-217">licensingType</span><span class="sxs-lookup"><span data-stu-id="216c4-217">licensingType</span></span>|[<span data-ttu-id="216c4-218">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="216c4-218">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="216c4-219">Unterstützter Lizenztyp</span><span class="sxs-lookup"><span data-stu-id="216c4-219">The supported License Type.</span></span>|



## <a name="response"></a><span data-ttu-id="216c4-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="216c4-220">Response</span></span>
<span data-ttu-id="216c4-221">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="216c4-221">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="216c4-222">Beispiel</span><span class="sxs-lookup"><span data-stu-id="216c4-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="216c4-223">Anforderung</span><span class="sxs-lookup"><span data-stu-id="216c4-223">Request</span></span>
<span data-ttu-id="216c4-224">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="216c4-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1105

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  }
}
```

### <a name="response"></a><span data-ttu-id="216c4-225">Antwort</span><span class="sxs-lookup"><span data-stu-id="216c4-225">Response</span></span>
<span data-ttu-id="216c4-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="216c4-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1277

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  }
}
```




