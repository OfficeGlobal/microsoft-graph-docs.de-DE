---
title: Win32LobApp aktualisieren
description: Aktualisieren der Eigenschaften eines win32LobApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4b0a8b44b42cdcc53118d6be7463050ea910d63
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150120"
---
# <a name="update-win32lobapp"></a><span data-ttu-id="bc207-103">Win32LobApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="bc207-103">Update win32LobApp</span></span>

> <span data-ttu-id="bc207-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bc207-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc207-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="bc207-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc207-106">Aktualisieren der Eigenschaften eines [win32LobApp](../resources/intune-apps-win32lobapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="bc207-106">Update the properties of a [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc207-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bc207-107">Prerequisites</span></span>
<span data-ttu-id="bc207-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bc207-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bc207-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bc207-110">Permission type</span></span>|<span data-ttu-id="bc207-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bc207-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc207-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bc207-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bc207-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc207-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bc207-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bc207-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc207-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bc207-115">Not supported.</span></span>|
|<span data-ttu-id="bc207-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bc207-116">Application</span></span>|<span data-ttu-id="bc207-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bc207-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc207-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc207-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="bc207-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bc207-119">Request headers</span></span>
|<span data-ttu-id="bc207-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bc207-120">Header</span></span>|<span data-ttu-id="bc207-121">Wert</span><span class="sxs-lookup"><span data-stu-id="bc207-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc207-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc207-122">Authorization</span></span>|<span data-ttu-id="bc207-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc207-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc207-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bc207-124">Accept</span></span>|<span data-ttu-id="bc207-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bc207-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc207-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bc207-126">Request body</span></span>
<span data-ttu-id="bc207-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [win32LobApp](../resources/intune-apps-win32lobapp.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="bc207-127">In the request body, supply a JSON representation for the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

<span data-ttu-id="bc207-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [win32LobApp](../resources/intune-apps-win32lobapp.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="bc207-128">The following table shows the properties that are required when you create the [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

|<span data-ttu-id="bc207-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bc207-129">Property</span></span>|<span data-ttu-id="bc207-130">Typ</span><span class="sxs-lookup"><span data-stu-id="bc207-130">Type</span></span>|<span data-ttu-id="bc207-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc207-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc207-132">id</span><span class="sxs-lookup"><span data-stu-id="bc207-132">id</span></span>|<span data-ttu-id="bc207-133">string</span><span class="sxs-lookup"><span data-stu-id="bc207-133">String</span></span>|<span data-ttu-id="bc207-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="bc207-134">Key of the entity.</span></span> <span data-ttu-id="bc207-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc207-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc207-136">displayName</span><span class="sxs-lookup"><span data-stu-id="bc207-136">displayName</span></span>|<span data-ttu-id="bc207-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc207-137">String</span></span>|<span data-ttu-id="bc207-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="bc207-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="bc207-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc207-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc207-140">description</span><span class="sxs-lookup"><span data-stu-id="bc207-140">description</span></span>|<span data-ttu-id="bc207-141">String</span><span class="sxs-lookup"><span data-stu-id="bc207-141">String</span></span>|<span data-ttu-id="bc207-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="bc207-142">The description of the app.</span></span> <span data-ttu-id="bc207-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc207-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc207-144">publisher</span><span class="sxs-lookup"><span data-stu-id="bc207-144">publisher</span></span>|<span data-ttu-id="bc207-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc207-145">String</span></span>|<span data-ttu-id="bc207-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="bc207-146">The publisher of the app.</span></span> <span data-ttu-id="bc207-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc207-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc207-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="bc207-148">largeIcon</span></span>|[<span data-ttu-id="bc207-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bc207-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="bc207-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="bc207-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="bc207-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc207-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc207-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc207-152">createdDateTime</span></span>|<span data-ttu-id="bc207-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc207-153">DateTimeOffset</span></span>|<span data-ttu-id="bc207-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="bc207-154">The date and time the app was created.</span></span> <span data-ttu-id="bc207-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc207-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc207-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc207-156">lastModifiedDateTime</span></span>|<span data-ttu-id="bc207-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc207-157">DateTimeOffset</span></span>|<span data-ttu-id="bc207-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="bc207-158">The date and time the app was last modified.</span></span> <span data-ttu-id="bc207-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc207-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc207-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="bc207-160">isFeatured</span></span>|<span data-ttu-id="bc207-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bc207-161">Boolean</span></span>|<span data-ttu-id="bc207-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc207-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc207-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="bc207-163">privacyInformationUrl</span></span>|<span data-ttu-id="bc207-164">String</span><span class="sxs-lookup"><span data-stu-id="bc207-164">String</span></span>|<span data-ttu-id="bc207-165">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="bc207-165">The privacy statement Url.</span></span> <span data-ttu-id="bc207-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc207-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc207-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="bc207-167">informationUrl</span></span>|<span data-ttu-id="bc207-168">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc207-168">String</span></span>|<span data-ttu-id="bc207-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="bc207-169">The more information Url.</span></span> <span data-ttu-id="bc207-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc207-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc207-171">owner</span><span class="sxs-lookup"><span data-stu-id="bc207-171">owner</span></span>|<span data-ttu-id="bc207-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc207-172">String</span></span>|<span data-ttu-id="bc207-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="bc207-173">The owner of the app.</span></span> <span data-ttu-id="bc207-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc207-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc207-175">developer</span><span class="sxs-lookup"><span data-stu-id="bc207-175">developer</span></span>|<span data-ttu-id="bc207-176">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc207-176">String</span></span>|<span data-ttu-id="bc207-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="bc207-177">The developer of the app.</span></span> <span data-ttu-id="bc207-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc207-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc207-179">notes</span><span class="sxs-lookup"><span data-stu-id="bc207-179">notes</span></span>|<span data-ttu-id="bc207-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc207-180">String</span></span>|<span data-ttu-id="bc207-181">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="bc207-181">Notes for the app.</span></span> <span data-ttu-id="bc207-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc207-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc207-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="bc207-183">uploadState</span></span>|<span data-ttu-id="bc207-184">Int32</span><span class="sxs-lookup"><span data-stu-id="bc207-184">Int32</span></span>|<span data-ttu-id="bc207-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="bc207-185">The upload state.</span></span> <span data-ttu-id="bc207-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc207-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc207-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="bc207-187">publishingState</span></span>|[<span data-ttu-id="bc207-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="bc207-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="bc207-189">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="bc207-189">The publishing state for the app.</span></span> <span data-ttu-id="bc207-190">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="bc207-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="bc207-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="bc207-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="bc207-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="bc207-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="bc207-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="bc207-193">isAssigned</span></span>|<span data-ttu-id="bc207-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc207-194">Boolean</span></span>|<span data-ttu-id="bc207-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="bc207-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="bc207-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc207-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc207-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="bc207-197">roleScopeTagIds</span></span>|<span data-ttu-id="bc207-198">String collection</span><span class="sxs-lookup"><span data-stu-id="bc207-198">String collection</span></span>|<span data-ttu-id="bc207-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="bc207-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="bc207-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc207-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bc207-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="bc207-201">committedContentVersion</span></span>|<span data-ttu-id="bc207-202">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc207-202">String</span></span>|<span data-ttu-id="bc207-203">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="bc207-203">The internal committed content version.</span></span> <span data-ttu-id="bc207-204">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc207-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="bc207-205">fileName</span><span class="sxs-lookup"><span data-stu-id="bc207-205">fileName</span></span>|<span data-ttu-id="bc207-206">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc207-206">String</span></span>|<span data-ttu-id="bc207-207">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="bc207-207">The name of the main Lob application file.</span></span> <span data-ttu-id="bc207-208">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc207-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="bc207-209">size</span><span class="sxs-lookup"><span data-stu-id="bc207-209">size</span></span>|<span data-ttu-id="bc207-210">Int64</span><span class="sxs-lookup"><span data-stu-id="bc207-210">Int64</span></span>|<span data-ttu-id="bc207-211">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="bc207-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="bc207-212">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc207-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="bc207-213">InstallCommandLine:</span><span class="sxs-lookup"><span data-stu-id="bc207-213">installCommandLine</span></span>|<span data-ttu-id="bc207-214">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc207-214">String</span></span>|<span data-ttu-id="bc207-215">Die Befehlszeile zum Installieren dieser APP</span><span class="sxs-lookup"><span data-stu-id="bc207-215">The command line to install this app</span></span>|
|<span data-ttu-id="bc207-216">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="bc207-216">uninstallCommandLine</span></span>|<span data-ttu-id="bc207-217">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc207-217">String</span></span>|<span data-ttu-id="bc207-218">Die Befehlszeile zum Deinstallieren dieser APP</span><span class="sxs-lookup"><span data-stu-id="bc207-218">The command line to uninstall this app</span></span>|
|<span data-ttu-id="bc207-219">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="bc207-219">applicableArchitectures</span></span>|[<span data-ttu-id="bc207-220">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="bc207-220">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="bc207-221">Die Windows-Architekturen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="bc207-221">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="bc207-222">Mögliche Werte sind: `none`, `x86`, `x64`, `arm`, `neutral` und `arm64`.</span><span class="sxs-lookup"><span data-stu-id="bc207-222">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="bc207-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bc207-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="bc207-224">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bc207-224">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="bc207-225">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="bc207-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="bc207-226">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="bc207-226">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="bc207-227">Int32</span><span class="sxs-lookup"><span data-stu-id="bc207-227">Int32</span></span>|<span data-ttu-id="bc207-228">Der Wert für den minimalen freien Speicherplatz, der erforderlich ist, um diese APP zu installieren.</span><span class="sxs-lookup"><span data-stu-id="bc207-228">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="bc207-229">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="bc207-229">minimumMemoryInMB</span></span>|<span data-ttu-id="bc207-230">Int32</span><span class="sxs-lookup"><span data-stu-id="bc207-230">Int32</span></span>|<span data-ttu-id="bc207-231">Der Wert für den minimalen physischen Arbeitsspeicher, der für die Installation dieser APP erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="bc207-231">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="bc207-232">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="bc207-232">minimumNumberOfProcessors</span></span>|<span data-ttu-id="bc207-233">Int32</span><span class="sxs-lookup"><span data-stu-id="bc207-233">Int32</span></span>|<span data-ttu-id="bc207-234">Der Wert für die Mindestanzahl von Prozessoren, die zum Installieren dieser APP erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="bc207-234">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="bc207-235">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="bc207-235">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="bc207-236">Int32</span><span class="sxs-lookup"><span data-stu-id="bc207-236">Int32</span></span>|<span data-ttu-id="bc207-237">Der Wert für die minimale CPU-Geschwindigkeit, die erforderlich ist, um diese APP zu installieren.</span><span class="sxs-lookup"><span data-stu-id="bc207-237">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="bc207-238">detectionRules</span><span class="sxs-lookup"><span data-stu-id="bc207-238">detectionRules</span></span>|<span data-ttu-id="bc207-239">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="bc207-239">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="bc207-240">Die Erkennungsregeln zum Erkennen der Win32-Branchen-app.</span><span class="sxs-lookup"><span data-stu-id="bc207-240">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="bc207-241">installExperience</span><span class="sxs-lookup"><span data-stu-id="bc207-241">installExperience</span></span>|[<span data-ttu-id="bc207-242">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="bc207-242">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="bc207-243">Die Installationsumgebung für diese APP.</span><span class="sxs-lookup"><span data-stu-id="bc207-243">The install experience for this app.</span></span>|
|<span data-ttu-id="bc207-244">returnCodes</span><span class="sxs-lookup"><span data-stu-id="bc207-244">returnCodes</span></span>|<span data-ttu-id="bc207-245">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="bc207-245">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="bc207-246">Die Rückgabecodes für das Verhalten nach der Installation.</span><span class="sxs-lookup"><span data-stu-id="bc207-246">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="bc207-247">msiInformation</span><span class="sxs-lookup"><span data-stu-id="bc207-247">msiInformation</span></span>|[<span data-ttu-id="bc207-248">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="bc207-248">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="bc207-249">Die MSI-Details, wenn diese Win32-App eine MSI-APP ist.</span><span class="sxs-lookup"><span data-stu-id="bc207-249">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="bc207-250">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="bc207-250">setupFilePath</span></span>|<span data-ttu-id="bc207-251">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc207-251">String</span></span>|<span data-ttu-id="bc207-252">Der relative Pfad der Setupdatei im verschlüsselten Win32LobApp-Paket.</span><span class="sxs-lookup"><span data-stu-id="bc207-252">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|



## <a name="response"></a><span data-ttu-id="bc207-253">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc207-253">Response</span></span>
<span data-ttu-id="bc207-254">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [win32LobApp](../resources/intune-apps-win32lobapp.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bc207-254">If successful, this method returns a `200 OK` response code and an updated [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc207-255">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bc207-255">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc207-256">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc207-256">Request</span></span>
<span data-ttu-id="bc207-257">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bc207-257">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2364

{
  "@odata.type": "#microsoft.graph.win32LobApp",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value"
}
```

### <a name="response"></a><span data-ttu-id="bc207-258">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc207-258">Response</span></span>
<span data-ttu-id="bc207-p122">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bc207-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2536

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "9607b530-b530-9607-30b5-079630b50796",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value"
}
```




