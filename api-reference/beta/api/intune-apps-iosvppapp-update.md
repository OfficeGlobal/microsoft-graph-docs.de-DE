---
title: iosVppApp aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs iosVppApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7b5b6cac0e83872f928b38556bb5c8cadecead6b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414074"
---
# <a name="update-iosvppapp"></a><span data-ttu-id="1a2cb-103">iosVppApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1a2cb-103">Update iosVppApp</span></span>

> <span data-ttu-id="1a2cb-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1a2cb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a2cb-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a2cb-107">Aktualisiert die Eigenschaften von Objekten des Typs [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a2cb-107">Update the properties of a [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a2cb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1a2cb-108">Prerequisites</span></span>
<span data-ttu-id="1a2cb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1a2cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1a2cb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1a2cb-111">Permission type</span></span>|<span data-ttu-id="1a2cb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1a2cb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a2cb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1a2cb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1a2cb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a2cb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1a2cb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1a2cb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a2cb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1a2cb-116">Not supported.</span></span>|
|<span data-ttu-id="1a2cb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1a2cb-117">Application</span></span>|<span data-ttu-id="1a2cb-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1a2cb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a2cb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a2cb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="1a2cb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1a2cb-120">Request headers</span></span>
|<span data-ttu-id="1a2cb-121">Header</span><span class="sxs-lookup"><span data-stu-id="1a2cb-121">Header</span></span>|<span data-ttu-id="1a2cb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1a2cb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a2cb-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1a2cb-123">Authorization</span></span>|<span data-ttu-id="1a2cb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1a2cb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a2cb-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1a2cb-125">Accept</span></span>|<span data-ttu-id="1a2cb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1a2cb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a2cb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1a2cb-127">Request body</span></span>
<span data-ttu-id="1a2cb-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [iosVppApp](../resources/intune-apps-iosvppapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-128">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

<span data-ttu-id="1a2cb-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosVppApp](../resources/intune-apps-iosvppapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-129">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>

|<span data-ttu-id="1a2cb-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1a2cb-130">Property</span></span>|<span data-ttu-id="1a2cb-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1a2cb-131">Type</span></span>|<span data-ttu-id="1a2cb-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a2cb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a2cb-133">id</span><span class="sxs-lookup"><span data-stu-id="1a2cb-133">id</span></span>|<span data-ttu-id="1a2cb-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a2cb-134">String</span></span>|<span data-ttu-id="1a2cb-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1a2cb-135">Key of the entity.</span></span> <span data-ttu-id="1a2cb-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a2cb-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a2cb-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1a2cb-137">displayName</span></span>|<span data-ttu-id="1a2cb-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a2cb-138">String</span></span>|<span data-ttu-id="1a2cb-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1a2cb-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a2cb-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a2cb-141">description</span><span class="sxs-lookup"><span data-stu-id="1a2cb-141">description</span></span>|<span data-ttu-id="1a2cb-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a2cb-142">String</span></span>|<span data-ttu-id="1a2cb-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-143">The description of the app.</span></span> <span data-ttu-id="1a2cb-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a2cb-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a2cb-145">publisher</span><span class="sxs-lookup"><span data-stu-id="1a2cb-145">publisher</span></span>|<span data-ttu-id="1a2cb-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a2cb-146">String</span></span>|<span data-ttu-id="1a2cb-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-147">The publisher of the app.</span></span> <span data-ttu-id="1a2cb-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a2cb-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a2cb-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1a2cb-149">largeIcon</span></span>|[<span data-ttu-id="1a2cb-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1a2cb-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1a2cb-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1a2cb-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a2cb-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a2cb-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a2cb-153">createdDateTime</span></span>|<span data-ttu-id="1a2cb-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a2cb-154">DateTimeOffset</span></span>|<span data-ttu-id="1a2cb-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-155">The date and time the app was created.</span></span> <span data-ttu-id="1a2cb-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a2cb-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a2cb-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a2cb-157">lastModifiedDateTime</span></span>|<span data-ttu-id="1a2cb-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a2cb-158">DateTimeOffset</span></span>|<span data-ttu-id="1a2cb-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-159">The date and time the app was last modified.</span></span> <span data-ttu-id="1a2cb-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a2cb-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a2cb-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1a2cb-161">isFeatured</span></span>|<span data-ttu-id="1a2cb-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a2cb-162">Boolean</span></span>|<span data-ttu-id="1a2cb-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a2cb-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a2cb-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1a2cb-164">privacyInformationUrl</span></span>|<span data-ttu-id="1a2cb-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a2cb-165">String</span></span>|<span data-ttu-id="1a2cb-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-166">The privacy statement Url.</span></span> <span data-ttu-id="1a2cb-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a2cb-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a2cb-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1a2cb-168">informationUrl</span></span>|<span data-ttu-id="1a2cb-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a2cb-169">String</span></span>|<span data-ttu-id="1a2cb-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-170">The more information Url.</span></span> <span data-ttu-id="1a2cb-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a2cb-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a2cb-172">owner</span><span class="sxs-lookup"><span data-stu-id="1a2cb-172">owner</span></span>|<span data-ttu-id="1a2cb-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a2cb-173">String</span></span>|<span data-ttu-id="1a2cb-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-174">The owner of the app.</span></span> <span data-ttu-id="1a2cb-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a2cb-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a2cb-176">developer</span><span class="sxs-lookup"><span data-stu-id="1a2cb-176">developer</span></span>|<span data-ttu-id="1a2cb-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a2cb-177">String</span></span>|<span data-ttu-id="1a2cb-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-178">The developer of the app.</span></span> <span data-ttu-id="1a2cb-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a2cb-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a2cb-180">notes</span><span class="sxs-lookup"><span data-stu-id="1a2cb-180">notes</span></span>|<span data-ttu-id="1a2cb-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a2cb-181">String</span></span>|<span data-ttu-id="1a2cb-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-182">Notes for the app.</span></span> <span data-ttu-id="1a2cb-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a2cb-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a2cb-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="1a2cb-184">uploadState</span></span>|<span data-ttu-id="1a2cb-185">Int32</span><span class="sxs-lookup"><span data-stu-id="1a2cb-185">Int32</span></span>|<span data-ttu-id="1a2cb-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-186">The upload state.</span></span> <span data-ttu-id="1a2cb-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a2cb-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a2cb-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="1a2cb-188">publishingState</span></span>|[<span data-ttu-id="1a2cb-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1a2cb-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1a2cb-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-190">The publishing state for the app.</span></span> <span data-ttu-id="1a2cb-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1a2cb-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a2cb-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="1a2cb-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1a2cb-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="1a2cb-194">isAssigned</span></span>|<span data-ttu-id="1a2cb-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a2cb-195">Boolean</span></span>|<span data-ttu-id="1a2cb-196">Der Wert, der angibt, ob die app mindestens eine Gruppe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="1a2cb-197">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a2cb-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a2cb-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1a2cb-198">roleScopeTagIds</span></span>|<span data-ttu-id="1a2cb-199">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="1a2cb-199">String collection</span></span>|<span data-ttu-id="1a2cb-200">Liste der Bereichs-Tag-Ids für diese mobile app.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="1a2cb-201">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1a2cb-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a2cb-202">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="1a2cb-202">usedLicenseCount</span></span>|<span data-ttu-id="1a2cb-203">Int32</span><span class="sxs-lookup"><span data-stu-id="1a2cb-203">Int32</span></span>|<span data-ttu-id="1a2cb-204">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-204">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="1a2cb-205">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="1a2cb-205">totalLicenseCount</span></span>|<span data-ttu-id="1a2cb-206">Int32</span><span class="sxs-lookup"><span data-stu-id="1a2cb-206">Int32</span></span>|<span data-ttu-id="1a2cb-207">Gesamtanzahl von VPP-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-207">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="1a2cb-208">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="1a2cb-208">releaseDateTime</span></span>|<span data-ttu-id="1a2cb-209">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a2cb-209">DateTimeOffset</span></span>|<span data-ttu-id="1a2cb-210">Datum und Uhrzeit der Veröffentlichung der VPP-Anwendung.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-210">The VPP application release date and time.</span></span>|
|<span data-ttu-id="1a2cb-211">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="1a2cb-211">appStoreUrl</span></span>|<span data-ttu-id="1a2cb-212">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a2cb-212">String</span></span>|<span data-ttu-id="1a2cb-213">Store-URL</span><span class="sxs-lookup"><span data-stu-id="1a2cb-213">The store URL.</span></span>|
|<span data-ttu-id="1a2cb-214">licensingType</span><span class="sxs-lookup"><span data-stu-id="1a2cb-214">licensingType</span></span>|[<span data-ttu-id="1a2cb-215">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="1a2cb-215">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="1a2cb-216">Unterstützter Lizenztyp</span><span class="sxs-lookup"><span data-stu-id="1a2cb-216">The supported License Type.</span></span>|
|<span data-ttu-id="1a2cb-217">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="1a2cb-217">applicableDeviceType</span></span>|[<span data-ttu-id="1a2cb-218">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="1a2cb-218">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="1a2cb-219">Gültiger iOS-Gerätetyp</span><span class="sxs-lookup"><span data-stu-id="1a2cb-219">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="1a2cb-220">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="1a2cb-220">vppTokenOrganizationName</span></span>|<span data-ttu-id="1a2cb-221">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a2cb-221">String</span></span>|<span data-ttu-id="1a2cb-222">Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="1a2cb-222">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="1a2cb-223">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="1a2cb-223">vppTokenAccountType</span></span>|[<span data-ttu-id="1a2cb-224">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="1a2cb-224">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="1a2cb-225">Volume Purchase Program-Typ, dem das angegebene Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-225">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="1a2cb-226">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-226">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="1a2cb-227">Mögliche Werte sind: `business` und `education`.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-227">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="1a2cb-228">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="1a2cb-228">vppTokenAppleId</span></span>|<span data-ttu-id="1a2cb-229">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a2cb-229">String</span></span>|<span data-ttu-id="1a2cb-230">Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="1a2cb-230">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="1a2cb-231">bundleId</span><span class="sxs-lookup"><span data-stu-id="1a2cb-231">bundleId</span></span>|<span data-ttu-id="1a2cb-232">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a2cb-232">String</span></span>|<span data-ttu-id="1a2cb-233">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="1a2cb-233">The Identity Name.</span></span>|
|<span data-ttu-id="1a2cb-234">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="1a2cb-234">vppTokenId</span></span>|<span data-ttu-id="1a2cb-235">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1a2cb-235">String</span></span>|<span data-ttu-id="1a2cb-236">Bezeichner des Tokens VPP diese app zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-236">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="1a2cb-237">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="1a2cb-237">revokeLicenseActionResults</span></span>|<span data-ttu-id="1a2cb-238">[IosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="1a2cb-238">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="1a2cb-239">Ergebnisse der widerrufen diese app-Lizenz Aktionen.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-239">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="1a2cb-240">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a2cb-240">Response</span></span>
<span data-ttu-id="1a2cb-241">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [iosVppApp](../resources/intune-apps-iosvppapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-241">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a2cb-242">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1a2cb-242">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a2cb-243">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1a2cb-243">Request</span></span>
<span data-ttu-id="1a2cb-244">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-244">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1972

{
  "@odata.type": "#microsoft.graph.iosVppApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="1a2cb-245">Antwort</span><span class="sxs-lookup"><span data-stu-id="1a2cb-245">Response</span></span>
<span data-ttu-id="1a2cb-p120">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1a2cb-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2144

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```




