---
title: windowsMobileMSI aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs windowsMobileMSI.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cff6787f782c4c86cbcc9298c0205e75315614dd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950900"
---
# <a name="update-windowsmobilemsi"></a><span data-ttu-id="a94df-103">windowsMobileMSI aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a94df-103">Update windowsMobileMSI</span></span>

> <span data-ttu-id="a94df-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a94df-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a94df-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a94df-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a94df-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a94df-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a94df-107">Aktualisiert die Eigenschaften von Objekten des Typs [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="a94df-107">Update the properties of a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a94df-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a94df-108">Prerequisites</span></span>
<span data-ttu-id="a94df-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a94df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a94df-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a94df-111">Permission type</span></span>|<span data-ttu-id="a94df-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a94df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a94df-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a94df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a94df-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a94df-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a94df-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a94df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a94df-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a94df-116">Not supported.</span></span>|
|<span data-ttu-id="a94df-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a94df-117">Application</span></span>|<span data-ttu-id="a94df-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a94df-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a94df-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a94df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="a94df-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a94df-120">Request headers</span></span>
|<span data-ttu-id="a94df-121">Header</span><span class="sxs-lookup"><span data-stu-id="a94df-121">Header</span></span>|<span data-ttu-id="a94df-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a94df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a94df-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a94df-123">Authorization</span></span>|<span data-ttu-id="a94df-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a94df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a94df-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a94df-125">Accept</span></span>|<span data-ttu-id="a94df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a94df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a94df-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a94df-127">Request body</span></span>
<span data-ttu-id="a94df-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="a94df-128">In the request body, supply a JSON representation for the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="a94df-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="a94df-129">The following table shows the properties that are required when you create the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span></span>

|<span data-ttu-id="a94df-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a94df-130">Property</span></span>|<span data-ttu-id="a94df-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a94df-131">Type</span></span>|<span data-ttu-id="a94df-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a94df-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a94df-133">id</span><span class="sxs-lookup"><span data-stu-id="a94df-133">id</span></span>|<span data-ttu-id="a94df-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a94df-134">String</span></span>|<span data-ttu-id="a94df-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a94df-135">Key of the entity.</span></span> <span data-ttu-id="a94df-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a94df-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a94df-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a94df-137">displayName</span></span>|<span data-ttu-id="a94df-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a94df-138">String</span></span>|<span data-ttu-id="a94df-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="a94df-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a94df-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a94df-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a94df-141">description</span><span class="sxs-lookup"><span data-stu-id="a94df-141">description</span></span>|<span data-ttu-id="a94df-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a94df-142">String</span></span>|<span data-ttu-id="a94df-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="a94df-143">The description of the app.</span></span> <span data-ttu-id="a94df-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a94df-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a94df-145">publisher</span><span class="sxs-lookup"><span data-stu-id="a94df-145">publisher</span></span>|<span data-ttu-id="a94df-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a94df-146">String</span></span>|<span data-ttu-id="a94df-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="a94df-147">The publisher of the app.</span></span> <span data-ttu-id="a94df-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a94df-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a94df-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a94df-149">largeIcon</span></span>|[<span data-ttu-id="a94df-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a94df-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a94df-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="a94df-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a94df-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a94df-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a94df-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a94df-153">createdDateTime</span></span>|<span data-ttu-id="a94df-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a94df-154">DateTimeOffset</span></span>|<span data-ttu-id="a94df-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="a94df-155">The date and time the app was created.</span></span> <span data-ttu-id="a94df-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a94df-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a94df-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a94df-157">lastModifiedDateTime</span></span>|<span data-ttu-id="a94df-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a94df-158">DateTimeOffset</span></span>|<span data-ttu-id="a94df-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="a94df-159">The date and time the app was last modified.</span></span> <span data-ttu-id="a94df-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a94df-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a94df-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a94df-161">isFeatured</span></span>|<span data-ttu-id="a94df-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a94df-162">Boolean</span></span>|<span data-ttu-id="a94df-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a94df-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a94df-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a94df-164">privacyInformationUrl</span></span>|<span data-ttu-id="a94df-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a94df-165">String</span></span>|<span data-ttu-id="a94df-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="a94df-166">The privacy statement Url.</span></span> <span data-ttu-id="a94df-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a94df-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a94df-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a94df-168">informationUrl</span></span>|<span data-ttu-id="a94df-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a94df-169">String</span></span>|<span data-ttu-id="a94df-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="a94df-170">The more information Url.</span></span> <span data-ttu-id="a94df-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a94df-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a94df-172">owner</span><span class="sxs-lookup"><span data-stu-id="a94df-172">owner</span></span>|<span data-ttu-id="a94df-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a94df-173">String</span></span>|<span data-ttu-id="a94df-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="a94df-174">The owner of the app.</span></span> <span data-ttu-id="a94df-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a94df-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a94df-176">developer</span><span class="sxs-lookup"><span data-stu-id="a94df-176">developer</span></span>|<span data-ttu-id="a94df-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a94df-177">String</span></span>|<span data-ttu-id="a94df-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="a94df-178">The developer of the app.</span></span> <span data-ttu-id="a94df-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a94df-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a94df-180">notes</span><span class="sxs-lookup"><span data-stu-id="a94df-180">notes</span></span>|<span data-ttu-id="a94df-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a94df-181">String</span></span>|<span data-ttu-id="a94df-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="a94df-182">Notes for the app.</span></span> <span data-ttu-id="a94df-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a94df-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a94df-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="a94df-184">uploadState</span></span>|<span data-ttu-id="a94df-185">Int32</span><span class="sxs-lookup"><span data-stu-id="a94df-185">Int32</span></span>|<span data-ttu-id="a94df-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="a94df-186">The upload state.</span></span> <span data-ttu-id="a94df-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a94df-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a94df-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="a94df-188">publishingState</span></span>|[<span data-ttu-id="a94df-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a94df-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a94df-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="a94df-190">The publishing state for the app.</span></span> <span data-ttu-id="a94df-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="a94df-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a94df-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a94df-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a94df-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="a94df-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a94df-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="a94df-194">committedContentVersion</span></span>|<span data-ttu-id="a94df-195">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a94df-195">String</span></span>|<span data-ttu-id="a94df-196">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="a94df-196">The internal committed content version.</span></span> <span data-ttu-id="a94df-197">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a94df-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a94df-198">fileName</span><span class="sxs-lookup"><span data-stu-id="a94df-198">fileName</span></span>|<span data-ttu-id="a94df-199">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a94df-199">String</span></span>|<span data-ttu-id="a94df-200">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="a94df-200">The name of the main Lob application file.</span></span> <span data-ttu-id="a94df-201">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a94df-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a94df-202">size</span><span class="sxs-lookup"><span data-stu-id="a94df-202">size</span></span>|<span data-ttu-id="a94df-203">Int64</span><span class="sxs-lookup"><span data-stu-id="a94df-203">Int64</span></span>|<span data-ttu-id="a94df-204">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="a94df-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="a94df-205">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a94df-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a94df-206">commandLine</span><span class="sxs-lookup"><span data-stu-id="a94df-206">commandLine</span></span>|<span data-ttu-id="a94df-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a94df-207">String</span></span>|<span data-ttu-id="a94df-208">Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="a94df-208">The command line.</span></span>|
|<span data-ttu-id="a94df-209">productCode</span><span class="sxs-lookup"><span data-stu-id="a94df-209">productCode</span></span>|<span data-ttu-id="a94df-210">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a94df-210">String</span></span>|<span data-ttu-id="a94df-211">Produktcode</span><span class="sxs-lookup"><span data-stu-id="a94df-211">The product code.</span></span>|
|<span data-ttu-id="a94df-212">productVersion</span><span class="sxs-lookup"><span data-stu-id="a94df-212">productVersion</span></span>|<span data-ttu-id="a94df-213">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a94df-213">String</span></span>|<span data-ttu-id="a94df-214">Produktversion der branchenspezifischen Windows Mobile-MSI-App.</span><span class="sxs-lookup"><span data-stu-id="a94df-214">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="a94df-215">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="a94df-215">ignoreVersionDetection</span></span>|<span data-ttu-id="a94df-216">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a94df-216">Boolean</span></span>|<span data-ttu-id="a94df-217">Boolescher Wert, der steuert, ob nach der Installation der App auf einem Gerät die App-Version zur Erkennung der App verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="a94df-217">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="a94df-218">Setzen Sie diese Eigenschaft auf „true“ bei branchenspezifischen Windows Mobile-MSI-Apps, die sich selbstständig aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="a94df-218">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="a94df-219">identityVersion</span><span class="sxs-lookup"><span data-stu-id="a94df-219">identityVersion</span></span>|<span data-ttu-id="a94df-220">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a94df-220">String</span></span>|<span data-ttu-id="a94df-221">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="a94df-221">The identity version.</span></span>|
|<span data-ttu-id="a94df-222">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="a94df-222">useDeviceContext</span></span>|<span data-ttu-id="a94df-223">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a94df-223">Boolean</span></span>|<span data-ttu-id="a94df-224">Gibt an, ob ein Dualmodus-MSI-Datei im Gerätekontext installiert.</span><span class="sxs-lookup"><span data-stu-id="a94df-224">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="a94df-225">Bei true wird die app für alle Benutzer installiert werden.</span><span class="sxs-lookup"><span data-stu-id="a94df-225">If true, app will be installed for all users.</span></span> <span data-ttu-id="a94df-226">Bei false werden app pro Benutzer installiert.</span><span class="sxs-lookup"><span data-stu-id="a94df-226">If false, app will be installed per-user.</span></span> <span data-ttu-id="a94df-227">Wenn null, wird Service die MSI-Paket Standard-Install-Kontext verwenden.</span><span class="sxs-lookup"><span data-stu-id="a94df-227">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="a94df-228">Im Fall eines WAN-Dualmodus-MSI werden diese Standardeinstellung pro Benutzer.</span><span class="sxs-lookup"><span data-stu-id="a94df-228">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="a94df-229">Kann nicht für apps Dual-Modus festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="a94df-229">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="a94df-230">Kann nach der ursprünglichen Erstellung der Anwendung geändert werden.</span><span class="sxs-lookup"><span data-stu-id="a94df-230">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="a94df-231">Antwort</span><span class="sxs-lookup"><span data-stu-id="a94df-231">Response</span></span>
<span data-ttu-id="a94df-232">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a94df-232">If successful, this method returns a `200 OK` response code and an updated [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a94df-233">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a94df-233">Example</span></span>
### <a name="request"></a><span data-ttu-id="a94df-234">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a94df-234">Request</span></span>
<span data-ttu-id="a94df-235">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a94df-235">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 963

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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```

### <a name="response"></a><span data-ttu-id="a94df-236">Antwort</span><span class="sxs-lookup"><span data-stu-id="a94df-236">Response</span></span>
<span data-ttu-id="a94df-p122">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a94df-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1126

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```





