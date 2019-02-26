---
title: microsoftStoreForBusinessApp erstellen
description: Erstellen eines neuen microsoftStoreForBusinessApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3471bb6e06d3c201ed21c4b120ca4f37c8c4c2ab
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174961"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="814f0-103">microsoftStoreForBusinessApp erstellen</span><span class="sxs-lookup"><span data-stu-id="814f0-103">Create microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="814f0-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="814f0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="814f0-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="814f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="814f0-106">Erstellen eines neuen [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="814f0-106">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="814f0-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="814f0-107">Prerequisites</span></span>
<span data-ttu-id="814f0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="814f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="814f0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="814f0-110">Permission type</span></span>|<span data-ttu-id="814f0-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="814f0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="814f0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="814f0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="814f0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="814f0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="814f0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="814f0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="814f0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="814f0-115">Not supported.</span></span>|
|<span data-ttu-id="814f0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="814f0-116">Application</span></span>|<span data-ttu-id="814f0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="814f0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="814f0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="814f0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="814f0-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="814f0-119">Request headers</span></span>
|<span data-ttu-id="814f0-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="814f0-120">Header</span></span>|<span data-ttu-id="814f0-121">Wert</span><span class="sxs-lookup"><span data-stu-id="814f0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="814f0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="814f0-122">Authorization</span></span>|<span data-ttu-id="814f0-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="814f0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="814f0-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="814f0-124">Accept</span></span>|<span data-ttu-id="814f0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="814f0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="814f0-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="814f0-126">Request body</span></span>
<span data-ttu-id="814f0-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das microsoftStoreForBusinessApp-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="814f0-127">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="814f0-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der microsoftStoreForBusinessApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="814f0-128">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="814f0-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="814f0-129">Property</span></span>|<span data-ttu-id="814f0-130">Typ</span><span class="sxs-lookup"><span data-stu-id="814f0-130">Type</span></span>|<span data-ttu-id="814f0-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="814f0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="814f0-132">id</span><span class="sxs-lookup"><span data-stu-id="814f0-132">id</span></span>|<span data-ttu-id="814f0-133">string</span><span class="sxs-lookup"><span data-stu-id="814f0-133">String</span></span>|<span data-ttu-id="814f0-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="814f0-134">Key of the entity.</span></span> <span data-ttu-id="814f0-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="814f0-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="814f0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="814f0-136">displayName</span></span>|<span data-ttu-id="814f0-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="814f0-137">String</span></span>|<span data-ttu-id="814f0-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="814f0-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="814f0-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="814f0-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="814f0-140">description</span><span class="sxs-lookup"><span data-stu-id="814f0-140">description</span></span>|<span data-ttu-id="814f0-141">String</span><span class="sxs-lookup"><span data-stu-id="814f0-141">String</span></span>|<span data-ttu-id="814f0-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="814f0-142">The description of the app.</span></span> <span data-ttu-id="814f0-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="814f0-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="814f0-144">publisher</span><span class="sxs-lookup"><span data-stu-id="814f0-144">publisher</span></span>|<span data-ttu-id="814f0-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="814f0-145">String</span></span>|<span data-ttu-id="814f0-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="814f0-146">The publisher of the app.</span></span> <span data-ttu-id="814f0-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="814f0-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="814f0-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="814f0-148">largeIcon</span></span>|[<span data-ttu-id="814f0-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="814f0-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="814f0-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="814f0-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="814f0-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="814f0-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="814f0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="814f0-152">createdDateTime</span></span>|<span data-ttu-id="814f0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="814f0-153">DateTimeOffset</span></span>|<span data-ttu-id="814f0-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="814f0-154">The date and time the app was created.</span></span> <span data-ttu-id="814f0-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="814f0-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="814f0-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="814f0-156">lastModifiedDateTime</span></span>|<span data-ttu-id="814f0-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="814f0-157">DateTimeOffset</span></span>|<span data-ttu-id="814f0-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="814f0-158">The date and time the app was last modified.</span></span> <span data-ttu-id="814f0-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="814f0-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="814f0-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="814f0-160">isFeatured</span></span>|<span data-ttu-id="814f0-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="814f0-161">Boolean</span></span>|<span data-ttu-id="814f0-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="814f0-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="814f0-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="814f0-163">privacyInformationUrl</span></span>|<span data-ttu-id="814f0-164">String</span><span class="sxs-lookup"><span data-stu-id="814f0-164">String</span></span>|<span data-ttu-id="814f0-165">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="814f0-165">The privacy statement Url.</span></span> <span data-ttu-id="814f0-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="814f0-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="814f0-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="814f0-167">informationUrl</span></span>|<span data-ttu-id="814f0-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="814f0-168">String</span></span>|<span data-ttu-id="814f0-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="814f0-169">The more information Url.</span></span> <span data-ttu-id="814f0-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="814f0-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="814f0-171">owner</span><span class="sxs-lookup"><span data-stu-id="814f0-171">owner</span></span>|<span data-ttu-id="814f0-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="814f0-172">String</span></span>|<span data-ttu-id="814f0-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="814f0-173">The owner of the app.</span></span> <span data-ttu-id="814f0-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="814f0-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="814f0-175">developer</span><span class="sxs-lookup"><span data-stu-id="814f0-175">developer</span></span>|<span data-ttu-id="814f0-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="814f0-176">String</span></span>|<span data-ttu-id="814f0-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="814f0-177">The developer of the app.</span></span> <span data-ttu-id="814f0-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="814f0-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="814f0-179">notes</span><span class="sxs-lookup"><span data-stu-id="814f0-179">notes</span></span>|<span data-ttu-id="814f0-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="814f0-180">String</span></span>|<span data-ttu-id="814f0-181">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="814f0-181">Notes for the app.</span></span> <span data-ttu-id="814f0-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="814f0-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="814f0-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="814f0-183">uploadState</span></span>|<span data-ttu-id="814f0-184">Int32</span><span class="sxs-lookup"><span data-stu-id="814f0-184">Int32</span></span>|<span data-ttu-id="814f0-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="814f0-185">The upload state.</span></span> <span data-ttu-id="814f0-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="814f0-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="814f0-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="814f0-187">publishingState</span></span>|[<span data-ttu-id="814f0-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="814f0-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="814f0-189">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="814f0-189">The publishing state for the app.</span></span> <span data-ttu-id="814f0-190">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="814f0-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="814f0-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="814f0-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="814f0-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="814f0-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="814f0-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="814f0-193">isAssigned</span></span>|<span data-ttu-id="814f0-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="814f0-194">Boolean</span></span>|<span data-ttu-id="814f0-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="814f0-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="814f0-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="814f0-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="814f0-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="814f0-197">roleScopeTagIds</span></span>|<span data-ttu-id="814f0-198">String collection</span><span class="sxs-lookup"><span data-stu-id="814f0-198">String collection</span></span>|<span data-ttu-id="814f0-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="814f0-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="814f0-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="814f0-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="814f0-201">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="814f0-201">usedLicenseCount</span></span>|<span data-ttu-id="814f0-202">Int32</span><span class="sxs-lookup"><span data-stu-id="814f0-202">Int32</span></span>|<span data-ttu-id="814f0-203">Die Anzahl von verwendeten Microsoft Store für Unternehmen-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="814f0-203">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="814f0-204">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="814f0-204">totalLicenseCount</span></span>|<span data-ttu-id="814f0-205">Int32</span><span class="sxs-lookup"><span data-stu-id="814f0-205">Int32</span></span>|<span data-ttu-id="814f0-206">Die Gesamtzahl der Microsoft Store für Unternehmen-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="814f0-206">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="814f0-207">productKey</span><span class="sxs-lookup"><span data-stu-id="814f0-207">productKey</span></span>|<span data-ttu-id="814f0-208">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="814f0-208">String</span></span>|<span data-ttu-id="814f0-209">Der Product Key der App</span><span class="sxs-lookup"><span data-stu-id="814f0-209">The app product key</span></span>|
|<span data-ttu-id="814f0-210">licenseType</span><span class="sxs-lookup"><span data-stu-id="814f0-210">licenseType</span></span>|[<span data-ttu-id="814f0-211">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="814f0-211">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="814f0-212">Der APP-Lizenztyp.</span><span class="sxs-lookup"><span data-stu-id="814f0-212">The app license type.</span></span> <span data-ttu-id="814f0-213">Mögliche Werte sind: `offline` und `online`.</span><span class="sxs-lookup"><span data-stu-id="814f0-213">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="814f0-214">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="814f0-214">packageIdentityName</span></span>|<span data-ttu-id="814f0-215">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="814f0-215">String</span></span>|<span data-ttu-id="814f0-216">Bezeichner des App-Pakets</span><span class="sxs-lookup"><span data-stu-id="814f0-216">The app package identifier</span></span>|
|<span data-ttu-id="814f0-217">licensingType</span><span class="sxs-lookup"><span data-stu-id="814f0-217">licensingType</span></span>|[<span data-ttu-id="814f0-218">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="814f0-218">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="814f0-219">Unterstützter Lizenztyp</span><span class="sxs-lookup"><span data-stu-id="814f0-219">The supported License Type.</span></span>|



## <a name="response"></a><span data-ttu-id="814f0-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="814f0-220">Response</span></span>
<span data-ttu-id="814f0-221">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="814f0-221">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="814f0-222">Beispiel</span><span class="sxs-lookup"><span data-stu-id="814f0-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="814f0-223">Anforderung</span><span class="sxs-lookup"><span data-stu-id="814f0-223">Request</span></span>
<span data-ttu-id="814f0-224">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="814f0-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="814f0-225">Antwort</span><span class="sxs-lookup"><span data-stu-id="814f0-225">Response</span></span>
<span data-ttu-id="814f0-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="814f0-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




