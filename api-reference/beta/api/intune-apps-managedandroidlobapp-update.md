---
title: managedAndroidLobApp aktualisieren
description: Aktualisieren der Eigenschaften eines managedAndroidLobApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a9d52be650851240639fdbdedd4dbccee57d0f87
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958081"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="e4166-103">managedAndroidLobApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e4166-103">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="e4166-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e4166-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4166-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e4166-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4166-106">Aktualisieren der Eigenschaften eines [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e4166-106">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4166-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e4166-107">Prerequisites</span></span>
<span data-ttu-id="e4166-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4166-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4166-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e4166-110">Permission type</span></span>|<span data-ttu-id="e4166-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e4166-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4166-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e4166-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e4166-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4166-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e4166-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e4166-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4166-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4166-115">Not supported.</span></span>|
|<span data-ttu-id="e4166-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e4166-116">Application</span></span>|<span data-ttu-id="e4166-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4166-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4166-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4166-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="e4166-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e4166-119">Request headers</span></span>
|<span data-ttu-id="e4166-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e4166-120">Header</span></span>|<span data-ttu-id="e4166-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e4166-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4166-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4166-122">Authorization</span></span>|<span data-ttu-id="e4166-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e4166-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4166-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e4166-124">Accept</span></span>|<span data-ttu-id="e4166-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e4166-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4166-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e4166-126">Request body</span></span>
<span data-ttu-id="e4166-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e4166-127">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="e4166-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e4166-128">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="e4166-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e4166-129">Property</span></span>|<span data-ttu-id="e4166-130">Typ</span><span class="sxs-lookup"><span data-stu-id="e4166-130">Type</span></span>|<span data-ttu-id="e4166-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4166-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4166-132">id</span><span class="sxs-lookup"><span data-stu-id="e4166-132">id</span></span>|<span data-ttu-id="e4166-133">String</span><span class="sxs-lookup"><span data-stu-id="e4166-133">String</span></span>|<span data-ttu-id="e4166-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e4166-134">Key of the entity.</span></span> <span data-ttu-id="e4166-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4166-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4166-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e4166-136">displayName</span></span>|<span data-ttu-id="e4166-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4166-137">String</span></span>|<span data-ttu-id="e4166-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="e4166-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e4166-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4166-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4166-140">description</span><span class="sxs-lookup"><span data-stu-id="e4166-140">description</span></span>|<span data-ttu-id="e4166-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4166-141">String</span></span>|<span data-ttu-id="e4166-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="e4166-142">The description of the app.</span></span> <span data-ttu-id="e4166-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4166-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4166-144">publisher</span><span class="sxs-lookup"><span data-stu-id="e4166-144">publisher</span></span>|<span data-ttu-id="e4166-145">String</span><span class="sxs-lookup"><span data-stu-id="e4166-145">String</span></span>|<span data-ttu-id="e4166-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="e4166-146">The publisher of the app.</span></span> <span data-ttu-id="e4166-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4166-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4166-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e4166-148">largeIcon</span></span>|[<span data-ttu-id="e4166-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e4166-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e4166-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="e4166-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e4166-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4166-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4166-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e4166-152">createdDateTime</span></span>|<span data-ttu-id="e4166-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4166-153">DateTimeOffset</span></span>|<span data-ttu-id="e4166-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="e4166-154">The date and time the app was created.</span></span> <span data-ttu-id="e4166-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4166-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4166-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4166-156">lastModifiedDateTime</span></span>|<span data-ttu-id="e4166-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4166-157">DateTimeOffset</span></span>|<span data-ttu-id="e4166-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="e4166-158">The date and time the app was last modified.</span></span> <span data-ttu-id="e4166-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4166-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4166-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e4166-160">isFeatured</span></span>|<span data-ttu-id="e4166-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4166-161">Boolean</span></span>|<span data-ttu-id="e4166-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4166-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4166-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e4166-163">privacyInformationUrl</span></span>|<span data-ttu-id="e4166-164">String</span><span class="sxs-lookup"><span data-stu-id="e4166-164">String</span></span>|<span data-ttu-id="e4166-165">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="e4166-165">The privacy statement Url.</span></span> <span data-ttu-id="e4166-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4166-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4166-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e4166-167">informationUrl</span></span>|<span data-ttu-id="e4166-168">String</span><span class="sxs-lookup"><span data-stu-id="e4166-168">String</span></span>|<span data-ttu-id="e4166-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="e4166-169">The more information Url.</span></span> <span data-ttu-id="e4166-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4166-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4166-171">owner</span><span class="sxs-lookup"><span data-stu-id="e4166-171">owner</span></span>|<span data-ttu-id="e4166-172">String</span><span class="sxs-lookup"><span data-stu-id="e4166-172">String</span></span>|<span data-ttu-id="e4166-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="e4166-173">The owner of the app.</span></span> <span data-ttu-id="e4166-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4166-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4166-175">developer</span><span class="sxs-lookup"><span data-stu-id="e4166-175">developer</span></span>|<span data-ttu-id="e4166-176">String</span><span class="sxs-lookup"><span data-stu-id="e4166-176">String</span></span>|<span data-ttu-id="e4166-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="e4166-177">The developer of the app.</span></span> <span data-ttu-id="e4166-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4166-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4166-179">notes</span><span class="sxs-lookup"><span data-stu-id="e4166-179">notes</span></span>|<span data-ttu-id="e4166-180">String</span><span class="sxs-lookup"><span data-stu-id="e4166-180">String</span></span>|<span data-ttu-id="e4166-181">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="e4166-181">Notes for the app.</span></span> <span data-ttu-id="e4166-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4166-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4166-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="e4166-183">uploadState</span></span>|<span data-ttu-id="e4166-184">Int32</span><span class="sxs-lookup"><span data-stu-id="e4166-184">Int32</span></span>|<span data-ttu-id="e4166-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="e4166-185">The upload state.</span></span> <span data-ttu-id="e4166-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4166-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4166-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="e4166-187">publishingState</span></span>|[<span data-ttu-id="e4166-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e4166-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e4166-189">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="e4166-189">The publishing state for the app.</span></span> <span data-ttu-id="e4166-190">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="e4166-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e4166-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="e4166-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e4166-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="e4166-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e4166-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e4166-193">isAssigned</span></span>|<span data-ttu-id="e4166-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4166-194">Boolean</span></span>|<span data-ttu-id="e4166-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="e4166-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e4166-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4166-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4166-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="e4166-197">roleScopeTagIds</span></span>|<span data-ttu-id="e4166-198">String collection</span><span class="sxs-lookup"><span data-stu-id="e4166-198">String collection</span></span>|<span data-ttu-id="e4166-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="e4166-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e4166-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4166-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4166-201">appAvailability</span><span class="sxs-lookup"><span data-stu-id="e4166-201">appAvailability</span></span>|[<span data-ttu-id="e4166-202">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="e4166-202">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="e4166-203">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="e4166-203">The Application's availability.</span></span> <span data-ttu-id="e4166-204">Von [ManagedApp](../resources/intune-apps-managedapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="e4166-204">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="e4166-205">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="e4166-205">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="e4166-206">version</span><span class="sxs-lookup"><span data-stu-id="e4166-206">version</span></span>|<span data-ttu-id="e4166-207">String</span><span class="sxs-lookup"><span data-stu-id="e4166-207">String</span></span>|<span data-ttu-id="e4166-208">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="e4166-208">The Application's version.</span></span> <span data-ttu-id="e4166-209">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="e4166-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="e4166-210">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e4166-210">committedContentVersion</span></span>|<span data-ttu-id="e4166-211">String</span><span class="sxs-lookup"><span data-stu-id="e4166-211">String</span></span>|<span data-ttu-id="e4166-212">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="e4166-212">The internal committed content version.</span></span> <span data-ttu-id="e4166-213">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4166-213">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e4166-214">fileName</span><span class="sxs-lookup"><span data-stu-id="e4166-214">fileName</span></span>|<span data-ttu-id="e4166-215">String</span><span class="sxs-lookup"><span data-stu-id="e4166-215">String</span></span>|<span data-ttu-id="e4166-216">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="e4166-216">The name of the main Lob application file.</span></span> <span data-ttu-id="e4166-217">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4166-217">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e4166-218">size</span><span class="sxs-lookup"><span data-stu-id="e4166-218">size</span></span>|<span data-ttu-id="e4166-219">Int64</span><span class="sxs-lookup"><span data-stu-id="e4166-219">Int64</span></span>|<span data-ttu-id="e4166-220">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="e4166-220">The total size, including all uploaded files.</span></span> <span data-ttu-id="e4166-221">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4166-221">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e4166-222">packageId</span><span class="sxs-lookup"><span data-stu-id="e4166-222">packageId</span></span>|<span data-ttu-id="e4166-223">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e4166-223">String</span></span>|<span data-ttu-id="e4166-224">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="e4166-224">The package identifier.</span></span>|
|<span data-ttu-id="e4166-225">identityName</span><span class="sxs-lookup"><span data-stu-id="e4166-225">identityName</span></span>|<span data-ttu-id="e4166-226">String</span><span class="sxs-lookup"><span data-stu-id="e4166-226">String</span></span>|<span data-ttu-id="e4166-227">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="e4166-227">The Identity Name.</span></span>|
|<span data-ttu-id="e4166-228">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e4166-228">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e4166-229">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e4166-229">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="e4166-230">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="e4166-230">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e4166-231">versionName</span><span class="sxs-lookup"><span data-stu-id="e4166-231">versionName</span></span>|<span data-ttu-id="e4166-232">String</span><span class="sxs-lookup"><span data-stu-id="e4166-232">String</span></span>|<span data-ttu-id="e4166-233">Der Versionsname der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="e4166-233">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e4166-234">versionCode</span><span class="sxs-lookup"><span data-stu-id="e4166-234">versionCode</span></span>|<span data-ttu-id="e4166-235">String</span><span class="sxs-lookup"><span data-stu-id="e4166-235">String</span></span>|<span data-ttu-id="e4166-236">Der Codename der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="e4166-236">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e4166-237">identityVersion</span><span class="sxs-lookup"><span data-stu-id="e4166-237">identityVersion</span></span>|<span data-ttu-id="e4166-238">String</span><span class="sxs-lookup"><span data-stu-id="e4166-238">String</span></span>|<span data-ttu-id="e4166-239">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="e4166-239">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="e4166-240">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4166-240">Response</span></span>
<span data-ttu-id="e4166-241">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4166-241">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4166-242">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e4166-242">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4166-243">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4166-243">Request</span></span>
<span data-ttu-id="e4166-244">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e4166-244">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1464

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="e4166-245">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4166-245">Response</span></span>
<span data-ttu-id="e4166-p123">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4166-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1636

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```




