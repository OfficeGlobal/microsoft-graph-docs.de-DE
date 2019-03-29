---
title: Erstellen von „iosVppApp“
description: Erstellen eines neuen iosVppApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20ed922851ae7e19138cc868e2b1ce2aed6c9aed
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978983"
---
# <a name="create-iosvppapp"></a><span data-ttu-id="76db7-103">Erstellen von „iosVppApp“</span><span class="sxs-lookup"><span data-stu-id="76db7-103">Create iosVppApp</span></span>

> <span data-ttu-id="76db7-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="76db7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76db7-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="76db7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76db7-106">Erstellen eines neuen [iosVppApp](../resources/intune-apps-iosvppapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="76db7-106">Create a new [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76db7-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="76db7-107">Prerequisites</span></span>
<span data-ttu-id="76db7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76db7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76db7-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="76db7-110">Permission type</span></span>|<span data-ttu-id="76db7-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="76db7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76db7-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="76db7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="76db7-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76db7-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="76db7-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="76db7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76db7-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="76db7-115">Not supported.</span></span>|
|<span data-ttu-id="76db7-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="76db7-116">Application</span></span>|<span data-ttu-id="76db7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="76db7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76db7-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="76db7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="76db7-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="76db7-119">Request headers</span></span>
|<span data-ttu-id="76db7-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="76db7-120">Header</span></span>|<span data-ttu-id="76db7-121">Wert</span><span class="sxs-lookup"><span data-stu-id="76db7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76db7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="76db7-122">Authorization</span></span>|<span data-ttu-id="76db7-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="76db7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76db7-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="76db7-124">Accept</span></span>|<span data-ttu-id="76db7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="76db7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76db7-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="76db7-126">Request body</span></span>
<span data-ttu-id="76db7-127">Geben Sie im Anforderungstext eine JSON-Darstellung des iosVppApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="76db7-127">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="76db7-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosVppApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="76db7-128">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="76db7-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="76db7-129">Property</span></span>|<span data-ttu-id="76db7-130">Typ</span><span class="sxs-lookup"><span data-stu-id="76db7-130">Type</span></span>|<span data-ttu-id="76db7-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="76db7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76db7-132">id</span><span class="sxs-lookup"><span data-stu-id="76db7-132">id</span></span>|<span data-ttu-id="76db7-133">String</span><span class="sxs-lookup"><span data-stu-id="76db7-133">String</span></span>|<span data-ttu-id="76db7-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="76db7-134">Key of the entity.</span></span> <span data-ttu-id="76db7-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db7-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="76db7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="76db7-136">displayName</span></span>|<span data-ttu-id="76db7-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="76db7-137">String</span></span>|<span data-ttu-id="76db7-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="76db7-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="76db7-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db7-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="76db7-140">description</span><span class="sxs-lookup"><span data-stu-id="76db7-140">description</span></span>|<span data-ttu-id="76db7-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="76db7-141">String</span></span>|<span data-ttu-id="76db7-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="76db7-142">The description of the app.</span></span> <span data-ttu-id="76db7-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db7-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="76db7-144">publisher</span><span class="sxs-lookup"><span data-stu-id="76db7-144">publisher</span></span>|<span data-ttu-id="76db7-145">String</span><span class="sxs-lookup"><span data-stu-id="76db7-145">String</span></span>|<span data-ttu-id="76db7-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="76db7-146">The publisher of the app.</span></span> <span data-ttu-id="76db7-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db7-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="76db7-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="76db7-148">largeIcon</span></span>|[<span data-ttu-id="76db7-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="76db7-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="76db7-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="76db7-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="76db7-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db7-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="76db7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="76db7-152">createdDateTime</span></span>|<span data-ttu-id="76db7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76db7-153">DateTimeOffset</span></span>|<span data-ttu-id="76db7-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="76db7-154">The date and time the app was created.</span></span> <span data-ttu-id="76db7-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db7-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="76db7-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="76db7-156">lastModifiedDateTime</span></span>|<span data-ttu-id="76db7-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76db7-157">DateTimeOffset</span></span>|<span data-ttu-id="76db7-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="76db7-158">The date and time the app was last modified.</span></span> <span data-ttu-id="76db7-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db7-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="76db7-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="76db7-160">isFeatured</span></span>|<span data-ttu-id="76db7-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="76db7-161">Boolean</span></span>|<span data-ttu-id="76db7-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db7-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="76db7-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="76db7-163">privacyInformationUrl</span></span>|<span data-ttu-id="76db7-164">String</span><span class="sxs-lookup"><span data-stu-id="76db7-164">String</span></span>|<span data-ttu-id="76db7-165">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="76db7-165">The privacy statement Url.</span></span> <span data-ttu-id="76db7-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db7-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="76db7-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="76db7-167">informationUrl</span></span>|<span data-ttu-id="76db7-168">String</span><span class="sxs-lookup"><span data-stu-id="76db7-168">String</span></span>|<span data-ttu-id="76db7-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="76db7-169">The more information Url.</span></span> <span data-ttu-id="76db7-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db7-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="76db7-171">owner</span><span class="sxs-lookup"><span data-stu-id="76db7-171">owner</span></span>|<span data-ttu-id="76db7-172">String</span><span class="sxs-lookup"><span data-stu-id="76db7-172">String</span></span>|<span data-ttu-id="76db7-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="76db7-173">The owner of the app.</span></span> <span data-ttu-id="76db7-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db7-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="76db7-175">developer</span><span class="sxs-lookup"><span data-stu-id="76db7-175">developer</span></span>|<span data-ttu-id="76db7-176">String</span><span class="sxs-lookup"><span data-stu-id="76db7-176">String</span></span>|<span data-ttu-id="76db7-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="76db7-177">The developer of the app.</span></span> <span data-ttu-id="76db7-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db7-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="76db7-179">notes</span><span class="sxs-lookup"><span data-stu-id="76db7-179">notes</span></span>|<span data-ttu-id="76db7-180">String</span><span class="sxs-lookup"><span data-stu-id="76db7-180">String</span></span>|<span data-ttu-id="76db7-181">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="76db7-181">Notes for the app.</span></span> <span data-ttu-id="76db7-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db7-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="76db7-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="76db7-183">uploadState</span></span>|<span data-ttu-id="76db7-184">Int32</span><span class="sxs-lookup"><span data-stu-id="76db7-184">Int32</span></span>|<span data-ttu-id="76db7-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="76db7-185">The upload state.</span></span> <span data-ttu-id="76db7-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db7-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="76db7-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="76db7-187">publishingState</span></span>|[<span data-ttu-id="76db7-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="76db7-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="76db7-189">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="76db7-189">The publishing state for the app.</span></span> <span data-ttu-id="76db7-190">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="76db7-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="76db7-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="76db7-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="76db7-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="76db7-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="76db7-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="76db7-193">isAssigned</span></span>|<span data-ttu-id="76db7-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="76db7-194">Boolean</span></span>|<span data-ttu-id="76db7-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="76db7-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="76db7-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db7-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="76db7-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="76db7-197">roleScopeTagIds</span></span>|<span data-ttu-id="76db7-198">String collection</span><span class="sxs-lookup"><span data-stu-id="76db7-198">String collection</span></span>|<span data-ttu-id="76db7-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="76db7-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="76db7-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="76db7-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="76db7-201">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="76db7-201">usedLicenseCount</span></span>|<span data-ttu-id="76db7-202">Int32</span><span class="sxs-lookup"><span data-stu-id="76db7-202">Int32</span></span>|<span data-ttu-id="76db7-203">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="76db7-203">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="76db7-204">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="76db7-204">totalLicenseCount</span></span>|<span data-ttu-id="76db7-205">Int32</span><span class="sxs-lookup"><span data-stu-id="76db7-205">Int32</span></span>|<span data-ttu-id="76db7-206">Gesamtanzahl von VPP-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="76db7-206">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="76db7-207">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="76db7-207">releaseDateTime</span></span>|<span data-ttu-id="76db7-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76db7-208">DateTimeOffset</span></span>|<span data-ttu-id="76db7-209">Datum und Uhrzeit der Veröffentlichung der VPP-Anwendung.</span><span class="sxs-lookup"><span data-stu-id="76db7-209">The VPP application release date and time.</span></span>|
|<span data-ttu-id="76db7-210">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="76db7-210">appStoreUrl</span></span>|<span data-ttu-id="76db7-211">String</span><span class="sxs-lookup"><span data-stu-id="76db7-211">String</span></span>|<span data-ttu-id="76db7-212">Store-URL</span><span class="sxs-lookup"><span data-stu-id="76db7-212">The store URL.</span></span>|
|<span data-ttu-id="76db7-213">licensingType</span><span class="sxs-lookup"><span data-stu-id="76db7-213">licensingType</span></span>|[<span data-ttu-id="76db7-214">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="76db7-214">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="76db7-215">Unterstützter Lizenztyp</span><span class="sxs-lookup"><span data-stu-id="76db7-215">The supported License Type.</span></span>|
|<span data-ttu-id="76db7-216">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="76db7-216">applicableDeviceType</span></span>|[<span data-ttu-id="76db7-217">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="76db7-217">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="76db7-218">Gültiger iOS-Gerätetyp</span><span class="sxs-lookup"><span data-stu-id="76db7-218">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="76db7-219">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="76db7-219">vppTokenOrganizationName</span></span>|<span data-ttu-id="76db7-220">String</span><span class="sxs-lookup"><span data-stu-id="76db7-220">String</span></span>|<span data-ttu-id="76db7-221">Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="76db7-221">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="76db7-222">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="76db7-222">vppTokenAccountType</span></span>|[<span data-ttu-id="76db7-223">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="76db7-223">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="76db7-224">Volume Purchase Program-Typ, dem das angegebene Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="76db7-224">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="76db7-225">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="76db7-225">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="76db7-226">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="76db7-226">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="76db7-227">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="76db7-227">vppTokenAppleId</span></span>|<span data-ttu-id="76db7-228">String</span><span class="sxs-lookup"><span data-stu-id="76db7-228">String</span></span>|<span data-ttu-id="76db7-229">Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="76db7-229">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="76db7-230">bundleId</span><span class="sxs-lookup"><span data-stu-id="76db7-230">bundleId</span></span>|<span data-ttu-id="76db7-231">String</span><span class="sxs-lookup"><span data-stu-id="76db7-231">String</span></span>|<span data-ttu-id="76db7-232">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="76db7-232">The Identity Name.</span></span>|
|<span data-ttu-id="76db7-233">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="76db7-233">vppTokenId</span></span>|<span data-ttu-id="76db7-234">String</span><span class="sxs-lookup"><span data-stu-id="76db7-234">String</span></span>|<span data-ttu-id="76db7-235">Der Bezeichner des VPP-Tokens, das dieser APP zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="76db7-235">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="76db7-236">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="76db7-236">revokeLicenseActionResults</span></span>|<span data-ttu-id="76db7-237">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="76db7-237">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="76db7-238">Ergebnisse der widerrufen Lizenz Aktionen auf dieser app.</span><span class="sxs-lookup"><span data-stu-id="76db7-238">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="76db7-239">Antwort</span><span class="sxs-lookup"><span data-stu-id="76db7-239">Response</span></span>
<span data-ttu-id="76db7-240">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [iosVppApp](../resources/intune-apps-iosvppapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="76db7-240">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76db7-241">Beispiel</span><span class="sxs-lookup"><span data-stu-id="76db7-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="76db7-242">Anforderung</span><span class="sxs-lookup"><span data-stu-id="76db7-242">Request</span></span>
<span data-ttu-id="76db7-243">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="76db7-243">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1972

{
  "@odata.type": "#microsoft.graph.iosVppApp",
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
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="76db7-244">Antwort</span><span class="sxs-lookup"><span data-stu-id="76db7-244">Response</span></span>
<span data-ttu-id="76db7-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="76db7-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2144

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```




