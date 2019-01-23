---
title: AndroidManagedStoreApp aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidManagedStoreApp-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9d100738e96219dff925f069259309b2ffccb84a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413766"
---
# <a name="update-androidmanagedstoreapp"></a><span data-ttu-id="6a716-103">AndroidManagedStoreApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6a716-103">Update androidManagedStoreApp</span></span>

> <span data-ttu-id="6a716-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="6a716-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6a716-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6a716-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6a716-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6a716-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a716-107">Aktualisieren Sie die Eigenschaften eines [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6a716-107">Update the properties of a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a716-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6a716-108">Prerequisites</span></span>
<span data-ttu-id="6a716-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6a716-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6a716-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6a716-111">Permission type</span></span>|<span data-ttu-id="6a716-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6a716-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a716-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6a716-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6a716-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a716-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6a716-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6a716-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a716-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6a716-116">Not supported.</span></span>|
|<span data-ttu-id="6a716-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6a716-117">Application</span></span>|<span data-ttu-id="6a716-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6a716-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a716-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a716-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="6a716-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6a716-120">Request headers</span></span>
|<span data-ttu-id="6a716-121">Header</span><span class="sxs-lookup"><span data-stu-id="6a716-121">Header</span></span>|<span data-ttu-id="6a716-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6a716-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a716-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6a716-123">Authorization</span></span>|<span data-ttu-id="6a716-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6a716-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a716-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6a716-125">Accept</span></span>|<span data-ttu-id="6a716-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6a716-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a716-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6a716-127">Request body</span></span>
<span data-ttu-id="6a716-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="6a716-128">In the request body, supply a JSON representation for the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

<span data-ttu-id="6a716-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="6a716-129">The following table shows the properties that are required when you create the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md).</span></span>

|<span data-ttu-id="6a716-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6a716-130">Property</span></span>|<span data-ttu-id="6a716-131">Typ</span><span class="sxs-lookup"><span data-stu-id="6a716-131">Type</span></span>|<span data-ttu-id="6a716-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6a716-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a716-133">id</span><span class="sxs-lookup"><span data-stu-id="6a716-133">id</span></span>|<span data-ttu-id="6a716-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a716-134">String</span></span>|<span data-ttu-id="6a716-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6a716-135">Key of the entity.</span></span> <span data-ttu-id="6a716-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a716-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a716-137">displayName</span><span class="sxs-lookup"><span data-stu-id="6a716-137">displayName</span></span>|<span data-ttu-id="6a716-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a716-138">String</span></span>|<span data-ttu-id="6a716-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="6a716-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6a716-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a716-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a716-141">description</span><span class="sxs-lookup"><span data-stu-id="6a716-141">description</span></span>|<span data-ttu-id="6a716-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a716-142">String</span></span>|<span data-ttu-id="6a716-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="6a716-143">The description of the app.</span></span> <span data-ttu-id="6a716-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a716-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a716-145">publisher</span><span class="sxs-lookup"><span data-stu-id="6a716-145">publisher</span></span>|<span data-ttu-id="6a716-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a716-146">String</span></span>|<span data-ttu-id="6a716-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="6a716-147">The publisher of the app.</span></span> <span data-ttu-id="6a716-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a716-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a716-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6a716-149">largeIcon</span></span>|[<span data-ttu-id="6a716-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6a716-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6a716-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="6a716-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6a716-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a716-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a716-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a716-153">createdDateTime</span></span>|<span data-ttu-id="6a716-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a716-154">DateTimeOffset</span></span>|<span data-ttu-id="6a716-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="6a716-155">The date and time the app was created.</span></span> <span data-ttu-id="6a716-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a716-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a716-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a716-157">lastModifiedDateTime</span></span>|<span data-ttu-id="6a716-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a716-158">DateTimeOffset</span></span>|<span data-ttu-id="6a716-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="6a716-159">The date and time the app was last modified.</span></span> <span data-ttu-id="6a716-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a716-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a716-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6a716-161">isFeatured</span></span>|<span data-ttu-id="6a716-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a716-162">Boolean</span></span>|<span data-ttu-id="6a716-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a716-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a716-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6a716-164">privacyInformationUrl</span></span>|<span data-ttu-id="6a716-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a716-165">String</span></span>|<span data-ttu-id="6a716-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="6a716-166">The privacy statement Url.</span></span> <span data-ttu-id="6a716-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a716-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a716-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6a716-168">informationUrl</span></span>|<span data-ttu-id="6a716-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a716-169">String</span></span>|<span data-ttu-id="6a716-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="6a716-170">The more information Url.</span></span> <span data-ttu-id="6a716-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a716-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a716-172">owner</span><span class="sxs-lookup"><span data-stu-id="6a716-172">owner</span></span>|<span data-ttu-id="6a716-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a716-173">String</span></span>|<span data-ttu-id="6a716-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="6a716-174">The owner of the app.</span></span> <span data-ttu-id="6a716-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a716-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a716-176">developer</span><span class="sxs-lookup"><span data-stu-id="6a716-176">developer</span></span>|<span data-ttu-id="6a716-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a716-177">String</span></span>|<span data-ttu-id="6a716-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="6a716-178">The developer of the app.</span></span> <span data-ttu-id="6a716-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a716-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a716-180">notes</span><span class="sxs-lookup"><span data-stu-id="6a716-180">notes</span></span>|<span data-ttu-id="6a716-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a716-181">String</span></span>|<span data-ttu-id="6a716-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="6a716-182">Notes for the app.</span></span> <span data-ttu-id="6a716-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a716-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a716-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="6a716-184">uploadState</span></span>|<span data-ttu-id="6a716-185">Int32</span><span class="sxs-lookup"><span data-stu-id="6a716-185">Int32</span></span>|<span data-ttu-id="6a716-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="6a716-186">The upload state.</span></span> <span data-ttu-id="6a716-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a716-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a716-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="6a716-188">publishingState</span></span>|[<span data-ttu-id="6a716-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="6a716-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="6a716-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="6a716-190">The publishing state for the app.</span></span> <span data-ttu-id="6a716-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="6a716-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6a716-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a716-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="6a716-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="6a716-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6a716-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="6a716-194">isAssigned</span></span>|<span data-ttu-id="6a716-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a716-195">Boolean</span></span>|<span data-ttu-id="6a716-196">Der Wert, der angibt, ob die app mindestens eine Gruppe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="6a716-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="6a716-197">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a716-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a716-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6a716-198">roleScopeTagIds</span></span>|<span data-ttu-id="6a716-199">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="6a716-199">String collection</span></span>|<span data-ttu-id="6a716-200">Liste der Bereichs-Tag-Ids für diese mobile app.</span><span class="sxs-lookup"><span data-stu-id="6a716-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="6a716-201">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a716-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6a716-202">packageId</span><span class="sxs-lookup"><span data-stu-id="6a716-202">packageId</span></span>|<span data-ttu-id="6a716-203">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a716-203">String</span></span>|<span data-ttu-id="6a716-204">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="6a716-204">The package identifier.</span></span>|
|<span data-ttu-id="6a716-205">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="6a716-205">appIdentifier</span></span>|<span data-ttu-id="6a716-206">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a716-206">String</span></span>|<span data-ttu-id="6a716-207">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="6a716-207">The Identity Name.</span></span>|
|<span data-ttu-id="6a716-208">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="6a716-208">usedLicenseCount</span></span>|<span data-ttu-id="6a716-209">Int32</span><span class="sxs-lookup"><span data-stu-id="6a716-209">Int32</span></span>|<span data-ttu-id="6a716-210">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="6a716-210">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="6a716-211">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="6a716-211">totalLicenseCount</span></span>|<span data-ttu-id="6a716-212">Int32</span><span class="sxs-lookup"><span data-stu-id="6a716-212">Int32</span></span>|<span data-ttu-id="6a716-213">Gesamtanzahl von VPP-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="6a716-213">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="6a716-214">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="6a716-214">appStoreUrl</span></span>|<span data-ttu-id="6a716-215">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a716-215">String</span></span>|<span data-ttu-id="6a716-216">Wiedergeben für Arbeit Store-app-URL.</span><span class="sxs-lookup"><span data-stu-id="6a716-216">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="6a716-217">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a716-217">Response</span></span>
<span data-ttu-id="6a716-218">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6a716-218">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a716-219">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6a716-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a716-220">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a716-220">Request</span></span>
<span data-ttu-id="6a716-221">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6a716-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 881

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="6a716-222">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a716-222">Response</span></span>
<span data-ttu-id="6a716-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6a716-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1053

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
  "id": "87247525-7525-8724-2575-248725752487",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```




