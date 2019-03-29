---
title: OfficeSuiteApp aktualisieren
description: Aktualisieren der Eigenschaften eines officeSuiteApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 90ca5b6c3c00f04f4120a7102b7f52a3255df263
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976995"
---
# <a name="update-officesuiteapp"></a><span data-ttu-id="4b5c1-103">OfficeSuiteApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4b5c1-103">Update officeSuiteApp</span></span>

> <span data-ttu-id="4b5c1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b5c1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b5c1-106">Aktualisieren der Eigenschaften eines [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-106">Update the properties of a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b5c1-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4b5c1-107">Prerequisites</span></span>
<span data-ttu-id="4b5c1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b5c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b5c1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4b5c1-110">Permission type</span></span>|<span data-ttu-id="4b5c1-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4b5c1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b5c1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4b5c1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4b5c1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b5c1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4b5c1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4b5c1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b5c1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4b5c1-115">Not supported.</span></span>|
|<span data-ttu-id="4b5c1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4b5c1-116">Application</span></span>|<span data-ttu-id="4b5c1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4b5c1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b5c1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b5c1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="4b5c1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4b5c1-119">Request headers</span></span>
|<span data-ttu-id="4b5c1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4b5c1-120">Header</span></span>|<span data-ttu-id="4b5c1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="4b5c1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b5c1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b5c1-122">Authorization</span></span>|<span data-ttu-id="4b5c1-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4b5c1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b5c1-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4b5c1-124">Accept</span></span>|<span data-ttu-id="4b5c1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4b5c1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b5c1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4b5c1-126">Request body</span></span>
<span data-ttu-id="4b5c1-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-127">In the request body, supply a JSON representation for the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

<span data-ttu-id="4b5c1-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [officeSuiteApp](../resources/intune-apps-officesuiteapp.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-128">The following table shows the properties that are required when you create the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span></span>

|<span data-ttu-id="4b5c1-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4b5c1-129">Property</span></span>|<span data-ttu-id="4b5c1-130">Typ</span><span class="sxs-lookup"><span data-stu-id="4b5c1-130">Type</span></span>|<span data-ttu-id="4b5c1-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b5c1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b5c1-132">id</span><span class="sxs-lookup"><span data-stu-id="4b5c1-132">id</span></span>|<span data-ttu-id="4b5c1-133">String</span><span class="sxs-lookup"><span data-stu-id="4b5c1-133">String</span></span>|<span data-ttu-id="4b5c1-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4b5c1-134">Key of the entity.</span></span> <span data-ttu-id="4b5c1-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b5c1-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b5c1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4b5c1-136">displayName</span></span>|<span data-ttu-id="4b5c1-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4b5c1-137">String</span></span>|<span data-ttu-id="4b5c1-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4b5c1-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b5c1-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b5c1-140">description</span><span class="sxs-lookup"><span data-stu-id="4b5c1-140">description</span></span>|<span data-ttu-id="4b5c1-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4b5c1-141">String</span></span>|<span data-ttu-id="4b5c1-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-142">The description of the app.</span></span> <span data-ttu-id="4b5c1-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b5c1-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b5c1-144">publisher</span><span class="sxs-lookup"><span data-stu-id="4b5c1-144">publisher</span></span>|<span data-ttu-id="4b5c1-145">String</span><span class="sxs-lookup"><span data-stu-id="4b5c1-145">String</span></span>|<span data-ttu-id="4b5c1-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-146">The publisher of the app.</span></span> <span data-ttu-id="4b5c1-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b5c1-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b5c1-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4b5c1-148">largeIcon</span></span>|[<span data-ttu-id="4b5c1-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4b5c1-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4b5c1-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4b5c1-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b5c1-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b5c1-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b5c1-152">createdDateTime</span></span>|<span data-ttu-id="4b5c1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b5c1-153">DateTimeOffset</span></span>|<span data-ttu-id="4b5c1-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-154">The date and time the app was created.</span></span> <span data-ttu-id="4b5c1-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b5c1-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b5c1-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b5c1-156">lastModifiedDateTime</span></span>|<span data-ttu-id="4b5c1-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b5c1-157">DateTimeOffset</span></span>|<span data-ttu-id="4b5c1-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-158">The date and time the app was last modified.</span></span> <span data-ttu-id="4b5c1-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b5c1-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b5c1-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4b5c1-160">isFeatured</span></span>|<span data-ttu-id="4b5c1-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b5c1-161">Boolean</span></span>|<span data-ttu-id="4b5c1-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b5c1-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b5c1-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4b5c1-163">privacyInformationUrl</span></span>|<span data-ttu-id="4b5c1-164">String</span><span class="sxs-lookup"><span data-stu-id="4b5c1-164">String</span></span>|<span data-ttu-id="4b5c1-165">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="4b5c1-165">The privacy statement Url.</span></span> <span data-ttu-id="4b5c1-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b5c1-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b5c1-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4b5c1-167">informationUrl</span></span>|<span data-ttu-id="4b5c1-168">String</span><span class="sxs-lookup"><span data-stu-id="4b5c1-168">String</span></span>|<span data-ttu-id="4b5c1-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-169">The more information Url.</span></span> <span data-ttu-id="4b5c1-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b5c1-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b5c1-171">owner</span><span class="sxs-lookup"><span data-stu-id="4b5c1-171">owner</span></span>|<span data-ttu-id="4b5c1-172">String</span><span class="sxs-lookup"><span data-stu-id="4b5c1-172">String</span></span>|<span data-ttu-id="4b5c1-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-173">The owner of the app.</span></span> <span data-ttu-id="4b5c1-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b5c1-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b5c1-175">developer</span><span class="sxs-lookup"><span data-stu-id="4b5c1-175">developer</span></span>|<span data-ttu-id="4b5c1-176">String</span><span class="sxs-lookup"><span data-stu-id="4b5c1-176">String</span></span>|<span data-ttu-id="4b5c1-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-177">The developer of the app.</span></span> <span data-ttu-id="4b5c1-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b5c1-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b5c1-179">notes</span><span class="sxs-lookup"><span data-stu-id="4b5c1-179">notes</span></span>|<span data-ttu-id="4b5c1-180">String</span><span class="sxs-lookup"><span data-stu-id="4b5c1-180">String</span></span>|<span data-ttu-id="4b5c1-181">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-181">Notes for the app.</span></span> <span data-ttu-id="4b5c1-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b5c1-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b5c1-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="4b5c1-183">uploadState</span></span>|<span data-ttu-id="4b5c1-184">Int32</span><span class="sxs-lookup"><span data-stu-id="4b5c1-184">Int32</span></span>|<span data-ttu-id="4b5c1-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-185">The upload state.</span></span> <span data-ttu-id="4b5c1-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b5c1-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b5c1-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="4b5c1-187">publishingState</span></span>|[<span data-ttu-id="4b5c1-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4b5c1-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4b5c1-189">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-189">The publishing state for the app.</span></span> <span data-ttu-id="4b5c1-190">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4b5c1-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="4b5c1-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4b5c1-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4b5c1-193">isAssigned</span></span>|<span data-ttu-id="4b5c1-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b5c1-194">Boolean</span></span>|<span data-ttu-id="4b5c1-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4b5c1-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b5c1-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b5c1-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="4b5c1-197">roleScopeTagIds</span></span>|<span data-ttu-id="4b5c1-198">String collection</span><span class="sxs-lookup"><span data-stu-id="4b5c1-198">String collection</span></span>|<span data-ttu-id="4b5c1-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4b5c1-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b5c1-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b5c1-201">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="4b5c1-201">autoAcceptEula</span></span>|<span data-ttu-id="4b5c1-202">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4b5c1-202">Boolean</span></span>|<span data-ttu-id="4b5c1-203">Der Wert, der EULA automatisch auf dem Gerät des endBENUTZERs akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-203">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="4b5c1-204">productIds</span><span class="sxs-lookup"><span data-stu-id="4b5c1-204">productIds</span></span>|<span data-ttu-id="4b5c1-205">[officeProductId](../resources/intune-apps-officeproductid.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="4b5c1-205">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="4b5c1-206">Die Produkt-IDs, die die SKU der Office365-Suite darstellen.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-206">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="4b5c1-207">Mögliche Werte sind: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail` und `projectProRetail`.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-207">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="4b5c1-208">excludedApps</span><span class="sxs-lookup"><span data-stu-id="4b5c1-208">excludedApps</span></span>|[<span data-ttu-id="4b5c1-209">excludedApps</span><span class="sxs-lookup"><span data-stu-id="4b5c1-209">excludedApps</span></span>](../resources/intune-apps-excludedapps.md)|<span data-ttu-id="4b5c1-210">Die Eigenschaft zur Darstellung der apps, die von der ausgewählten Office365-Produkt-ID ausgeschlossen werden.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-210">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="4b5c1-211">Eigenschaften usesharedcomputeractivation</span><span class="sxs-lookup"><span data-stu-id="4b5c1-211">useSharedComputerActivation</span></span>|<span data-ttu-id="4b5c1-212">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4b5c1-212">Boolean</span></span>|<span data-ttu-id="4b5c1-213">Die Eigenschaft, die angibt, ob die Aktivierung gemeinsam genutzter Computer nicht für die Office365-App-Suite verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-213">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="4b5c1-214">updateChannel</span><span class="sxs-lookup"><span data-stu-id="4b5c1-214">updateChannel</span></span>|[<span data-ttu-id="4b5c1-215">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="4b5c1-215">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="4b5c1-216">Die Eigenschaft, die den Office365-Aktualisierungs Kanal darstellt.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-216">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="4b5c1-217">Mögliche Werte: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-217">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span></span>|
|<span data-ttu-id="4b5c1-218">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="4b5c1-218">officePlatformArchitecture</span></span>|[<span data-ttu-id="4b5c1-219">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="4b5c1-219">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="4b5c1-220">Die Eigenschaft, die die Version der Office365-App-Suite darstellt.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-220">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="4b5c1-221">Mögliche Werte sind: `none`, `x86`, `x64`, `arm`, `neutral` und `arm64`.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-221">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="4b5c1-222">Localestoinstall wurden</span><span class="sxs-lookup"><span data-stu-id="4b5c1-222">localesToInstall</span></span>|<span data-ttu-id="4b5c1-223">String collection</span><span class="sxs-lookup"><span data-stu-id="4b5c1-223">String collection</span></span>|<span data-ttu-id="4b5c1-224">Die Eigenschaft, die die Gebietsschemas darstellt, die bei der Installation der apps von Office365 installiert werden.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-224">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="4b5c1-225">Es verwendet Standard RFC 6033.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-225">It uses standard RFC 6033.</span></span> <span data-ttu-id="4b5c1-226">Refhttps://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="4b5c1-226">Ref: https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="4b5c1-227">installProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="4b5c1-227">installProgressDisplayLevel</span></span>|[<span data-ttu-id="4b5c1-228">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="4b5c1-228">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="4b5c1-229">So geben Sie die Anzeigeebene für die Setup-Benutzeroberfläche des InstallationsfortSchritts auf dem Gerät an.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-229">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="4b5c1-230">Mögliche Werte sind: `none` und `full`.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-230">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="4b5c1-231">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="4b5c1-231">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="4b5c1-232">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="4b5c1-232">Boolean</span></span>|<span data-ttu-id="4b5c1-233">Die Eigenschaft, um zu bestimmen, ob eine vorhandene Office-MSI-Installation installiert werden soll, wenn eine Office365-App-Suite auf dem Gerät bereitgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-233">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="4b5c1-234">targetVersion</span><span class="sxs-lookup"><span data-stu-id="4b5c1-234">targetVersion</span></span>|<span data-ttu-id="4b5c1-235">String</span><span class="sxs-lookup"><span data-stu-id="4b5c1-235">String</span></span>|<span data-ttu-id="4b5c1-236">Die Eigenschaft, die die spezifische Zielversion für die Office365-App-Suite darstellt, die auf den Geräten bereitgestellt bleiben soll.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-236">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="4b5c1-237">updateVersion</span><span class="sxs-lookup"><span data-stu-id="4b5c1-237">updateVersion</span></span>|<span data-ttu-id="4b5c1-238">String</span><span class="sxs-lookup"><span data-stu-id="4b5c1-238">String</span></span>|<span data-ttu-id="4b5c1-239">Die Eigenschaft, die die Update Version darstellt, in der die spezifische Zielversion für die Office365-App-Suite verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-239">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="4b5c1-240">officeConfigurationXml</span><span class="sxs-lookup"><span data-stu-id="4b5c1-240">officeConfigurationXml</span></span>|<span data-ttu-id="4b5c1-241">Binär</span><span class="sxs-lookup"><span data-stu-id="4b5c1-241">Binary</span></span>|<span data-ttu-id="4b5c1-242">Die Eigenschaft, die die XML-Konfigurationsdatei darstellt, die für Office proPlus-apps angegeben werden kann.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-242">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="4b5c1-243">Vorrang vor allen anderen Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-243">Takes precedence over all other properties.</span></span> <span data-ttu-id="4b5c1-244">Wenn dieser Parameter vorhanden ist, wird die XML-Konfigurationsdatei zum Erstellen der APP verwendet.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-244">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="4b5c1-245">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b5c1-245">Response</span></span>
<span data-ttu-id="4b5c1-246">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-246">If successful, this method returns a `200 OK` response code and an updated [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b5c1-247">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4b5c1-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b5c1-248">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b5c1-248">Request</span></span>
<span data-ttu-id="4b5c1-249">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-249">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1572

{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
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
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "teams": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "current",
  "officePlatformArchitecture": "x86",
  "localesToInstall": [
    "Locales To Install value"
  ],
  "installProgressDisplayLevel": "full",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "Target Version value",
  "updateVersion": "Update Version value",
  "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
}
```

### <a name="response"></a><span data-ttu-id="4b5c1-250">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b5c1-250">Response</span></span>
<span data-ttu-id="4b5c1-p124">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1744

{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
  "id": "9b263b46-3b46-9b26-463b-269b463b269b",
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
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "teams": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "current",
  "officePlatformArchitecture": "x86",
  "localesToInstall": [
    "Locales To Install value"
  ],
  "installProgressDisplayLevel": "full",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "Target Version value",
  "updateVersion": "Update Version value",
  "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
}
```




