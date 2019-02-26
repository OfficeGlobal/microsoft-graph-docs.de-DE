---
title: MacOsVppApp erstellen
description: Erstellen eines neuen macOsVppApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 50f09757ce9d5c2d8a2bed167ff5009d28a45911
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149322"
---
# <a name="create-macosvppapp"></a><span data-ttu-id="c1538-103">MacOsVppApp erstellen</span><span class="sxs-lookup"><span data-stu-id="c1538-103">Create macOsVppApp</span></span>

> <span data-ttu-id="c1538-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c1538-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1538-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c1538-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1538-106">Erstellen eines neuen [macOsVppApp](../resources/intune-apps-macosvppapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c1538-106">Create a new [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1538-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c1538-107">Prerequisites</span></span>
<span data-ttu-id="c1538-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c1538-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c1538-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c1538-110">Permission type</span></span>|<span data-ttu-id="c1538-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c1538-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1538-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c1538-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c1538-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1538-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c1538-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c1538-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1538-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1538-115">Not supported.</span></span>|
|<span data-ttu-id="c1538-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c1538-116">Application</span></span>|<span data-ttu-id="c1538-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1538-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1538-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1538-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c1538-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c1538-119">Request headers</span></span>
|<span data-ttu-id="c1538-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c1538-120">Header</span></span>|<span data-ttu-id="c1538-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c1538-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1538-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1538-122">Authorization</span></span>|<span data-ttu-id="c1538-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c1538-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1538-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c1538-124">Accept</span></span>|<span data-ttu-id="c1538-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c1538-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1538-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c1538-126">Request body</span></span>
<span data-ttu-id="c1538-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das macOsVppApp-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="c1538-127">In the request body, supply a JSON representation for the macOsVppApp object.</span></span>

<span data-ttu-id="c1538-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der macOsVppApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c1538-128">The following table shows the properties that are required when you create the macOsVppApp.</span></span>

|<span data-ttu-id="c1538-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c1538-129">Property</span></span>|<span data-ttu-id="c1538-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c1538-130">Type</span></span>|<span data-ttu-id="c1538-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1538-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1538-132">id</span><span class="sxs-lookup"><span data-stu-id="c1538-132">id</span></span>|<span data-ttu-id="c1538-133">string</span><span class="sxs-lookup"><span data-stu-id="c1538-133">String</span></span>|<span data-ttu-id="c1538-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c1538-134">Key of the entity.</span></span> <span data-ttu-id="c1538-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1538-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1538-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c1538-136">displayName</span></span>|<span data-ttu-id="c1538-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1538-137">String</span></span>|<span data-ttu-id="c1538-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="c1538-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c1538-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1538-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1538-140">description</span><span class="sxs-lookup"><span data-stu-id="c1538-140">description</span></span>|<span data-ttu-id="c1538-141">String</span><span class="sxs-lookup"><span data-stu-id="c1538-141">String</span></span>|<span data-ttu-id="c1538-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="c1538-142">The description of the app.</span></span> <span data-ttu-id="c1538-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1538-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1538-144">publisher</span><span class="sxs-lookup"><span data-stu-id="c1538-144">publisher</span></span>|<span data-ttu-id="c1538-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1538-145">String</span></span>|<span data-ttu-id="c1538-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="c1538-146">The publisher of the app.</span></span> <span data-ttu-id="c1538-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1538-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1538-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c1538-148">largeIcon</span></span>|[<span data-ttu-id="c1538-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c1538-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c1538-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="c1538-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c1538-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1538-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1538-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c1538-152">createdDateTime</span></span>|<span data-ttu-id="c1538-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1538-153">DateTimeOffset</span></span>|<span data-ttu-id="c1538-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="c1538-154">The date and time the app was created.</span></span> <span data-ttu-id="c1538-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1538-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1538-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1538-156">lastModifiedDateTime</span></span>|<span data-ttu-id="c1538-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1538-157">DateTimeOffset</span></span>|<span data-ttu-id="c1538-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="c1538-158">The date and time the app was last modified.</span></span> <span data-ttu-id="c1538-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1538-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1538-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c1538-160">isFeatured</span></span>|<span data-ttu-id="c1538-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c1538-161">Boolean</span></span>|<span data-ttu-id="c1538-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1538-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1538-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c1538-163">privacyInformationUrl</span></span>|<span data-ttu-id="c1538-164">String</span><span class="sxs-lookup"><span data-stu-id="c1538-164">String</span></span>|<span data-ttu-id="c1538-165">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="c1538-165">The privacy statement Url.</span></span> <span data-ttu-id="c1538-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1538-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1538-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c1538-167">informationUrl</span></span>|<span data-ttu-id="c1538-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1538-168">String</span></span>|<span data-ttu-id="c1538-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="c1538-169">The more information Url.</span></span> <span data-ttu-id="c1538-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1538-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1538-171">owner</span><span class="sxs-lookup"><span data-stu-id="c1538-171">owner</span></span>|<span data-ttu-id="c1538-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1538-172">String</span></span>|<span data-ttu-id="c1538-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="c1538-173">The owner of the app.</span></span> <span data-ttu-id="c1538-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1538-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1538-175">developer</span><span class="sxs-lookup"><span data-stu-id="c1538-175">developer</span></span>|<span data-ttu-id="c1538-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1538-176">String</span></span>|<span data-ttu-id="c1538-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="c1538-177">The developer of the app.</span></span> <span data-ttu-id="c1538-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1538-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1538-179">notes</span><span class="sxs-lookup"><span data-stu-id="c1538-179">notes</span></span>|<span data-ttu-id="c1538-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1538-180">String</span></span>|<span data-ttu-id="c1538-181">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="c1538-181">Notes for the app.</span></span> <span data-ttu-id="c1538-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1538-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1538-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="c1538-183">uploadState</span></span>|<span data-ttu-id="c1538-184">Int32</span><span class="sxs-lookup"><span data-stu-id="c1538-184">Int32</span></span>|<span data-ttu-id="c1538-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="c1538-185">The upload state.</span></span> <span data-ttu-id="c1538-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1538-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1538-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="c1538-187">publishingState</span></span>|[<span data-ttu-id="c1538-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c1538-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c1538-189">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="c1538-189">The publishing state for the app.</span></span> <span data-ttu-id="c1538-190">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="c1538-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c1538-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="c1538-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c1538-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="c1538-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c1538-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c1538-193">isAssigned</span></span>|<span data-ttu-id="c1538-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1538-194">Boolean</span></span>|<span data-ttu-id="c1538-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="c1538-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="c1538-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1538-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1538-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="c1538-197">roleScopeTagIds</span></span>|<span data-ttu-id="c1538-198">String collection</span><span class="sxs-lookup"><span data-stu-id="c1538-198">String collection</span></span>|<span data-ttu-id="c1538-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="c1538-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="c1538-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c1538-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1538-201">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="c1538-201">usedLicenseCount</span></span>|<span data-ttu-id="c1538-202">Int32</span><span class="sxs-lookup"><span data-stu-id="c1538-202">Int32</span></span>|<span data-ttu-id="c1538-203">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="c1538-203">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="c1538-204">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="c1538-204">totalLicenseCount</span></span>|<span data-ttu-id="c1538-205">Int32</span><span class="sxs-lookup"><span data-stu-id="c1538-205">Int32</span></span>|<span data-ttu-id="c1538-206">Gesamtanzahl von VPP-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="c1538-206">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="c1538-207">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="c1538-207">releaseDateTime</span></span>|<span data-ttu-id="c1538-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1538-208">DateTimeOffset</span></span>|<span data-ttu-id="c1538-209">Datum und Uhrzeit der Veröffentlichung der VPP-Anwendung.</span><span class="sxs-lookup"><span data-stu-id="c1538-209">The VPP application release date and time.</span></span>|
|<span data-ttu-id="c1538-210">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="c1538-210">appStoreUrl</span></span>|<span data-ttu-id="c1538-211">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1538-211">String</span></span>|<span data-ttu-id="c1538-212">Store-URL</span><span class="sxs-lookup"><span data-stu-id="c1538-212">The store URL.</span></span>|
|<span data-ttu-id="c1538-213">licensingType</span><span class="sxs-lookup"><span data-stu-id="c1538-213">licensingType</span></span>|[<span data-ttu-id="c1538-214">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="c1538-214">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="c1538-215">Unterstützter Lizenztyp</span><span class="sxs-lookup"><span data-stu-id="c1538-215">The supported License Type.</span></span>|
|<span data-ttu-id="c1538-216">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="c1538-216">vppTokenOrganizationName</span></span>|<span data-ttu-id="c1538-217">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1538-217">String</span></span>|<span data-ttu-id="c1538-218">Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="c1538-218">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="c1538-219">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="c1538-219">vppTokenAccountType</span></span>|[<span data-ttu-id="c1538-220">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="c1538-220">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="c1538-221">Volume Purchase Program-Typ, dem das angegebene Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="c1538-221">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="c1538-222">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="c1538-222">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="c1538-223">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="c1538-223">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="c1538-224">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="c1538-224">vppTokenAppleId</span></span>|<span data-ttu-id="c1538-225">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1538-225">String</span></span>|<span data-ttu-id="c1538-226">Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="c1538-226">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="c1538-227">bundleId</span><span class="sxs-lookup"><span data-stu-id="c1538-227">bundleId</span></span>|<span data-ttu-id="c1538-228">String</span><span class="sxs-lookup"><span data-stu-id="c1538-228">String</span></span>|<span data-ttu-id="c1538-229">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="c1538-229">The Identity Name.</span></span>|
|<span data-ttu-id="c1538-230">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="c1538-230">vppTokenId</span></span>|<span data-ttu-id="c1538-231">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c1538-231">String</span></span>|<span data-ttu-id="c1538-232">Der Bezeichner des VPP-Tokens, das dieser APP zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="c1538-232">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="c1538-233">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="c1538-233">revokeLicenseActionResults</span></span>|<span data-ttu-id="c1538-234">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="c1538-234">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="c1538-235">Ergebnisse der widerrufen Lizenz Aktionen auf dieser app.</span><span class="sxs-lookup"><span data-stu-id="c1538-235">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="c1538-236">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1538-236">Response</span></span>
<span data-ttu-id="c1538-237">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [macOsVppApp](../resources/intune-apps-macosvppapp.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c1538-237">If successful, this method returns a `201 Created` response code and a [macOsVppApp](../resources/intune-apps-macosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1538-238">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1538-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1538-239">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1538-239">Request</span></span>
<span data-ttu-id="c1538-240">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c1538-240">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1842

{
  "@odata.type": "#microsoft.graph.macOsVppApp",
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
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
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

### <a name="response"></a><span data-ttu-id="c1538-241">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1538-241">Response</span></span>
<span data-ttu-id="c1538-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1538-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2014

{
  "@odata.type": "#microsoft.graph.macOsVppApp",
  "id": "10b95265-5265-10b9-6552-b9106552b910",
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
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
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




