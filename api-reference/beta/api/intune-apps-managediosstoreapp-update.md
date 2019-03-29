---
title: managedIOSStoreApp aktualisieren
description: Aktualisieren der Eigenschaften eines managedIOSStoreApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c588c0b41961aca714efc5b74f49f8421c1eb33
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984919"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="b2a97-103">managedIOSStoreApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b2a97-103">Update managedIOSStoreApp</span></span>

> <span data-ttu-id="b2a97-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b2a97-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2a97-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b2a97-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2a97-106">Aktualisieren der Eigenschaften eines [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b2a97-106">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2a97-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b2a97-107">Prerequisites</span></span>
<span data-ttu-id="b2a97-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2a97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2a97-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b2a97-110">Permission type</span></span>|<span data-ttu-id="b2a97-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b2a97-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2a97-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b2a97-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2a97-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2a97-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b2a97-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b2a97-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2a97-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b2a97-115">Not supported.</span></span>|
|<span data-ttu-id="b2a97-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b2a97-116">Application</span></span>|<span data-ttu-id="b2a97-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b2a97-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2a97-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b2a97-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="b2a97-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b2a97-119">Request headers</span></span>
|<span data-ttu-id="b2a97-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b2a97-120">Header</span></span>|<span data-ttu-id="b2a97-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b2a97-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2a97-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2a97-122">Authorization</span></span>|<span data-ttu-id="b2a97-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b2a97-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2a97-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b2a97-124">Accept</span></span>|<span data-ttu-id="b2a97-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2a97-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2a97-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b2a97-126">Request body</span></span>
<span data-ttu-id="b2a97-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="b2a97-127">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="b2a97-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b2a97-128">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="b2a97-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b2a97-129">Property</span></span>|<span data-ttu-id="b2a97-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b2a97-130">Type</span></span>|<span data-ttu-id="b2a97-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b2a97-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2a97-132">id</span><span class="sxs-lookup"><span data-stu-id="b2a97-132">id</span></span>|<span data-ttu-id="b2a97-133">String</span><span class="sxs-lookup"><span data-stu-id="b2a97-133">String</span></span>|<span data-ttu-id="b2a97-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b2a97-134">Key of the entity.</span></span> <span data-ttu-id="b2a97-135">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b2a97-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a97-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b2a97-136">displayName</span></span>|<span data-ttu-id="b2a97-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b2a97-137">String</span></span>|<span data-ttu-id="b2a97-138">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="b2a97-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b2a97-139">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b2a97-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a97-140">description</span><span class="sxs-lookup"><span data-stu-id="b2a97-140">description</span></span>|<span data-ttu-id="b2a97-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b2a97-141">String</span></span>|<span data-ttu-id="b2a97-142">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="b2a97-142">The description of the app.</span></span> <span data-ttu-id="b2a97-143">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b2a97-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a97-144">publisher</span><span class="sxs-lookup"><span data-stu-id="b2a97-144">publisher</span></span>|<span data-ttu-id="b2a97-145">String</span><span class="sxs-lookup"><span data-stu-id="b2a97-145">String</span></span>|<span data-ttu-id="b2a97-146">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="b2a97-146">The publisher of the app.</span></span> <span data-ttu-id="b2a97-147">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b2a97-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a97-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b2a97-148">largeIcon</span></span>|[<span data-ttu-id="b2a97-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b2a97-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b2a97-150">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="b2a97-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b2a97-151">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b2a97-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a97-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b2a97-152">createdDateTime</span></span>|<span data-ttu-id="b2a97-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2a97-153">DateTimeOffset</span></span>|<span data-ttu-id="b2a97-154">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="b2a97-154">The date and time the app was created.</span></span> <span data-ttu-id="b2a97-155">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b2a97-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a97-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b2a97-156">lastModifiedDateTime</span></span>|<span data-ttu-id="b2a97-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2a97-157">DateTimeOffset</span></span>|<span data-ttu-id="b2a97-158">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="b2a97-158">The date and time the app was last modified.</span></span> <span data-ttu-id="b2a97-159">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b2a97-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a97-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b2a97-160">isFeatured</span></span>|<span data-ttu-id="b2a97-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2a97-161">Boolean</span></span>|<span data-ttu-id="b2a97-162">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b2a97-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a97-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b2a97-163">privacyInformationUrl</span></span>|<span data-ttu-id="b2a97-164">String</span><span class="sxs-lookup"><span data-stu-id="b2a97-164">String</span></span>|<span data-ttu-id="b2a97-165">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="b2a97-165">The privacy statement Url.</span></span> <span data-ttu-id="b2a97-166">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b2a97-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a97-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b2a97-167">informationUrl</span></span>|<span data-ttu-id="b2a97-168">String</span><span class="sxs-lookup"><span data-stu-id="b2a97-168">String</span></span>|<span data-ttu-id="b2a97-169">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="b2a97-169">The more information Url.</span></span> <span data-ttu-id="b2a97-170">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b2a97-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a97-171">owner</span><span class="sxs-lookup"><span data-stu-id="b2a97-171">owner</span></span>|<span data-ttu-id="b2a97-172">String</span><span class="sxs-lookup"><span data-stu-id="b2a97-172">String</span></span>|<span data-ttu-id="b2a97-173">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="b2a97-173">The owner of the app.</span></span> <span data-ttu-id="b2a97-174">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b2a97-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a97-175">developer</span><span class="sxs-lookup"><span data-stu-id="b2a97-175">developer</span></span>|<span data-ttu-id="b2a97-176">String</span><span class="sxs-lookup"><span data-stu-id="b2a97-176">String</span></span>|<span data-ttu-id="b2a97-177">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="b2a97-177">The developer of the app.</span></span> <span data-ttu-id="b2a97-178">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b2a97-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a97-179">notes</span><span class="sxs-lookup"><span data-stu-id="b2a97-179">notes</span></span>|<span data-ttu-id="b2a97-180">String</span><span class="sxs-lookup"><span data-stu-id="b2a97-180">String</span></span>|<span data-ttu-id="b2a97-181">Hinweise für die App.</span><span class="sxs-lookup"><span data-stu-id="b2a97-181">Notes for the app.</span></span> <span data-ttu-id="b2a97-182">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b2a97-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a97-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="b2a97-183">uploadState</span></span>|<span data-ttu-id="b2a97-184">Int32</span><span class="sxs-lookup"><span data-stu-id="b2a97-184">Int32</span></span>|<span data-ttu-id="b2a97-185">Der Uploadstatus.</span><span class="sxs-lookup"><span data-stu-id="b2a97-185">The upload state.</span></span> <span data-ttu-id="b2a97-186">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b2a97-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a97-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="b2a97-187">publishingState</span></span>|[<span data-ttu-id="b2a97-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b2a97-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b2a97-189">Der Veröffentlichungsstatus für die App.</span><span class="sxs-lookup"><span data-stu-id="b2a97-189">The publishing state for the app.</span></span> <span data-ttu-id="b2a97-190">Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="b2a97-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b2a97-191">Von [MobileApp](../resources/intune-apps-mobileapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="b2a97-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b2a97-192">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="b2a97-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b2a97-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b2a97-193">isAssigned</span></span>|<span data-ttu-id="b2a97-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2a97-194">Boolean</span></span>|<span data-ttu-id="b2a97-195">Der Wert, der angibt, ob die APP mindestens einer Gruppe zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="b2a97-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b2a97-196">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b2a97-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a97-197">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="b2a97-197">roleScopeTagIds</span></span>|<span data-ttu-id="b2a97-198">String collection</span><span class="sxs-lookup"><span data-stu-id="b2a97-198">String collection</span></span>|<span data-ttu-id="b2a97-199">Liste der bereichstag-IDs für diese Mobile App.</span><span class="sxs-lookup"><span data-stu-id="b2a97-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b2a97-200">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b2a97-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a97-201">appAvailability</span><span class="sxs-lookup"><span data-stu-id="b2a97-201">appAvailability</span></span>|[<span data-ttu-id="b2a97-202">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="b2a97-202">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="b2a97-203">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="b2a97-203">The Application's availability.</span></span> <span data-ttu-id="b2a97-204">Von [ManagedApp](../resources/intune-apps-managedapp.md)geerbt.</span><span class="sxs-lookup"><span data-stu-id="b2a97-204">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="b2a97-205">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="b2a97-205">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="b2a97-206">version</span><span class="sxs-lookup"><span data-stu-id="b2a97-206">version</span></span>|<span data-ttu-id="b2a97-207">String</span><span class="sxs-lookup"><span data-stu-id="b2a97-207">String</span></span>|<span data-ttu-id="b2a97-208">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="b2a97-208">The Application's version.</span></span> <span data-ttu-id="b2a97-209">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="b2a97-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="b2a97-210">bundleId</span><span class="sxs-lookup"><span data-stu-id="b2a97-210">bundleId</span></span>|<span data-ttu-id="b2a97-211">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b2a97-211">String</span></span>|<span data-ttu-id="b2a97-212">Die Bundle-ID einer App.</span><span class="sxs-lookup"><span data-stu-id="b2a97-212">The app's Bundle ID.</span></span>|
|<span data-ttu-id="b2a97-213">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b2a97-213">appStoreUrl</span></span>|<span data-ttu-id="b2a97-214">String</span><span class="sxs-lookup"><span data-stu-id="b2a97-214">String</span></span>|<span data-ttu-id="b2a97-215">Die URL des Apple-App-Stores.</span><span class="sxs-lookup"><span data-stu-id="b2a97-215">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="b2a97-216">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="b2a97-216">applicableDeviceType</span></span>|[<span data-ttu-id="b2a97-217">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="b2a97-217">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="b2a97-218">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="b2a97-218">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="b2a97-219">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b2a97-219">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b2a97-220">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b2a97-220">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="b2a97-221">Der Wert für die Mindestversion des unterstützten Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="b2a97-221">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="b2a97-222">Antwort</span><span class="sxs-lookup"><span data-stu-id="b2a97-222">Response</span></span>
<span data-ttu-id="b2a97-223">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b2a97-223">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2a97-224">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b2a97-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2a97-225">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b2a97-225">Request</span></span>
<span data-ttu-id="b2a97-226">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b2a97-226">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1191

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="b2a97-227">Antwort</span><span class="sxs-lookup"><span data-stu-id="b2a97-227">Response</span></span>
<span data-ttu-id="b2a97-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b2a97-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1363

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```




