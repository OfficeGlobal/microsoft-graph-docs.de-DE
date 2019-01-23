---
title: Erstellen von officeSuiteApp
description: Erstellen eines neuen OfficeSuiteApp-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c1821c88f974bf61fe23de6bb34cfeb06d9250f6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405842"
---
# <a name="create-officesuiteapp"></a><span data-ttu-id="80461-103">Erstellen von officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="80461-103">Create officeSuiteApp</span></span>

> <span data-ttu-id="80461-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="80461-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="80461-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="80461-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80461-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="80461-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80461-107">Erstellen eines neuen [OfficeSuiteApp](../resources/intune-apps-officesuiteapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="80461-107">Create a new [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80461-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="80461-108">Prerequisites</span></span>
<span data-ttu-id="80461-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="80461-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="80461-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="80461-111">Permission type</span></span>|<span data-ttu-id="80461-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="80461-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80461-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="80461-113">Delegated (work or school account)</span></span>|<span data-ttu-id="80461-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80461-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="80461-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="80461-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80461-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80461-116">Not supported.</span></span>|
|<span data-ttu-id="80461-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="80461-117">Application</span></span>|<span data-ttu-id="80461-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80461-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80461-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="80461-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="80461-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="80461-120">Request headers</span></span>
|<span data-ttu-id="80461-121">Header</span><span class="sxs-lookup"><span data-stu-id="80461-121">Header</span></span>|<span data-ttu-id="80461-122">Wert</span><span class="sxs-lookup"><span data-stu-id="80461-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80461-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="80461-123">Authorization</span></span>|<span data-ttu-id="80461-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="80461-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80461-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="80461-125">Accept</span></span>|<span data-ttu-id="80461-126">application/json</span><span class="sxs-lookup"><span data-stu-id="80461-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80461-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="80461-127">Request body</span></span>
<span data-ttu-id="80461-128">Geben Sie im Textkörper Anforderung für das Objekt OfficeSuiteApp eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="80461-128">In the request body, supply a JSON representation for the officeSuiteApp object.</span></span>

<span data-ttu-id="80461-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die OfficeSuiteApp erstellen.</span><span class="sxs-lookup"><span data-stu-id="80461-129">The following table shows the properties that are required when you create the officeSuiteApp.</span></span>

|<span data-ttu-id="80461-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="80461-130">Property</span></span>|<span data-ttu-id="80461-131">Typ</span><span class="sxs-lookup"><span data-stu-id="80461-131">Type</span></span>|<span data-ttu-id="80461-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80461-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80461-133">id</span><span class="sxs-lookup"><span data-stu-id="80461-133">id</span></span>|<span data-ttu-id="80461-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80461-134">String</span></span>|<span data-ttu-id="80461-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="80461-135">Key of the entity.</span></span> <span data-ttu-id="80461-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80461-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80461-137">displayName</span><span class="sxs-lookup"><span data-stu-id="80461-137">displayName</span></span>|<span data-ttu-id="80461-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80461-138">String</span></span>|<span data-ttu-id="80461-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="80461-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="80461-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80461-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80461-141">description</span><span class="sxs-lookup"><span data-stu-id="80461-141">description</span></span>|<span data-ttu-id="80461-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80461-142">String</span></span>|<span data-ttu-id="80461-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="80461-143">The description of the app.</span></span> <span data-ttu-id="80461-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80461-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80461-145">publisher</span><span class="sxs-lookup"><span data-stu-id="80461-145">publisher</span></span>|<span data-ttu-id="80461-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80461-146">String</span></span>|<span data-ttu-id="80461-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="80461-147">The publisher of the app.</span></span> <span data-ttu-id="80461-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80461-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80461-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="80461-149">largeIcon</span></span>|[<span data-ttu-id="80461-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="80461-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="80461-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="80461-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="80461-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80461-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80461-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="80461-153">createdDateTime</span></span>|<span data-ttu-id="80461-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80461-154">DateTimeOffset</span></span>|<span data-ttu-id="80461-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="80461-155">The date and time the app was created.</span></span> <span data-ttu-id="80461-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80461-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80461-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80461-157">lastModifiedDateTime</span></span>|<span data-ttu-id="80461-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80461-158">DateTimeOffset</span></span>|<span data-ttu-id="80461-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="80461-159">The date and time the app was last modified.</span></span> <span data-ttu-id="80461-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80461-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80461-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="80461-161">isFeatured</span></span>|<span data-ttu-id="80461-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="80461-162">Boolean</span></span>|<span data-ttu-id="80461-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80461-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80461-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="80461-164">privacyInformationUrl</span></span>|<span data-ttu-id="80461-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80461-165">String</span></span>|<span data-ttu-id="80461-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="80461-166">The privacy statement Url.</span></span> <span data-ttu-id="80461-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80461-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80461-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="80461-168">informationUrl</span></span>|<span data-ttu-id="80461-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80461-169">String</span></span>|<span data-ttu-id="80461-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="80461-170">The more information Url.</span></span> <span data-ttu-id="80461-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80461-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80461-172">owner</span><span class="sxs-lookup"><span data-stu-id="80461-172">owner</span></span>|<span data-ttu-id="80461-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80461-173">String</span></span>|<span data-ttu-id="80461-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="80461-174">The owner of the app.</span></span> <span data-ttu-id="80461-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80461-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80461-176">developer</span><span class="sxs-lookup"><span data-stu-id="80461-176">developer</span></span>|<span data-ttu-id="80461-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80461-177">String</span></span>|<span data-ttu-id="80461-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="80461-178">The developer of the app.</span></span> <span data-ttu-id="80461-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80461-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80461-180">notes</span><span class="sxs-lookup"><span data-stu-id="80461-180">notes</span></span>|<span data-ttu-id="80461-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80461-181">String</span></span>|<span data-ttu-id="80461-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="80461-182">Notes for the app.</span></span> <span data-ttu-id="80461-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80461-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80461-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="80461-184">uploadState</span></span>|<span data-ttu-id="80461-185">Int32</span><span class="sxs-lookup"><span data-stu-id="80461-185">Int32</span></span>|<span data-ttu-id="80461-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="80461-186">The upload state.</span></span> <span data-ttu-id="80461-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80461-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80461-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="80461-188">publishingState</span></span>|[<span data-ttu-id="80461-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="80461-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="80461-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="80461-190">The publishing state for the app.</span></span> <span data-ttu-id="80461-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="80461-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="80461-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80461-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="80461-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="80461-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="80461-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="80461-194">isAssigned</span></span>|<span data-ttu-id="80461-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="80461-195">Boolean</span></span>|<span data-ttu-id="80461-196">Der Wert, der angibt, ob die app mindestens eine Gruppe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="80461-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="80461-197">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80461-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80461-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="80461-198">roleScopeTagIds</span></span>|<span data-ttu-id="80461-199">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="80461-199">String collection</span></span>|<span data-ttu-id="80461-200">Liste der Bereichs-Tag-Ids für diese mobile app.</span><span class="sxs-lookup"><span data-stu-id="80461-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="80461-201">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80461-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80461-202">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="80461-202">autoAcceptEula</span></span>|<span data-ttu-id="80461-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="80461-203">Boolean</span></span>|<span data-ttu-id="80461-204">Der Wert, der automatisch auf den des Endbenutzers Gerät den Lizenzvertrag zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="80461-204">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="80461-205">productIds</span><span class="sxs-lookup"><span data-stu-id="80461-205">productIds</span></span>|<span data-ttu-id="80461-206">[OfficeProductId](../resources/intune-apps-officeproductid.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="80461-206">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="80461-207">Die Produkt-Ids, die die Office365 Suite SKU darstellen.</span><span class="sxs-lookup"><span data-stu-id="80461-207">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="80461-208">Mögliche Werte: sind `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail` und `projectProRetail`.</span><span class="sxs-lookup"><span data-stu-id="80461-208">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="80461-209">excludedApps</span><span class="sxs-lookup"><span data-stu-id="80461-209">excludedApps</span></span>|[<span data-ttu-id="80461-210">excludedApps</span><span class="sxs-lookup"><span data-stu-id="80461-210">excludedApps</span></span>](../resources/intune-apps-excludedapps.md)|<span data-ttu-id="80461-211">Die Eigenschaft, um die apps darstellen, die von der ausgewählten Office365 Produkt-ID ausgeschlossen werden</span><span class="sxs-lookup"><span data-stu-id="80461-211">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="80461-212">useSharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="80461-212">useSharedComputerActivation</span></span>|<span data-ttu-id="80461-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="80461-213">Boolean</span></span>|<span data-ttu-id="80461-214">Die Eigenschaft an, die darstellen, ob die Aktivierung gemeinsam genutzter Computer nicht für die app-Suite Office365 verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="80461-214">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="80461-215">updateChannel</span><span class="sxs-lookup"><span data-stu-id="80461-215">updateChannel</span></span>|[<span data-ttu-id="80461-216">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="80461-216">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="80461-217">Die Eigenschaft, die Update-Kanal Office365 darstellen.</span><span class="sxs-lookup"><span data-stu-id="80461-217">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="80461-218">Mögliche Werte sind: `none`, `current`, `deferred`, `firstReleaseCurrent` und `firstReleaseDeferred`.</span><span class="sxs-lookup"><span data-stu-id="80461-218">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span></span>|
|<span data-ttu-id="80461-219">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="80461-219">officePlatformArchitecture</span></span>|[<span data-ttu-id="80461-220">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="80461-220">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="80461-221">Die Eigenschaft, die Office365 app Suite Version darstellen.</span><span class="sxs-lookup"><span data-stu-id="80461-221">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="80461-222">Mögliche Werte sind: `none`, `x86`, `x64`, `arm`, `neutral` und `arm64`.</span><span class="sxs-lookup"><span data-stu-id="80461-222">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="80461-223">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="80461-223">localesToInstall</span></span>|<span data-ttu-id="80461-224">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="80461-224">String collection</span></span>|<span data-ttu-id="80461-225">Die Eigenschaft, um die Gebietsschemas darstellen, die installiert werden Wenn apps aus Office365 installiert wird.</span><span class="sxs-lookup"><span data-stu-id="80461-225">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="80461-226">Standard RFC 6033 verwendet.</span><span class="sxs-lookup"><span data-stu-id="80461-226">It uses standard RFC 6033.</span></span> <span data-ttu-id="80461-227">REF:https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="80461-227">Ref: https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="80461-228">installProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="80461-228">installProgressDisplayLevel</span></span>|[<span data-ttu-id="80461-229">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="80461-229">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="80461-230">Sie können die Anzeigeebene für die Installation des Fortschritts Setup-Benutzeroberfläche auf dem Gerät angeben.</span><span class="sxs-lookup"><span data-stu-id="80461-230">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="80461-231">Mögliche Werte sind: `none` und `full`.</span><span class="sxs-lookup"><span data-stu-id="80461-231">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="80461-232">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="80461-232">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="80461-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="80461-233">Boolean</span></span>|<span data-ttu-id="80461-234">Die Eigenschaft zum bestimmen, ob das vorhandene Office MSI deinstallieren, wenn eine Office365 app-Suite auf dem Gerät bereitgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="80461-234">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="80461-235">targetVersion</span><span class="sxs-lookup"><span data-stu-id="80461-235">targetVersion</span></span>|<span data-ttu-id="80461-236">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80461-236">String</span></span>|<span data-ttu-id="80461-237">Die Eigenschaft, die bestimmte Zielversion für die app-Suite Office365 darstellen, die auf den Geräten bereitgestellten blieb werden sollte.</span><span class="sxs-lookup"><span data-stu-id="80461-237">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="80461-238">updateVersion</span><span class="sxs-lookup"><span data-stu-id="80461-238">updateVersion</span></span>|<span data-ttu-id="80461-239">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80461-239">String</span></span>|<span data-ttu-id="80461-240">Die Eigenschaft, die Version darstellen, die bestimmten Zielversion für die app-Suite Office365 verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="80461-240">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="80461-241">officeConfigurationXml</span><span class="sxs-lookup"><span data-stu-id="80461-241">officeConfigurationXml</span></span>|<span data-ttu-id="80461-242">Binär</span><span class="sxs-lookup"><span data-stu-id="80461-242">Binary</span></span>|<span data-ttu-id="80461-243">Die Eigenschaft zur Darstellung der XML-Konfigurationsdatei, die für Office ProPlus Apps angegeben werden können.</span><span class="sxs-lookup"><span data-stu-id="80461-243">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="80461-244">Hat Vorrang vor allen anderen Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="80461-244">Takes precedence over all other properties.</span></span> <span data-ttu-id="80461-245">Wenn dieser Parameter angegeben wurde, wird die XML-Konfigurationsdatei zum Erstellen der app verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="80461-245">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="80461-246">Antwort</span><span class="sxs-lookup"><span data-stu-id="80461-246">Response</span></span>
<span data-ttu-id="80461-247">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [OfficeSuiteApp](../resources/intune-apps-officesuiteapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="80461-247">If successful, this method returns a `201 Created` response code and a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80461-248">Beispiel</span><span class="sxs-lookup"><span data-stu-id="80461-248">Example</span></span>

### <a name="request"></a><span data-ttu-id="80461-249">Anforderung</span><span class="sxs-lookup"><span data-stu-id="80461-249">Request</span></span>
<span data-ttu-id="80461-250">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="80461-250">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1552

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

### <a name="response"></a><span data-ttu-id="80461-251">Antwort</span><span class="sxs-lookup"><span data-stu-id="80461-251">Response</span></span>
<span data-ttu-id="80461-p125">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="80461-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1724

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




