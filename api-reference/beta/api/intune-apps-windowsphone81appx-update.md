---
title: WindowsPhone81AppX aktualisieren
description: Aktualisieren Sie die Eigenschaften eines windowsPhone81AppX-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2d7f295c5d2e6441c550b74c316f598d7c1ffed1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823261"
---
# <a name="update-windowsphone81appx"></a><span data-ttu-id="5dfa6-103">WindowsPhone81AppX aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5dfa6-103">Update windowsPhone81AppX</span></span>

> <span data-ttu-id="5dfa6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5dfa6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5dfa6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5dfa6-107">Aktualisieren Sie die Eigenschaften eines [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-107">Update the properties of a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5dfa6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5dfa6-108">Prerequisites</span></span>
<span data-ttu-id="5dfa6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5dfa6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dfa6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5dfa6-111">Permission type</span></span>|<span data-ttu-id="5dfa6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5dfa6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5dfa6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5dfa6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5dfa6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dfa6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5dfa6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5dfa6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5dfa6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5dfa6-116">Not supported.</span></span>|
|<span data-ttu-id="5dfa6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5dfa6-117">Application</span></span>|<span data-ttu-id="5dfa6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5dfa6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5dfa6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5dfa6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="5dfa6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5dfa6-120">Request headers</span></span>
|<span data-ttu-id="5dfa6-121">Header</span><span class="sxs-lookup"><span data-stu-id="5dfa6-121">Header</span></span>|<span data-ttu-id="5dfa6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5dfa6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5dfa6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5dfa6-123">Authorization</span></span>|<span data-ttu-id="5dfa6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5dfa6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5dfa6-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5dfa6-125">Accept</span></span>|<span data-ttu-id="5dfa6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5dfa6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5dfa6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5dfa6-127">Request body</span></span>
<span data-ttu-id="5dfa6-128">Geben Sie im Textkörper Anforderung für das Objekt [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-128">In the request body, supply a JSON representation for the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

<span data-ttu-id="5dfa6-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-129">The following table shows the properties that are required when you create the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span>

|<span data-ttu-id="5dfa6-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5dfa6-130">Property</span></span>|<span data-ttu-id="5dfa6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5dfa6-131">Type</span></span>|<span data-ttu-id="5dfa6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5dfa6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dfa6-133">id</span><span class="sxs-lookup"><span data-stu-id="5dfa6-133">id</span></span>|<span data-ttu-id="5dfa6-134">String</span><span class="sxs-lookup"><span data-stu-id="5dfa6-134">String</span></span>|<span data-ttu-id="5dfa6-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5dfa6-135">Key of the entity.</span></span> <span data-ttu-id="5dfa6-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5dfa6-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5dfa6-137">displayName</span><span class="sxs-lookup"><span data-stu-id="5dfa6-137">displayName</span></span>|<span data-ttu-id="5dfa6-138">String</span><span class="sxs-lookup"><span data-stu-id="5dfa6-138">String</span></span>|<span data-ttu-id="5dfa6-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5dfa6-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5dfa6-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5dfa6-141">description</span><span class="sxs-lookup"><span data-stu-id="5dfa6-141">description</span></span>|<span data-ttu-id="5dfa6-142">String</span><span class="sxs-lookup"><span data-stu-id="5dfa6-142">String</span></span>|<span data-ttu-id="5dfa6-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-143">The description of the app.</span></span> <span data-ttu-id="5dfa6-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5dfa6-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5dfa6-145">publisher</span><span class="sxs-lookup"><span data-stu-id="5dfa6-145">publisher</span></span>|<span data-ttu-id="5dfa6-146">String</span><span class="sxs-lookup"><span data-stu-id="5dfa6-146">String</span></span>|<span data-ttu-id="5dfa6-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-147">The publisher of the app.</span></span> <span data-ttu-id="5dfa6-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5dfa6-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5dfa6-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5dfa6-149">largeIcon</span></span>|[<span data-ttu-id="5dfa6-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5dfa6-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5dfa6-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5dfa6-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5dfa6-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5dfa6-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5dfa6-153">createdDateTime</span></span>|<span data-ttu-id="5dfa6-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5dfa6-154">DateTimeOffset</span></span>|<span data-ttu-id="5dfa6-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-155">The date and time the app was created.</span></span> <span data-ttu-id="5dfa6-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5dfa6-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5dfa6-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5dfa6-157">lastModifiedDateTime</span></span>|<span data-ttu-id="5dfa6-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5dfa6-158">DateTimeOffset</span></span>|<span data-ttu-id="5dfa6-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-159">The date and time the app was last modified.</span></span> <span data-ttu-id="5dfa6-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5dfa6-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5dfa6-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5dfa6-161">isFeatured</span></span>|<span data-ttu-id="5dfa6-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5dfa6-162">Boolean</span></span>|<span data-ttu-id="5dfa6-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5dfa6-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5dfa6-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5dfa6-164">privacyInformationUrl</span></span>|<span data-ttu-id="5dfa6-165">String</span><span class="sxs-lookup"><span data-stu-id="5dfa6-165">String</span></span>|<span data-ttu-id="5dfa6-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-166">The privacy statement Url.</span></span> <span data-ttu-id="5dfa6-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5dfa6-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5dfa6-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5dfa6-168">informationUrl</span></span>|<span data-ttu-id="5dfa6-169">String</span><span class="sxs-lookup"><span data-stu-id="5dfa6-169">String</span></span>|<span data-ttu-id="5dfa6-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-170">The more information Url.</span></span> <span data-ttu-id="5dfa6-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5dfa6-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5dfa6-172">owner</span><span class="sxs-lookup"><span data-stu-id="5dfa6-172">owner</span></span>|<span data-ttu-id="5dfa6-173">String</span><span class="sxs-lookup"><span data-stu-id="5dfa6-173">String</span></span>|<span data-ttu-id="5dfa6-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-174">The owner of the app.</span></span> <span data-ttu-id="5dfa6-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5dfa6-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5dfa6-176">developer</span><span class="sxs-lookup"><span data-stu-id="5dfa6-176">developer</span></span>|<span data-ttu-id="5dfa6-177">String</span><span class="sxs-lookup"><span data-stu-id="5dfa6-177">String</span></span>|<span data-ttu-id="5dfa6-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-178">The developer of the app.</span></span> <span data-ttu-id="5dfa6-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5dfa6-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5dfa6-180">notes</span><span class="sxs-lookup"><span data-stu-id="5dfa6-180">notes</span></span>|<span data-ttu-id="5dfa6-181">String</span><span class="sxs-lookup"><span data-stu-id="5dfa6-181">String</span></span>|<span data-ttu-id="5dfa6-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-182">Notes for the app.</span></span> <span data-ttu-id="5dfa6-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5dfa6-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5dfa6-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="5dfa6-184">uploadState</span></span>|<span data-ttu-id="5dfa6-185">Int32</span><span class="sxs-lookup"><span data-stu-id="5dfa6-185">Int32</span></span>|<span data-ttu-id="5dfa6-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-186">The upload state.</span></span> <span data-ttu-id="5dfa6-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5dfa6-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5dfa6-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="5dfa6-188">publishingState</span></span>|[<span data-ttu-id="5dfa6-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="5dfa6-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="5dfa6-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-190">The publishing state for the app.</span></span> <span data-ttu-id="5dfa6-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5dfa6-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5dfa6-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="5dfa6-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5dfa6-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="5dfa6-194">committedContentVersion</span></span>|<span data-ttu-id="5dfa6-195">String</span><span class="sxs-lookup"><span data-stu-id="5dfa6-195">String</span></span>|<span data-ttu-id="5dfa6-196">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-196">The internal committed content version.</span></span> <span data-ttu-id="5dfa6-197">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="5dfa6-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5dfa6-198">fileName</span><span class="sxs-lookup"><span data-stu-id="5dfa6-198">fileName</span></span>|<span data-ttu-id="5dfa6-199">String</span><span class="sxs-lookup"><span data-stu-id="5dfa6-199">String</span></span>|<span data-ttu-id="5dfa6-200">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-200">The name of the main Lob application file.</span></span> <span data-ttu-id="5dfa6-201">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="5dfa6-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5dfa6-202">size</span><span class="sxs-lookup"><span data-stu-id="5dfa6-202">size</span></span>|<span data-ttu-id="5dfa6-203">Int64</span><span class="sxs-lookup"><span data-stu-id="5dfa6-203">Int64</span></span>|<span data-ttu-id="5dfa6-204">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="5dfa6-205">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="5dfa6-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5dfa6-206">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="5dfa6-206">applicableArchitectures</span></span>|[<span data-ttu-id="5dfa6-207">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="5dfa6-207">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="5dfa6-208">Die Windows-Architekturen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-208">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="5dfa6-209">Mögliche Werte: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-209">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="5dfa6-210">identityName</span><span class="sxs-lookup"><span data-stu-id="5dfa6-210">identityName</span></span>|<span data-ttu-id="5dfa6-211">String</span><span class="sxs-lookup"><span data-stu-id="5dfa6-211">String</span></span>|<span data-ttu-id="5dfa6-212">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="5dfa6-212">The Identity Name.</span></span>|
|<span data-ttu-id="5dfa6-213">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="5dfa6-213">identityPublisherHash</span></span>|<span data-ttu-id="5dfa6-214">String</span><span class="sxs-lookup"><span data-stu-id="5dfa6-214">String</span></span>|<span data-ttu-id="5dfa6-215">Der Hash des Identitätsherausgebers.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-215">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="5dfa6-216">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="5dfa6-216">identityResourceIdentifier</span></span>|<span data-ttu-id="5dfa6-217">String</span><span class="sxs-lookup"><span data-stu-id="5dfa6-217">String</span></span>|<span data-ttu-id="5dfa6-218">Der Identitätsressourcenbezeichner.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-218">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="5dfa6-219">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5dfa6-219">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="5dfa6-220">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5dfa6-220">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="5dfa6-221">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-221">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="5dfa6-222">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="5dfa6-222">phoneProductIdentifier</span></span>|<span data-ttu-id="5dfa6-223">String</span><span class="sxs-lookup"><span data-stu-id="5dfa6-223">String</span></span>|<span data-ttu-id="5dfa6-224">Die Produkt-ID des Telefons.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-224">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="5dfa6-225">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="5dfa6-225">phonePublisherId</span></span>|<span data-ttu-id="5dfa6-226">String</span><span class="sxs-lookup"><span data-stu-id="5dfa6-226">String</span></span>|<span data-ttu-id="5dfa6-227">Die Telefon Publisher-Id.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-227">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="5dfa6-228">identityVersion</span><span class="sxs-lookup"><span data-stu-id="5dfa6-228">identityVersion</span></span>|<span data-ttu-id="5dfa6-229">String</span><span class="sxs-lookup"><span data-stu-id="5dfa6-229">String</span></span>|<span data-ttu-id="5dfa6-230">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="5dfa6-230">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="5dfa6-231">Antwort</span><span class="sxs-lookup"><span data-stu-id="5dfa6-231">Response</span></span>
<span data-ttu-id="5dfa6-232">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-232">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dfa6-233">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5dfa6-233">Example</span></span>
### <a name="request"></a><span data-ttu-id="5dfa6-234">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5dfa6-234">Request</span></span>
<span data-ttu-id="5dfa6-235">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-235">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1362

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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="5dfa6-236">Antwort</span><span class="sxs-lookup"><span data-stu-id="5dfa6-236">Response</span></span>
<span data-ttu-id="5dfa6-p121">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5dfa6-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1527

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
  "id": "4ff27f80-7f80-4ff2-807f-f24f807ff24f",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```





