---
title: OfficeSuiteApp aktualisieren
description: Aktualisieren Sie die Eigenschaften eines OfficeSuiteApp-Objekts.
author: tfitzmac
ms.openlocfilehash: 444bf90622d47d803a311e29d504dd8517369768
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337940"
---
# <a name="update-officesuiteapp"></a><span data-ttu-id="a6a31-103">OfficeSuiteApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a6a31-103">Update officeSuiteApp</span></span>

> <span data-ttu-id="a6a31-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a6a31-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6a31-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a6a31-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a6a31-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a6a31-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6a31-107">Aktualisieren Sie die Eigenschaften eines [OfficeSuiteApp](../resources/intune-apps-officesuiteapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="a6a31-107">Update the properties of a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a6a31-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a6a31-108">Prerequisites</span></span>
<span data-ttu-id="a6a31-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6a31-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6a31-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a6a31-111">Permission type</span></span>|<span data-ttu-id="a6a31-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a6a31-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6a31-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a6a31-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6a31-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6a31-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a6a31-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a6a31-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6a31-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a6a31-116">Not supported.</span></span>|
|<span data-ttu-id="a6a31-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a6a31-117">Application</span></span>|<span data-ttu-id="a6a31-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a6a31-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6a31-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6a31-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="a6a31-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a6a31-120">Request headers</span></span>
|<span data-ttu-id="a6a31-121">Header</span><span class="sxs-lookup"><span data-stu-id="a6a31-121">Header</span></span>|<span data-ttu-id="a6a31-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a6a31-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6a31-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a6a31-123">Authorization</span></span>|<span data-ttu-id="a6a31-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a6a31-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6a31-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a6a31-125">Accept</span></span>|<span data-ttu-id="a6a31-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6a31-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6a31-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a6a31-127">Request body</span></span>
<span data-ttu-id="a6a31-128">Geben Sie im Textkörper Anforderung für das Objekt [OfficeSuiteApp](../resources/intune-apps-officesuiteapp.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="a6a31-128">In the request body, supply a JSON representation for the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

<span data-ttu-id="a6a31-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [OfficeSuiteApp](../resources/intune-apps-officesuiteapp.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="a6a31-129">The following table shows the properties that are required when you create the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span></span>

|<span data-ttu-id="a6a31-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a6a31-130">Property</span></span>|<span data-ttu-id="a6a31-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a6a31-131">Type</span></span>|<span data-ttu-id="a6a31-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a6a31-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6a31-133">id</span><span class="sxs-lookup"><span data-stu-id="a6a31-133">id</span></span>|<span data-ttu-id="a6a31-134">String</span><span class="sxs-lookup"><span data-stu-id="a6a31-134">String</span></span>|<span data-ttu-id="a6a31-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a6a31-135">Key of the entity.</span></span> <span data-ttu-id="a6a31-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a6a31-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a31-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a6a31-137">displayName</span></span>|<span data-ttu-id="a6a31-138">String</span><span class="sxs-lookup"><span data-stu-id="a6a31-138">String</span></span>|<span data-ttu-id="a6a31-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="a6a31-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a6a31-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a6a31-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a31-141">description</span><span class="sxs-lookup"><span data-stu-id="a6a31-141">description</span></span>|<span data-ttu-id="a6a31-142">String</span><span class="sxs-lookup"><span data-stu-id="a6a31-142">String</span></span>|<span data-ttu-id="a6a31-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="a6a31-143">The description of the app.</span></span> <span data-ttu-id="a6a31-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a6a31-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a31-145">publisher</span><span class="sxs-lookup"><span data-stu-id="a6a31-145">publisher</span></span>|<span data-ttu-id="a6a31-146">String</span><span class="sxs-lookup"><span data-stu-id="a6a31-146">String</span></span>|<span data-ttu-id="a6a31-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="a6a31-147">The publisher of the app.</span></span> <span data-ttu-id="a6a31-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a6a31-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a31-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a6a31-149">largeIcon</span></span>|[<span data-ttu-id="a6a31-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a6a31-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a6a31-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="a6a31-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a6a31-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a6a31-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a31-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6a31-153">createdDateTime</span></span>|<span data-ttu-id="a6a31-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6a31-154">DateTimeOffset</span></span>|<span data-ttu-id="a6a31-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="a6a31-155">The date and time the app was created.</span></span> <span data-ttu-id="a6a31-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a6a31-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a31-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6a31-157">lastModifiedDateTime</span></span>|<span data-ttu-id="a6a31-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6a31-158">DateTimeOffset</span></span>|<span data-ttu-id="a6a31-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="a6a31-159">The date and time the app was last modified.</span></span> <span data-ttu-id="a6a31-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a6a31-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a31-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a6a31-161">isFeatured</span></span>|<span data-ttu-id="a6a31-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a6a31-162">Boolean</span></span>|<span data-ttu-id="a6a31-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a6a31-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a31-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a6a31-164">privacyInformationUrl</span></span>|<span data-ttu-id="a6a31-165">String</span><span class="sxs-lookup"><span data-stu-id="a6a31-165">String</span></span>|<span data-ttu-id="a6a31-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="a6a31-166">The privacy statement Url.</span></span> <span data-ttu-id="a6a31-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a6a31-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a31-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a6a31-168">informationUrl</span></span>|<span data-ttu-id="a6a31-169">String</span><span class="sxs-lookup"><span data-stu-id="a6a31-169">String</span></span>|<span data-ttu-id="a6a31-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="a6a31-170">The more information Url.</span></span> <span data-ttu-id="a6a31-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a6a31-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a31-172">owner</span><span class="sxs-lookup"><span data-stu-id="a6a31-172">owner</span></span>|<span data-ttu-id="a6a31-173">String</span><span class="sxs-lookup"><span data-stu-id="a6a31-173">String</span></span>|<span data-ttu-id="a6a31-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="a6a31-174">The owner of the app.</span></span> <span data-ttu-id="a6a31-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a6a31-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a31-176">developer</span><span class="sxs-lookup"><span data-stu-id="a6a31-176">developer</span></span>|<span data-ttu-id="a6a31-177">String</span><span class="sxs-lookup"><span data-stu-id="a6a31-177">String</span></span>|<span data-ttu-id="a6a31-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="a6a31-178">The developer of the app.</span></span> <span data-ttu-id="a6a31-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a6a31-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a31-180">notes</span><span class="sxs-lookup"><span data-stu-id="a6a31-180">notes</span></span>|<span data-ttu-id="a6a31-181">String</span><span class="sxs-lookup"><span data-stu-id="a6a31-181">String</span></span>|<span data-ttu-id="a6a31-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="a6a31-182">Notes for the app.</span></span> <span data-ttu-id="a6a31-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a6a31-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a31-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="a6a31-184">uploadState</span></span>|<span data-ttu-id="a6a31-185">Int32</span><span class="sxs-lookup"><span data-stu-id="a6a31-185">Int32</span></span>|<span data-ttu-id="a6a31-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="a6a31-186">The upload state.</span></span> <span data-ttu-id="a6a31-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a6a31-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a31-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="a6a31-188">publishingState</span></span>|[<span data-ttu-id="a6a31-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a6a31-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a6a31-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="a6a31-190">The publishing state for the app.</span></span> <span data-ttu-id="a6a31-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="a6a31-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a6a31-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a6a31-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a6a31-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="a6a31-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a6a31-194">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="a6a31-194">autoAcceptEula</span></span>|<span data-ttu-id="a6a31-195">Boolesch</span><span class="sxs-lookup"><span data-stu-id="a6a31-195">Boolean</span></span>|<span data-ttu-id="a6a31-196">Der Wert, der automatisch auf den des Endbenutzers Gerät den Lizenzvertrag zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="a6a31-196">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="a6a31-197">productIds</span><span class="sxs-lookup"><span data-stu-id="a6a31-197">productIds</span></span>|<span data-ttu-id="a6a31-198">[OfficeProductId](../resources/intune-apps-officeproductid.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="a6a31-198">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="a6a31-199">Die Produkt-Ids, die die Office365 Suite SKU darstellen.</span><span class="sxs-lookup"><span data-stu-id="a6a31-199">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="a6a31-200">Mögliche Werte: sind `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail` und `projectProRetail`.</span><span class="sxs-lookup"><span data-stu-id="a6a31-200">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="a6a31-201">excludedApps</span><span class="sxs-lookup"><span data-stu-id="a6a31-201">excludedApps</span></span>|[<span data-ttu-id="a6a31-202">excludedApps</span><span class="sxs-lookup"><span data-stu-id="a6a31-202">excludedApps</span></span>](../resources/intune-apps-excludedapps.md)|<span data-ttu-id="a6a31-203">Die Eigenschaft, um die apps darstellen, die von der ausgewählten Office365 Produkt-ID ausgeschlossen werden</span><span class="sxs-lookup"><span data-stu-id="a6a31-203">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="a6a31-204">useSharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="a6a31-204">useSharedComputerActivation</span></span>|<span data-ttu-id="a6a31-205">Boolesch</span><span class="sxs-lookup"><span data-stu-id="a6a31-205">Boolean</span></span>|<span data-ttu-id="a6a31-206">Die Eigenschaft an, die darstellen, ob die Aktivierung gemeinsam genutzter Computer nicht für die app-Suite Office365 verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="a6a31-206">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="a6a31-207">updateChannel</span><span class="sxs-lookup"><span data-stu-id="a6a31-207">updateChannel</span></span>|[<span data-ttu-id="a6a31-208">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="a6a31-208">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="a6a31-209">Die Eigenschaft, die Update-Kanal Office365 darstellen.</span><span class="sxs-lookup"><span data-stu-id="a6a31-209">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="a6a31-210">Mögliche Werte sind: `none`, `current`, `deferred`, `firstReleaseCurrent` und `firstReleaseDeferred`.</span><span class="sxs-lookup"><span data-stu-id="a6a31-210">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span></span>|
|<span data-ttu-id="a6a31-211">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="a6a31-211">officePlatformArchitecture</span></span>|[<span data-ttu-id="a6a31-212">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="a6a31-212">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="a6a31-213">Die Eigenschaft, die Office365 app Suite Version darstellen.</span><span class="sxs-lookup"><span data-stu-id="a6a31-213">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="a6a31-214">Mögliche Werte sind: `none`, `x86`, `x64`, `arm` und `neutral`.</span><span class="sxs-lookup"><span data-stu-id="a6a31-214">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="a6a31-215">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="a6a31-215">localesToInstall</span></span>|<span data-ttu-id="a6a31-216">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="a6a31-216">String collection</span></span>|<span data-ttu-id="a6a31-217">Die Eigenschaft, um die Gebietsschemas darstellen, die installiert werden Wenn apps aus Office365 installiert wird.</span><span class="sxs-lookup"><span data-stu-id="a6a31-217">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="a6a31-218">Standard RFC 6033 verwendet.</span><span class="sxs-lookup"><span data-stu-id="a6a31-218">It uses standard RFC 6033.</span></span> <span data-ttu-id="a6a31-219">REF:https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="a6a31-219">Ref: https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="a6a31-220">installProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="a6a31-220">installProgressDisplayLevel</span></span>|[<span data-ttu-id="a6a31-221">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="a6a31-221">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="a6a31-222">Sie können die Anzeigeebene für die Installation des Fortschritts Setup-Benutzeroberfläche auf dem Gerät angeben.</span><span class="sxs-lookup"><span data-stu-id="a6a31-222">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="a6a31-223">Mögliche Werte sind: `none` und `full`.</span><span class="sxs-lookup"><span data-stu-id="a6a31-223">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="a6a31-224">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="a6a31-224">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="a6a31-225">Boolesch</span><span class="sxs-lookup"><span data-stu-id="a6a31-225">Boolean</span></span>|<span data-ttu-id="a6a31-226">Die Eigenschaft zum bestimmen, ob das vorhandene Office MSI deinstallieren, wenn eine Office365 app-Suite auf dem Gerät bereitgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="a6a31-226">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="a6a31-227">targetVersion</span><span class="sxs-lookup"><span data-stu-id="a6a31-227">targetVersion</span></span>|<span data-ttu-id="a6a31-228">String</span><span class="sxs-lookup"><span data-stu-id="a6a31-228">String</span></span>|<span data-ttu-id="a6a31-229">Die Eigenschaft, die bestimmte Zielversion für die app-Suite Office365 darstellen, die auf den Geräten bereitgestellten blieb werden sollte.</span><span class="sxs-lookup"><span data-stu-id="a6a31-229">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="a6a31-230">updateVersion</span><span class="sxs-lookup"><span data-stu-id="a6a31-230">updateVersion</span></span>|<span data-ttu-id="a6a31-231">String</span><span class="sxs-lookup"><span data-stu-id="a6a31-231">String</span></span>|<span data-ttu-id="a6a31-232">Die Eigenschaft, die Version darstellen, die bestimmten Zielversion für die app-Suite Office365 verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="a6a31-232">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|



## <a name="response"></a><span data-ttu-id="a6a31-233">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6a31-233">Response</span></span>
<span data-ttu-id="a6a31-234">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [OfficeSuiteApp](../resources/intune-apps-officesuiteapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="a6a31-234">If successful, this method returns a `200 OK` response code and an updated [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6a31-235">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a6a31-235">Example</span></span>
### <a name="request"></a><span data-ttu-id="a6a31-236">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6a31-236">Request</span></span>
<span data-ttu-id="a6a31-237">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a6a31-237">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1413

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
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
  "updateVersion": "Update Version value"
}
```

### <a name="response"></a><span data-ttu-id="a6a31-238">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6a31-238">Response</span></span>
<span data-ttu-id="a6a31-p122">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a6a31-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

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
  "updateVersion": "Update Version value"
}
```





