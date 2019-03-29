---
title: microsoftStoreForBusinessApp erstellen
description: Erstellen eines neuen microsoftStoreForBusinessApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39a5ff6c11a30b7fea7d93875e344fddfa6febe3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978787"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="4cc62-103">microsoftStoreForBusinessApp erstellen</span><span class="sxs-lookup"><span data-stu-id="4cc62-103">Create microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="4cc62-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4cc62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4cc62-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4cc62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cc62-106">Erstellen eines neuen [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4cc62-106">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4cc62-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4cc62-107">Prerequisites</span></span>
<span data-ttu-id="4cc62-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cc62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cc62-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4cc62-110">Permission type</span></span>|<span data-ttu-id="4cc62-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4cc62-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4cc62-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4cc62-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4cc62-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cc62-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4cc62-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4cc62-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4cc62-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4cc62-115">Not supported.</span></span>|
|<span data-ttu-id="4cc62-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4cc62-116">Application</span></span>|<span data-ttu-id="4cc62-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4cc62-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4cc62-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4cc62-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="4cc62-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4cc62-119">Request headers</span></span>
|<span data-ttu-id="4cc62-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4cc62-120">Header</span></span>|<span data-ttu-id="4cc62-121">Wert</span><span class="sxs-lookup"><span data-stu-id="4cc62-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4cc62-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cc62-122">Authorization</span></span>|<span data-ttu-id="4cc62-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4cc62-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4cc62-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4cc62-124">Accept</span></span>|<span data-ttu-id="4cc62-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4cc62-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cc62-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4cc62-126">Request body</span></span>
<span data-ttu-id="4cc62-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das microsoftStoreForBusinessApp-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="4cc62-127">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="4cc62-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der microsoftStoreForBusinessApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="4cc62-128">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="4cc62-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4cc62-129">Property</span></span>|<span data-ttu-id="4cc62-130">Typ</span><span class="sxs-lookup"><span data-stu-id="4cc62-130">Type</span></span>|<span data-ttu-id="4cc62-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4cc62-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cc62-132">id</span><span class="sxs-lookup"><span data-stu-id="4cc62-132">id</span></span>|<span data-ttu-id="4cc62-133">String</span><span class="sxs-lookup"><span data-stu-id="4cc62-133">String</span></span>|<span data-ttu-id="4cc62-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4cc62-134">Key of the entity.</span></span> <span data-ttu-id="4cc62-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4cc62-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4cc62-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4cc62-136">displayName</span></span>|<span data-ttu-id="4cc62-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4cc62-137">String</span></span>|<span data-ttu-id="4cc62-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="4cc62-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4cc62-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4cc62-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4cc62-140">description</span><span class="sxs-lookup"><span data-stu-id="4cc62-140">description</span></span>|<span data-ttu-id="4cc62-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4cc62-141">String</span></span>|<span data-ttu-id="4cc62-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="4cc62-142">The description of the app.</span></span> <span data-ttu-id="4cc62-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4cc62-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4cc62-144">publisher</span><span class="sxs-lookup"><span data-stu-id="4cc62-144">publisher</span></span>|<span data-ttu-id="4cc62-145">String</span><span class="sxs-lookup"><span data-stu-id="4cc62-145">String</span></span>|<span data-ttu-id="4cc62-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="4cc62-146">The publisher of the app.</span></span> <span data-ttu-id="4cc62-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4cc62-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4cc62-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4cc62-148">largeIcon</span></span>|[<span data-ttu-id="4cc62-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4cc62-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4cc62-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="4cc62-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4cc62-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4cc62-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4cc62-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4cc62-152">createdDateTime</span></span>|<span data-ttu-id="4cc62-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cc62-153">DateTimeOffset</span></span>|<span data-ttu-id="4cc62-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="4cc62-154">The date and time the app was created.</span></span> <span data-ttu-id="4cc62-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4cc62-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4cc62-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4cc62-156">lastModifiedDateTime</span></span>|<span data-ttu-id="4cc62-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cc62-157">DateTimeOffset</span></span>|<span data-ttu-id="4cc62-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="4cc62-158">The date and time the app was last modified.</span></span> <span data-ttu-id="4cc62-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4cc62-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4cc62-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4cc62-160">isFeatured</span></span>|<span data-ttu-id="4cc62-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="4cc62-161">Boolean</span></span>|<span data-ttu-id="4cc62-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4cc62-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4cc62-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4cc62-163">privacyInformationUrl</span></span>|<span data-ttu-id="4cc62-164">String</span><span class="sxs-lookup"><span data-stu-id="4cc62-164">String</span></span>|<span data-ttu-id="4cc62-165">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="4cc62-165">The privacy statement Url.</span></span> <span data-ttu-id="4cc62-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4cc62-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4cc62-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4cc62-167">informationUrl</span></span>|<span data-ttu-id="4cc62-168">String</span><span class="sxs-lookup"><span data-stu-id="4cc62-168">String</span></span>|<span data-ttu-id="4cc62-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="4cc62-169">The more information Url.</span></span> <span data-ttu-id="4cc62-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4cc62-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4cc62-171">owner</span><span class="sxs-lookup"><span data-stu-id="4cc62-171">owner</span></span>|<span data-ttu-id="4cc62-172">String</span><span class="sxs-lookup"><span data-stu-id="4cc62-172">String</span></span>|<span data-ttu-id="4cc62-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="4cc62-173">The owner of the app.</span></span> <span data-ttu-id="4cc62-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4cc62-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4cc62-175">developer</span><span class="sxs-lookup"><span data-stu-id="4cc62-175">developer</span></span>|<span data-ttu-id="4cc62-176">String</span><span class="sxs-lookup"><span data-stu-id="4cc62-176">String</span></span>|<span data-ttu-id="4cc62-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="4cc62-177">The developer of the app.</span></span> <span data-ttu-id="4cc62-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4cc62-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4cc62-179">notes</span><span class="sxs-lookup"><span data-stu-id="4cc62-179">notes</span></span>|<span data-ttu-id="4cc62-180">String</span><span class="sxs-lookup"><span data-stu-id="4cc62-180">String</span></span>|<span data-ttu-id="4cc62-181">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="4cc62-181">Notes for the app.</span></span> <span data-ttu-id="4cc62-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4cc62-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4cc62-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="4cc62-183">uploadState</span></span>|<span data-ttu-id="4cc62-184">Int32</span><span class="sxs-lookup"><span data-stu-id="4cc62-184">Int32</span></span>|<span data-ttu-id="4cc62-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="4cc62-185">The upload state.</span></span> <span data-ttu-id="4cc62-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4cc62-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4cc62-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="4cc62-187">publishingState</span></span>|[<span data-ttu-id="4cc62-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4cc62-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4cc62-189">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="4cc62-189">The publishing state for the app.</span></span> <span data-ttu-id="4cc62-190">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="4cc62-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4cc62-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="4cc62-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="4cc62-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="4cc62-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4cc62-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4cc62-193">isAssigned</span></span>|<span data-ttu-id="4cc62-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4cc62-194">Boolean</span></span>|<span data-ttu-id="4cc62-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="4cc62-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4cc62-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4cc62-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4cc62-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="4cc62-197">roleScopeTagIds</span></span>|<span data-ttu-id="4cc62-198">String collection</span><span class="sxs-lookup"><span data-stu-id="4cc62-198">String collection</span></span>|<span data-ttu-id="4cc62-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="4cc62-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4cc62-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4cc62-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4cc62-201">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="4cc62-201">usedLicenseCount</span></span>|<span data-ttu-id="4cc62-202">Int32</span><span class="sxs-lookup"><span data-stu-id="4cc62-202">Int32</span></span>|<span data-ttu-id="4cc62-203">Die Anzahl von verwendeten Microsoft Store für Unternehmen-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="4cc62-203">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="4cc62-204">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="4cc62-204">totalLicenseCount</span></span>|<span data-ttu-id="4cc62-205">Int32</span><span class="sxs-lookup"><span data-stu-id="4cc62-205">Int32</span></span>|<span data-ttu-id="4cc62-206">Die Gesamtzahl der Microsoft Store für Unternehmen-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="4cc62-206">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="4cc62-207">productKey</span><span class="sxs-lookup"><span data-stu-id="4cc62-207">productKey</span></span>|<span data-ttu-id="4cc62-208">String</span><span class="sxs-lookup"><span data-stu-id="4cc62-208">String</span></span>|<span data-ttu-id="4cc62-209">Der Product Key der App</span><span class="sxs-lookup"><span data-stu-id="4cc62-209">The app product key</span></span>|
|<span data-ttu-id="4cc62-210">licenseType</span><span class="sxs-lookup"><span data-stu-id="4cc62-210">licenseType</span></span>|[<span data-ttu-id="4cc62-211">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="4cc62-211">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="4cc62-212">Der APP-Lizenztyp.</span><span class="sxs-lookup"><span data-stu-id="4cc62-212">The app license type.</span></span> <span data-ttu-id="4cc62-213">Mögliche Werte sind: `offline` und `online`.</span><span class="sxs-lookup"><span data-stu-id="4cc62-213">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="4cc62-214">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="4cc62-214">packageIdentityName</span></span>|<span data-ttu-id="4cc62-215">String</span><span class="sxs-lookup"><span data-stu-id="4cc62-215">String</span></span>|<span data-ttu-id="4cc62-216">Bezeichner des App-Pakets</span><span class="sxs-lookup"><span data-stu-id="4cc62-216">The app package identifier</span></span>|
|<span data-ttu-id="4cc62-217">licensingType</span><span class="sxs-lookup"><span data-stu-id="4cc62-217">licensingType</span></span>|[<span data-ttu-id="4cc62-218">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="4cc62-218">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="4cc62-219">Unterstützter Lizenztyp</span><span class="sxs-lookup"><span data-stu-id="4cc62-219">The supported License Type.</span></span>|



## <a name="response"></a><span data-ttu-id="4cc62-220">Antwort</span><span class="sxs-lookup"><span data-stu-id="4cc62-220">Response</span></span>
<span data-ttu-id="4cc62-221">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4cc62-221">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cc62-222">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4cc62-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="4cc62-223">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4cc62-223">Request</span></span>
<span data-ttu-id="4cc62-224">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4cc62-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4cc62-225">Antwort</span><span class="sxs-lookup"><span data-stu-id="4cc62-225">Response</span></span>
<span data-ttu-id="4cc62-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4cc62-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




