---
title: Win32LobApp erstellen
description: Erstellen eines neuen win32LobApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a945b6118c016cfa93cd1ea87958718f60bd2ea4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958543"
---
# <a name="create-win32lobapp"></a><span data-ttu-id="71c4f-103">Win32LobApp erstellen</span><span class="sxs-lookup"><span data-stu-id="71c4f-103">Create win32LobApp</span></span>

> <span data-ttu-id="71c4f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="71c4f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71c4f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="71c4f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71c4f-106">Erstellen eines neuen [win32LobApp](../resources/intune-apps-win32lobapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="71c4f-106">Create a new [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71c4f-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="71c4f-107">Prerequisites</span></span>
<span data-ttu-id="71c4f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71c4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71c4f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="71c4f-110">Permission type</span></span>|<span data-ttu-id="71c4f-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="71c4f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71c4f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="71c4f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="71c4f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71c4f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="71c4f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="71c4f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71c4f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71c4f-115">Not supported.</span></span>|
|<span data-ttu-id="71c4f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="71c4f-116">Application</span></span>|<span data-ttu-id="71c4f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="71c4f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71c4f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="71c4f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="71c4f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="71c4f-119">Request headers</span></span>
|<span data-ttu-id="71c4f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="71c4f-120">Header</span></span>|<span data-ttu-id="71c4f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="71c4f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71c4f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="71c4f-122">Authorization</span></span>|<span data-ttu-id="71c4f-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="71c4f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71c4f-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="71c4f-124">Accept</span></span>|<span data-ttu-id="71c4f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="71c4f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71c4f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="71c4f-126">Request body</span></span>
<span data-ttu-id="71c4f-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das win32LobApp-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="71c4f-127">In the request body, supply a JSON representation for the win32LobApp object.</span></span>

<span data-ttu-id="71c4f-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der win32LobApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="71c4f-128">The following table shows the properties that are required when you create the win32LobApp.</span></span>

|<span data-ttu-id="71c4f-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="71c4f-129">Property</span></span>|<span data-ttu-id="71c4f-130">Typ</span><span class="sxs-lookup"><span data-stu-id="71c4f-130">Type</span></span>|<span data-ttu-id="71c4f-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71c4f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71c4f-132">id</span><span class="sxs-lookup"><span data-stu-id="71c4f-132">id</span></span>|<span data-ttu-id="71c4f-133">String</span><span class="sxs-lookup"><span data-stu-id="71c4f-133">String</span></span>|<span data-ttu-id="71c4f-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="71c4f-134">Key of the entity.</span></span> <span data-ttu-id="71c4f-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71c4f-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71c4f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="71c4f-136">displayName</span></span>|<span data-ttu-id="71c4f-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="71c4f-137">String</span></span>|<span data-ttu-id="71c4f-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="71c4f-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="71c4f-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71c4f-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71c4f-140">description</span><span class="sxs-lookup"><span data-stu-id="71c4f-140">description</span></span>|<span data-ttu-id="71c4f-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="71c4f-141">String</span></span>|<span data-ttu-id="71c4f-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="71c4f-142">The description of the app.</span></span> <span data-ttu-id="71c4f-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71c4f-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71c4f-144">publisher</span><span class="sxs-lookup"><span data-stu-id="71c4f-144">publisher</span></span>|<span data-ttu-id="71c4f-145">String</span><span class="sxs-lookup"><span data-stu-id="71c4f-145">String</span></span>|<span data-ttu-id="71c4f-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="71c4f-146">The publisher of the app.</span></span> <span data-ttu-id="71c4f-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71c4f-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71c4f-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="71c4f-148">largeIcon</span></span>|[<span data-ttu-id="71c4f-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="71c4f-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="71c4f-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="71c4f-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="71c4f-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71c4f-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71c4f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71c4f-152">createdDateTime</span></span>|<span data-ttu-id="71c4f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71c4f-153">DateTimeOffset</span></span>|<span data-ttu-id="71c4f-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="71c4f-154">The date and time the app was created.</span></span> <span data-ttu-id="71c4f-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71c4f-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71c4f-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71c4f-156">lastModifiedDateTime</span></span>|<span data-ttu-id="71c4f-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71c4f-157">DateTimeOffset</span></span>|<span data-ttu-id="71c4f-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="71c4f-158">The date and time the app was last modified.</span></span> <span data-ttu-id="71c4f-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71c4f-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71c4f-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="71c4f-160">isFeatured</span></span>|<span data-ttu-id="71c4f-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="71c4f-161">Boolean</span></span>|<span data-ttu-id="71c4f-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71c4f-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71c4f-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="71c4f-163">privacyInformationUrl</span></span>|<span data-ttu-id="71c4f-164">String</span><span class="sxs-lookup"><span data-stu-id="71c4f-164">String</span></span>|<span data-ttu-id="71c4f-165">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="71c4f-165">The privacy statement Url.</span></span> <span data-ttu-id="71c4f-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71c4f-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71c4f-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="71c4f-167">informationUrl</span></span>|<span data-ttu-id="71c4f-168">String</span><span class="sxs-lookup"><span data-stu-id="71c4f-168">String</span></span>|<span data-ttu-id="71c4f-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="71c4f-169">The more information Url.</span></span> <span data-ttu-id="71c4f-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71c4f-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71c4f-171">owner</span><span class="sxs-lookup"><span data-stu-id="71c4f-171">owner</span></span>|<span data-ttu-id="71c4f-172">String</span><span class="sxs-lookup"><span data-stu-id="71c4f-172">String</span></span>|<span data-ttu-id="71c4f-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="71c4f-173">The owner of the app.</span></span> <span data-ttu-id="71c4f-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71c4f-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71c4f-175">developer</span><span class="sxs-lookup"><span data-stu-id="71c4f-175">developer</span></span>|<span data-ttu-id="71c4f-176">String</span><span class="sxs-lookup"><span data-stu-id="71c4f-176">String</span></span>|<span data-ttu-id="71c4f-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="71c4f-177">The developer of the app.</span></span> <span data-ttu-id="71c4f-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71c4f-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71c4f-179">notes</span><span class="sxs-lookup"><span data-stu-id="71c4f-179">notes</span></span>|<span data-ttu-id="71c4f-180">String</span><span class="sxs-lookup"><span data-stu-id="71c4f-180">String</span></span>|<span data-ttu-id="71c4f-181">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="71c4f-181">Notes for the app.</span></span> <span data-ttu-id="71c4f-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71c4f-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71c4f-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="71c4f-183">uploadState</span></span>|<span data-ttu-id="71c4f-184">Int32</span><span class="sxs-lookup"><span data-stu-id="71c4f-184">Int32</span></span>|<span data-ttu-id="71c4f-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="71c4f-185">The upload state.</span></span> <span data-ttu-id="71c4f-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71c4f-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71c4f-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="71c4f-187">publishingState</span></span>|[<span data-ttu-id="71c4f-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="71c4f-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="71c4f-189">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="71c4f-189">The publishing state for the app.</span></span> <span data-ttu-id="71c4f-190">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="71c4f-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="71c4f-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="71c4f-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="71c4f-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="71c4f-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="71c4f-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="71c4f-193">isAssigned</span></span>|<span data-ttu-id="71c4f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="71c4f-194">Boolean</span></span>|<span data-ttu-id="71c4f-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="71c4f-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="71c4f-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71c4f-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71c4f-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="71c4f-197">roleScopeTagIds</span></span>|<span data-ttu-id="71c4f-198">String collection</span><span class="sxs-lookup"><span data-stu-id="71c4f-198">String collection</span></span>|<span data-ttu-id="71c4f-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="71c4f-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="71c4f-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71c4f-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71c4f-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="71c4f-201">committedContentVersion</span></span>|<span data-ttu-id="71c4f-202">String</span><span class="sxs-lookup"><span data-stu-id="71c4f-202">String</span></span>|<span data-ttu-id="71c4f-203">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="71c4f-203">The internal committed content version.</span></span> <span data-ttu-id="71c4f-204">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="71c4f-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="71c4f-205">fileName</span><span class="sxs-lookup"><span data-stu-id="71c4f-205">fileName</span></span>|<span data-ttu-id="71c4f-206">String</span><span class="sxs-lookup"><span data-stu-id="71c4f-206">String</span></span>|<span data-ttu-id="71c4f-207">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="71c4f-207">The name of the main Lob application file.</span></span> <span data-ttu-id="71c4f-208">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="71c4f-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="71c4f-209">size</span><span class="sxs-lookup"><span data-stu-id="71c4f-209">size</span></span>|<span data-ttu-id="71c4f-210">Int64</span><span class="sxs-lookup"><span data-stu-id="71c4f-210">Int64</span></span>|<span data-ttu-id="71c4f-211">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="71c4f-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="71c4f-212">Geerbt von [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="71c4f-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="71c4f-213">InstallCommandLine:</span><span class="sxs-lookup"><span data-stu-id="71c4f-213">installCommandLine</span></span>|<span data-ttu-id="71c4f-214">String</span><span class="sxs-lookup"><span data-stu-id="71c4f-214">String</span></span>|<span data-ttu-id="71c4f-215">Die Befehlszeile zum Installieren dieser APP</span><span class="sxs-lookup"><span data-stu-id="71c4f-215">The command line to install this app</span></span>|
|<span data-ttu-id="71c4f-216">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="71c4f-216">uninstallCommandLine</span></span>|<span data-ttu-id="71c4f-217">String</span><span class="sxs-lookup"><span data-stu-id="71c4f-217">String</span></span>|<span data-ttu-id="71c4f-218">Die Befehlszeile zum Deinstallieren dieser APP</span><span class="sxs-lookup"><span data-stu-id="71c4f-218">The command line to uninstall this app</span></span>|
|<span data-ttu-id="71c4f-219">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="71c4f-219">applicableArchitectures</span></span>|[<span data-ttu-id="71c4f-220">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="71c4f-220">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="71c4f-221">Die Windows-Architekturen, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="71c4f-221">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="71c4f-222">Mögliche Werte sind: `none`, `x86`, `x64`, `arm`, `neutral` und `arm64`.</span><span class="sxs-lookup"><span data-stu-id="71c4f-222">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="71c4f-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="71c4f-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="71c4f-224">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="71c4f-224">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="71c4f-225">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="71c4f-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="71c4f-226">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="71c4f-226">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="71c4f-227">Int32</span><span class="sxs-lookup"><span data-stu-id="71c4f-227">Int32</span></span>|<span data-ttu-id="71c4f-228">Der Wert für den minimalen freien Speicherplatz, der erforderlich ist, um diese APP zu installieren.</span><span class="sxs-lookup"><span data-stu-id="71c4f-228">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="71c4f-229">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="71c4f-229">minimumMemoryInMB</span></span>|<span data-ttu-id="71c4f-230">Int32</span><span class="sxs-lookup"><span data-stu-id="71c4f-230">Int32</span></span>|<span data-ttu-id="71c4f-231">Der Wert für den minimalen physischen Arbeitsspeicher, der für die Installation dieser APP erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="71c4f-231">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="71c4f-232">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="71c4f-232">minimumNumberOfProcessors</span></span>|<span data-ttu-id="71c4f-233">Int32</span><span class="sxs-lookup"><span data-stu-id="71c4f-233">Int32</span></span>|<span data-ttu-id="71c4f-234">Der Wert für die Mindestanzahl von Prozessoren, die zum Installieren dieser APP erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="71c4f-234">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="71c4f-235">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="71c4f-235">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="71c4f-236">Int32</span><span class="sxs-lookup"><span data-stu-id="71c4f-236">Int32</span></span>|<span data-ttu-id="71c4f-237">Der Wert für die minimale CPU-Geschwindigkeit, die erforderlich ist, um diese APP zu installieren.</span><span class="sxs-lookup"><span data-stu-id="71c4f-237">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="71c4f-238">detectionRules</span><span class="sxs-lookup"><span data-stu-id="71c4f-238">detectionRules</span></span>|<span data-ttu-id="71c4f-239">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="71c4f-239">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="71c4f-240">Die Erkennungsregeln zum Erkennen der Win32-Branchen-app.</span><span class="sxs-lookup"><span data-stu-id="71c4f-240">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="71c4f-241">installExperience</span><span class="sxs-lookup"><span data-stu-id="71c4f-241">installExperience</span></span>|[<span data-ttu-id="71c4f-242">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="71c4f-242">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="71c4f-243">Die Installationsumgebung für diese APP.</span><span class="sxs-lookup"><span data-stu-id="71c4f-243">The install experience for this app.</span></span>|
|<span data-ttu-id="71c4f-244">returnCodes</span><span class="sxs-lookup"><span data-stu-id="71c4f-244">returnCodes</span></span>|<span data-ttu-id="71c4f-245">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="71c4f-245">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="71c4f-246">Die Rückgabecodes für das Verhalten nach der Installation.</span><span class="sxs-lookup"><span data-stu-id="71c4f-246">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="71c4f-247">msiInformation</span><span class="sxs-lookup"><span data-stu-id="71c4f-247">msiInformation</span></span>|[<span data-ttu-id="71c4f-248">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="71c4f-248">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="71c4f-249">Die MSI-Details, wenn diese Win32-App eine MSI-APP ist.</span><span class="sxs-lookup"><span data-stu-id="71c4f-249">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="71c4f-250">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="71c4f-250">setupFilePath</span></span>|<span data-ttu-id="71c4f-251">String</span><span class="sxs-lookup"><span data-stu-id="71c4f-251">String</span></span>|<span data-ttu-id="71c4f-252">Der relative Pfad der Setupdatei im verschlüsselten Win32LobApp-Paket.</span><span class="sxs-lookup"><span data-stu-id="71c4f-252">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|



## <a name="response"></a><span data-ttu-id="71c4f-253">Antwort</span><span class="sxs-lookup"><span data-stu-id="71c4f-253">Response</span></span>
<span data-ttu-id="71c4f-254">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [win32LobApp](../resources/intune-apps-win32lobapp.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="71c4f-254">If successful, this method returns a `201 Created` response code and a [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71c4f-255">Beispiel</span><span class="sxs-lookup"><span data-stu-id="71c4f-255">Example</span></span>

### <a name="request"></a><span data-ttu-id="71c4f-256">Anforderung</span><span class="sxs-lookup"><span data-stu-id="71c4f-256">Request</span></span>
<span data-ttu-id="71c4f-257">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="71c4f-257">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="71c4f-258">Antwort</span><span class="sxs-lookup"><span data-stu-id="71c4f-258">Response</span></span>
<span data-ttu-id="71c4f-p122">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="71c4f-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




