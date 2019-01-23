---
title: MacOSLobApp aktualisieren
description: Aktualisieren Sie die Eigenschaften eines MacOSLobApp-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bcf3301fb022f672db1340f45296ca19763a4d63
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413598"
---
# <a name="update-macoslobapp"></a><span data-ttu-id="93856-103">MacOSLobApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="93856-103">Update macOSLobApp</span></span>

> <span data-ttu-id="93856-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="93856-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="93856-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="93856-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="93856-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="93856-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93856-107">Aktualisieren Sie die Eigenschaften eines [MacOSLobApp](../resources/intune-apps-macoslobapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="93856-107">Update the properties of a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93856-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="93856-108">Prerequisites</span></span>
<span data-ttu-id="93856-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="93856-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="93856-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="93856-111">Permission type</span></span>|<span data-ttu-id="93856-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="93856-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93856-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="93856-113">Delegated (work or school account)</span></span>|<span data-ttu-id="93856-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93856-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="93856-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="93856-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93856-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="93856-116">Not supported.</span></span>|
|<span data-ttu-id="93856-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="93856-117">Application</span></span>|<span data-ttu-id="93856-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="93856-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93856-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="93856-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="93856-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="93856-120">Request headers</span></span>
|<span data-ttu-id="93856-121">Header</span><span class="sxs-lookup"><span data-stu-id="93856-121">Header</span></span>|<span data-ttu-id="93856-122">Wert</span><span class="sxs-lookup"><span data-stu-id="93856-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93856-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="93856-123">Authorization</span></span>|<span data-ttu-id="93856-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="93856-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93856-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="93856-125">Accept</span></span>|<span data-ttu-id="93856-126">application/json</span><span class="sxs-lookup"><span data-stu-id="93856-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93856-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="93856-127">Request body</span></span>
<span data-ttu-id="93856-128">Geben Sie im Textkörper Anforderung für das Objekt [MacOSLobApp](../resources/intune-apps-macoslobapp.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="93856-128">In the request body, supply a JSON representation for the [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

<span data-ttu-id="93856-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [MacOSLobApp](../resources/intune-apps-macoslobapp.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="93856-129">The following table shows the properties that are required when you create the [macOSLobApp](../resources/intune-apps-macoslobapp.md).</span></span>

|<span data-ttu-id="93856-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="93856-130">Property</span></span>|<span data-ttu-id="93856-131">Typ</span><span class="sxs-lookup"><span data-stu-id="93856-131">Type</span></span>|<span data-ttu-id="93856-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="93856-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93856-133">id</span><span class="sxs-lookup"><span data-stu-id="93856-133">id</span></span>|<span data-ttu-id="93856-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93856-134">String</span></span>|<span data-ttu-id="93856-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="93856-135">Key of the entity.</span></span> <span data-ttu-id="93856-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="93856-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93856-137">displayName</span><span class="sxs-lookup"><span data-stu-id="93856-137">displayName</span></span>|<span data-ttu-id="93856-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93856-138">String</span></span>|<span data-ttu-id="93856-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="93856-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="93856-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="93856-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93856-141">description</span><span class="sxs-lookup"><span data-stu-id="93856-141">description</span></span>|<span data-ttu-id="93856-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93856-142">String</span></span>|<span data-ttu-id="93856-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="93856-143">The description of the app.</span></span> <span data-ttu-id="93856-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="93856-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93856-145">publisher</span><span class="sxs-lookup"><span data-stu-id="93856-145">publisher</span></span>|<span data-ttu-id="93856-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93856-146">String</span></span>|<span data-ttu-id="93856-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="93856-147">The publisher of the app.</span></span> <span data-ttu-id="93856-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="93856-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93856-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="93856-149">largeIcon</span></span>|[<span data-ttu-id="93856-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="93856-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="93856-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="93856-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="93856-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="93856-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93856-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="93856-153">createdDateTime</span></span>|<span data-ttu-id="93856-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93856-154">DateTimeOffset</span></span>|<span data-ttu-id="93856-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="93856-155">The date and time the app was created.</span></span> <span data-ttu-id="93856-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="93856-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93856-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="93856-157">lastModifiedDateTime</span></span>|<span data-ttu-id="93856-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93856-158">DateTimeOffset</span></span>|<span data-ttu-id="93856-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="93856-159">The date and time the app was last modified.</span></span> <span data-ttu-id="93856-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="93856-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93856-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="93856-161">isFeatured</span></span>|<span data-ttu-id="93856-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="93856-162">Boolean</span></span>|<span data-ttu-id="93856-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="93856-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93856-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="93856-164">privacyInformationUrl</span></span>|<span data-ttu-id="93856-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93856-165">String</span></span>|<span data-ttu-id="93856-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="93856-166">The privacy statement Url.</span></span> <span data-ttu-id="93856-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="93856-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93856-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="93856-168">informationUrl</span></span>|<span data-ttu-id="93856-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93856-169">String</span></span>|<span data-ttu-id="93856-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="93856-170">The more information Url.</span></span> <span data-ttu-id="93856-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="93856-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93856-172">owner</span><span class="sxs-lookup"><span data-stu-id="93856-172">owner</span></span>|<span data-ttu-id="93856-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93856-173">String</span></span>|<span data-ttu-id="93856-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="93856-174">The owner of the app.</span></span> <span data-ttu-id="93856-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="93856-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93856-176">developer</span><span class="sxs-lookup"><span data-stu-id="93856-176">developer</span></span>|<span data-ttu-id="93856-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93856-177">String</span></span>|<span data-ttu-id="93856-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="93856-178">The developer of the app.</span></span> <span data-ttu-id="93856-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="93856-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93856-180">notes</span><span class="sxs-lookup"><span data-stu-id="93856-180">notes</span></span>|<span data-ttu-id="93856-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93856-181">String</span></span>|<span data-ttu-id="93856-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="93856-182">Notes for the app.</span></span> <span data-ttu-id="93856-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="93856-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93856-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="93856-184">uploadState</span></span>|<span data-ttu-id="93856-185">Int32</span><span class="sxs-lookup"><span data-stu-id="93856-185">Int32</span></span>|<span data-ttu-id="93856-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="93856-186">The upload state.</span></span> <span data-ttu-id="93856-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="93856-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93856-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="93856-188">publishingState</span></span>|[<span data-ttu-id="93856-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="93856-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="93856-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="93856-190">The publishing state for the app.</span></span> <span data-ttu-id="93856-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="93856-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="93856-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="93856-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="93856-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="93856-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="93856-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="93856-194">isAssigned</span></span>|<span data-ttu-id="93856-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="93856-195">Boolean</span></span>|<span data-ttu-id="93856-196">Der Wert, der angibt, ob die app mindestens eine Gruppe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="93856-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="93856-197">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="93856-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93856-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="93856-198">roleScopeTagIds</span></span>|<span data-ttu-id="93856-199">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="93856-199">String collection</span></span>|<span data-ttu-id="93856-200">Liste der Bereichs-Tag-Ids für diese mobile app.</span><span class="sxs-lookup"><span data-stu-id="93856-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="93856-201">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="93856-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93856-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="93856-202">committedContentVersion</span></span>|<span data-ttu-id="93856-203">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93856-203">String</span></span>|<span data-ttu-id="93856-204">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="93856-204">The internal committed content version.</span></span> <span data-ttu-id="93856-205">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="93856-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="93856-206">fileName</span><span class="sxs-lookup"><span data-stu-id="93856-206">fileName</span></span>|<span data-ttu-id="93856-207">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93856-207">String</span></span>|<span data-ttu-id="93856-208">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="93856-208">The name of the main Lob application file.</span></span> <span data-ttu-id="93856-209">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="93856-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="93856-210">size</span><span class="sxs-lookup"><span data-stu-id="93856-210">size</span></span>|<span data-ttu-id="93856-211">Int64</span><span class="sxs-lookup"><span data-stu-id="93856-211">Int64</span></span>|<span data-ttu-id="93856-212">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="93856-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="93856-213">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="93856-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="93856-214">bundleId</span><span class="sxs-lookup"><span data-stu-id="93856-214">bundleId</span></span>|<span data-ttu-id="93856-215">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93856-215">String</span></span>|<span data-ttu-id="93856-216">Die Paket-Id.</span><span class="sxs-lookup"><span data-stu-id="93856-216">The bundle id.</span></span>|
|<span data-ttu-id="93856-217">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="93856-217">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="93856-218">macOSMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="93856-218">macOSMinimumOperatingSystem</span></span>](../resources/intune-apps-macosminimumoperatingsystem.md)|<span data-ttu-id="93856-219">Wert, der angibt, welche Betriebssystemversion mindestens erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="93856-219">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="93856-220">buildNumber</span><span class="sxs-lookup"><span data-stu-id="93856-220">buildNumber</span></span>|<span data-ttu-id="93856-221">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93856-221">String</span></span>|<span data-ttu-id="93856-222">Die Buildnummer der Mac OS-Zeile des Business (LoB) app.</span><span class="sxs-lookup"><span data-stu-id="93856-222">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="93856-223">versionNumber</span><span class="sxs-lookup"><span data-stu-id="93856-223">versionNumber</span></span>|<span data-ttu-id="93856-224">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93856-224">String</span></span>|<span data-ttu-id="93856-225">Die Versionsnummer der Mac OS-Zeile des Business (LoB) app.</span><span class="sxs-lookup"><span data-stu-id="93856-225">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="93856-226">childApps</span><span class="sxs-lookup"><span data-stu-id="93856-226">childApps</span></span>|<span data-ttu-id="93856-227">[MacOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="93856-227">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="93856-228">Die Liste der von Apps in diesem Paket bundle</span><span class="sxs-lookup"><span data-stu-id="93856-228">The app list in this bundle package</span></span>|
|<span data-ttu-id="93856-229">identityVersion</span><span class="sxs-lookup"><span data-stu-id="93856-229">identityVersion</span></span>|<span data-ttu-id="93856-230">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="93856-230">String</span></span>|<span data-ttu-id="93856-231">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="93856-231">The identity version.</span></span>|
|<span data-ttu-id="93856-232">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="93856-232">md5HashChunkSize</span></span>|<span data-ttu-id="93856-233">Int32</span><span class="sxs-lookup"><span data-stu-id="93856-233">Int32</span></span>|<span data-ttu-id="93856-234">Die Chunk-Size für MD5-hash</span><span class="sxs-lookup"><span data-stu-id="93856-234">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="93856-235">md5Hash</span><span class="sxs-lookup"><span data-stu-id="93856-235">md5Hash</span></span>|<span data-ttu-id="93856-236">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="93856-236">String collection</span></span>|<span data-ttu-id="93856-237">Die MD5-Hash-codes</span><span class="sxs-lookup"><span data-stu-id="93856-237">The MD5 hash codes</span></span>|
|<span data-ttu-id="93856-238">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="93856-238">ignoreVersionDetection</span></span>|<span data-ttu-id="93856-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="93856-239">Boolean</span></span>|<span data-ttu-id="93856-240">Boolescher Wert, der steuert, ob nach der Installation der App auf einem Gerät die App-Version zur Erkennung der App verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="93856-240">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="93856-241">Legen Sie dies für Mac OS Line of Business (LoB) apps "true", die ein Updatefeature Self zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="93856-241">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="93856-242">Antwort</span><span class="sxs-lookup"><span data-stu-id="93856-242">Response</span></span>
<span data-ttu-id="93856-243">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [MacOSLobApp](../resources/intune-apps-macoslobapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="93856-243">If successful, this method returns a `200 OK` response code and an updated [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93856-244">Beispiel</span><span class="sxs-lookup"><span data-stu-id="93856-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="93856-245">Anforderung</span><span class="sxs-lookup"><span data-stu-id="93856-245">Request</span></span>
<span data-ttu-id="93856-246">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="93856-246">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1547

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="93856-247">Antwort</span><span class="sxs-lookup"><span data-stu-id="93856-247">Response</span></span>
<span data-ttu-id="93856-p123">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="93856-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1719

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
  "id": "7be9250a-250a-7be9-0a25-e97b0a25e97b",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```




