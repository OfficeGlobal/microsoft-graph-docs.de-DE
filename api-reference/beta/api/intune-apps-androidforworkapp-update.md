---
title: AndroidForWorkApp aktualisieren
description: Aktualisieren Sie die Eigenschaften eines AndroidForWorkApp-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 09b5f502ca8b666a687e2b0df99fed52b1c4ff12
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398345"
---
# <a name="update-androidforworkapp"></a><span data-ttu-id="21e07-103">AndroidForWorkApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="21e07-103">Update androidForWorkApp</span></span>

> <span data-ttu-id="21e07-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="21e07-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="21e07-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="21e07-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21e07-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="21e07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21e07-107">Aktualisieren Sie die Eigenschaften eines [AndroidForWorkApp](../resources/intune-apps-androidforworkapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="21e07-107">Update the properties of a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21e07-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="21e07-108">Prerequisites</span></span>
<span data-ttu-id="21e07-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="21e07-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="21e07-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="21e07-111">Permission type</span></span>|<span data-ttu-id="21e07-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="21e07-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21e07-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="21e07-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21e07-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21e07-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="21e07-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="21e07-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21e07-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21e07-116">Not supported.</span></span>|
|<span data-ttu-id="21e07-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="21e07-117">Application</span></span>|<span data-ttu-id="21e07-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21e07-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21e07-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="21e07-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="21e07-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="21e07-120">Request headers</span></span>
|<span data-ttu-id="21e07-121">Header</span><span class="sxs-lookup"><span data-stu-id="21e07-121">Header</span></span>|<span data-ttu-id="21e07-122">Wert</span><span class="sxs-lookup"><span data-stu-id="21e07-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21e07-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="21e07-123">Authorization</span></span>|<span data-ttu-id="21e07-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="21e07-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21e07-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="21e07-125">Accept</span></span>|<span data-ttu-id="21e07-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21e07-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21e07-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="21e07-127">Request body</span></span>
<span data-ttu-id="21e07-128">Geben Sie im Textkörper Anforderung für das Objekt [AndroidForWorkApp](../resources/intune-apps-androidforworkapp.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="21e07-128">In the request body, supply a JSON representation for the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

<span data-ttu-id="21e07-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [AndroidForWorkApp](../resources/intune-apps-androidforworkapp.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="21e07-129">The following table shows the properties that are required when you create the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md).</span></span>

|<span data-ttu-id="21e07-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="21e07-130">Property</span></span>|<span data-ttu-id="21e07-131">Typ</span><span class="sxs-lookup"><span data-stu-id="21e07-131">Type</span></span>|<span data-ttu-id="21e07-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21e07-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21e07-133">id</span><span class="sxs-lookup"><span data-stu-id="21e07-133">id</span></span>|<span data-ttu-id="21e07-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21e07-134">String</span></span>|<span data-ttu-id="21e07-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="21e07-135">Key of the entity.</span></span> <span data-ttu-id="21e07-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21e07-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21e07-137">displayName</span><span class="sxs-lookup"><span data-stu-id="21e07-137">displayName</span></span>|<span data-ttu-id="21e07-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21e07-138">String</span></span>|<span data-ttu-id="21e07-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="21e07-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="21e07-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21e07-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21e07-141">description</span><span class="sxs-lookup"><span data-stu-id="21e07-141">description</span></span>|<span data-ttu-id="21e07-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21e07-142">String</span></span>|<span data-ttu-id="21e07-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="21e07-143">The description of the app.</span></span> <span data-ttu-id="21e07-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21e07-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21e07-145">publisher</span><span class="sxs-lookup"><span data-stu-id="21e07-145">publisher</span></span>|<span data-ttu-id="21e07-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21e07-146">String</span></span>|<span data-ttu-id="21e07-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="21e07-147">The publisher of the app.</span></span> <span data-ttu-id="21e07-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21e07-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21e07-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="21e07-149">largeIcon</span></span>|[<span data-ttu-id="21e07-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="21e07-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="21e07-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="21e07-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="21e07-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21e07-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21e07-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21e07-153">createdDateTime</span></span>|<span data-ttu-id="21e07-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21e07-154">DateTimeOffset</span></span>|<span data-ttu-id="21e07-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="21e07-155">The date and time the app was created.</span></span> <span data-ttu-id="21e07-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21e07-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21e07-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="21e07-157">lastModifiedDateTime</span></span>|<span data-ttu-id="21e07-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21e07-158">DateTimeOffset</span></span>|<span data-ttu-id="21e07-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="21e07-159">The date and time the app was last modified.</span></span> <span data-ttu-id="21e07-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21e07-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21e07-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="21e07-161">isFeatured</span></span>|<span data-ttu-id="21e07-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="21e07-162">Boolean</span></span>|<span data-ttu-id="21e07-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21e07-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21e07-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="21e07-164">privacyInformationUrl</span></span>|<span data-ttu-id="21e07-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21e07-165">String</span></span>|<span data-ttu-id="21e07-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="21e07-166">The privacy statement Url.</span></span> <span data-ttu-id="21e07-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21e07-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21e07-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="21e07-168">informationUrl</span></span>|<span data-ttu-id="21e07-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21e07-169">String</span></span>|<span data-ttu-id="21e07-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="21e07-170">The more information Url.</span></span> <span data-ttu-id="21e07-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21e07-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21e07-172">owner</span><span class="sxs-lookup"><span data-stu-id="21e07-172">owner</span></span>|<span data-ttu-id="21e07-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21e07-173">String</span></span>|<span data-ttu-id="21e07-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="21e07-174">The owner of the app.</span></span> <span data-ttu-id="21e07-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21e07-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21e07-176">developer</span><span class="sxs-lookup"><span data-stu-id="21e07-176">developer</span></span>|<span data-ttu-id="21e07-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21e07-177">String</span></span>|<span data-ttu-id="21e07-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="21e07-178">The developer of the app.</span></span> <span data-ttu-id="21e07-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21e07-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21e07-180">notes</span><span class="sxs-lookup"><span data-stu-id="21e07-180">notes</span></span>|<span data-ttu-id="21e07-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21e07-181">String</span></span>|<span data-ttu-id="21e07-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="21e07-182">Notes for the app.</span></span> <span data-ttu-id="21e07-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21e07-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21e07-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="21e07-184">uploadState</span></span>|<span data-ttu-id="21e07-185">Int32</span><span class="sxs-lookup"><span data-stu-id="21e07-185">Int32</span></span>|<span data-ttu-id="21e07-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="21e07-186">The upload state.</span></span> <span data-ttu-id="21e07-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21e07-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21e07-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="21e07-188">publishingState</span></span>|[<span data-ttu-id="21e07-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="21e07-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="21e07-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="21e07-190">The publishing state for the app.</span></span> <span data-ttu-id="21e07-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="21e07-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="21e07-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21e07-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="21e07-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="21e07-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="21e07-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="21e07-194">isAssigned</span></span>|<span data-ttu-id="21e07-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="21e07-195">Boolean</span></span>|<span data-ttu-id="21e07-196">Der Wert, der angibt, ob die app mindestens eine Gruppe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="21e07-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="21e07-197">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21e07-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21e07-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="21e07-198">roleScopeTagIds</span></span>|<span data-ttu-id="21e07-199">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="21e07-199">String collection</span></span>|<span data-ttu-id="21e07-200">Liste der Bereichs-Tag-Ids für diese mobile app.</span><span class="sxs-lookup"><span data-stu-id="21e07-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="21e07-201">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21e07-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="21e07-202">packageId</span><span class="sxs-lookup"><span data-stu-id="21e07-202">packageId</span></span>|<span data-ttu-id="21e07-203">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21e07-203">String</span></span>|<span data-ttu-id="21e07-204">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="21e07-204">The package identifier.</span></span>|
|<span data-ttu-id="21e07-205">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="21e07-205">appIdentifier</span></span>|<span data-ttu-id="21e07-206">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21e07-206">String</span></span>|<span data-ttu-id="21e07-207">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="21e07-207">The Identity Name.</span></span>|
|<span data-ttu-id="21e07-208">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="21e07-208">usedLicenseCount</span></span>|<span data-ttu-id="21e07-209">Int32</span><span class="sxs-lookup"><span data-stu-id="21e07-209">Int32</span></span>|<span data-ttu-id="21e07-210">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="21e07-210">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="21e07-211">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="21e07-211">totalLicenseCount</span></span>|<span data-ttu-id="21e07-212">Int32</span><span class="sxs-lookup"><span data-stu-id="21e07-212">Int32</span></span>|<span data-ttu-id="21e07-213">Gesamtanzahl von VPP-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="21e07-213">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="21e07-214">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="21e07-214">appStoreUrl</span></span>|<span data-ttu-id="21e07-215">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21e07-215">String</span></span>|<span data-ttu-id="21e07-216">Wiedergeben für Arbeit Store-app-URL.</span><span class="sxs-lookup"><span data-stu-id="21e07-216">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="21e07-217">Antwort</span><span class="sxs-lookup"><span data-stu-id="21e07-217">Response</span></span>
<span data-ttu-id="21e07-218">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [AndroidForWorkApp](../resources/intune-apps-androidforworkapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="21e07-218">If successful, this method returns a `200 OK` response code and an updated [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21e07-219">Beispiel</span><span class="sxs-lookup"><span data-stu-id="21e07-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="21e07-220">Anforderung</span><span class="sxs-lookup"><span data-stu-id="21e07-220">Request</span></span>
<span data-ttu-id="21e07-221">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="21e07-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 876

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
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

### <a name="response"></a><span data-ttu-id="21e07-222">Antwort</span><span class="sxs-lookup"><span data-stu-id="21e07-222">Response</span></span>
<span data-ttu-id="21e07-p119">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="21e07-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1048

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
  "id": "c5010785-0785-c501-8507-01c5850701c5",
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




