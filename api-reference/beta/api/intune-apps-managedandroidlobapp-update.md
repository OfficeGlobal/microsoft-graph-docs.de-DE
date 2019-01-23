---
title: managedAndroidLobApp aktualisieren
description: Aktualisieren der Eigenschaften eines managedAndroidLobApp-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7fa0ace9f4e1235b5ca63ee9c7249d7f667c8b2e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394642"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="4f165-103">managedAndroidLobApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4f165-103">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="4f165-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="4f165-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4f165-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4f165-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4f165-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4f165-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f165-107">Aktualisieren der Eigenschaften eines [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4f165-107">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f165-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4f165-108">Prerequisites</span></span>
<span data-ttu-id="4f165-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4f165-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4f165-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4f165-111">Permission type</span></span>|<span data-ttu-id="4f165-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4f165-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f165-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4f165-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f165-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f165-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4f165-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4f165-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f165-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4f165-116">Not supported.</span></span>|
|<span data-ttu-id="4f165-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4f165-117">Application</span></span>|<span data-ttu-id="4f165-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4f165-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f165-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4f165-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="4f165-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4f165-120">Request headers</span></span>
|<span data-ttu-id="4f165-121">Header</span><span class="sxs-lookup"><span data-stu-id="4f165-121">Header</span></span>|<span data-ttu-id="4f165-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4f165-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f165-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4f165-123">Authorization</span></span>|<span data-ttu-id="4f165-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4f165-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f165-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4f165-125">Accept</span></span>|<span data-ttu-id="4f165-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4f165-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f165-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4f165-127">Request body</span></span>
<span data-ttu-id="4f165-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="4f165-128">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="4f165-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="4f165-129">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="4f165-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4f165-130">Property</span></span>|<span data-ttu-id="4f165-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4f165-131">Type</span></span>|<span data-ttu-id="4f165-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4f165-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f165-133">id</span><span class="sxs-lookup"><span data-stu-id="4f165-133">id</span></span>|<span data-ttu-id="4f165-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f165-134">String</span></span>|<span data-ttu-id="4f165-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4f165-135">Key of the entity.</span></span> <span data-ttu-id="4f165-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f165-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f165-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4f165-137">displayName</span></span>|<span data-ttu-id="4f165-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f165-138">String</span></span>|<span data-ttu-id="4f165-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="4f165-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4f165-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f165-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f165-141">description</span><span class="sxs-lookup"><span data-stu-id="4f165-141">description</span></span>|<span data-ttu-id="4f165-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f165-142">String</span></span>|<span data-ttu-id="4f165-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="4f165-143">The description of the app.</span></span> <span data-ttu-id="4f165-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f165-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f165-145">publisher</span><span class="sxs-lookup"><span data-stu-id="4f165-145">publisher</span></span>|<span data-ttu-id="4f165-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f165-146">String</span></span>|<span data-ttu-id="4f165-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="4f165-147">The publisher of the app.</span></span> <span data-ttu-id="4f165-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f165-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f165-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4f165-149">largeIcon</span></span>|[<span data-ttu-id="4f165-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4f165-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4f165-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="4f165-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4f165-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f165-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f165-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4f165-153">createdDateTime</span></span>|<span data-ttu-id="4f165-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f165-154">DateTimeOffset</span></span>|<span data-ttu-id="4f165-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="4f165-155">The date and time the app was created.</span></span> <span data-ttu-id="4f165-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f165-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f165-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f165-157">lastModifiedDateTime</span></span>|<span data-ttu-id="4f165-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f165-158">DateTimeOffset</span></span>|<span data-ttu-id="4f165-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="4f165-159">The date and time the app was last modified.</span></span> <span data-ttu-id="4f165-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f165-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f165-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4f165-161">isFeatured</span></span>|<span data-ttu-id="4f165-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f165-162">Boolean</span></span>|<span data-ttu-id="4f165-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f165-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f165-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4f165-164">privacyInformationUrl</span></span>|<span data-ttu-id="4f165-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f165-165">String</span></span>|<span data-ttu-id="4f165-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="4f165-166">The privacy statement Url.</span></span> <span data-ttu-id="4f165-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f165-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f165-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4f165-168">informationUrl</span></span>|<span data-ttu-id="4f165-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f165-169">String</span></span>|<span data-ttu-id="4f165-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="4f165-170">The more information Url.</span></span> <span data-ttu-id="4f165-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f165-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f165-172">owner</span><span class="sxs-lookup"><span data-stu-id="4f165-172">owner</span></span>|<span data-ttu-id="4f165-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f165-173">String</span></span>|<span data-ttu-id="4f165-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="4f165-174">The owner of the app.</span></span> <span data-ttu-id="4f165-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f165-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f165-176">developer</span><span class="sxs-lookup"><span data-stu-id="4f165-176">developer</span></span>|<span data-ttu-id="4f165-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f165-177">String</span></span>|<span data-ttu-id="4f165-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="4f165-178">The developer of the app.</span></span> <span data-ttu-id="4f165-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f165-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f165-180">notes</span><span class="sxs-lookup"><span data-stu-id="4f165-180">notes</span></span>|<span data-ttu-id="4f165-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f165-181">String</span></span>|<span data-ttu-id="4f165-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="4f165-182">Notes for the app.</span></span> <span data-ttu-id="4f165-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f165-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f165-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="4f165-184">uploadState</span></span>|<span data-ttu-id="4f165-185">Int32</span><span class="sxs-lookup"><span data-stu-id="4f165-185">Int32</span></span>|<span data-ttu-id="4f165-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="4f165-186">The upload state.</span></span> <span data-ttu-id="4f165-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f165-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f165-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="4f165-188">publishingState</span></span>|[<span data-ttu-id="4f165-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4f165-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4f165-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="4f165-190">The publishing state for the app.</span></span> <span data-ttu-id="4f165-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="4f165-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4f165-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f165-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="4f165-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="4f165-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4f165-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4f165-194">isAssigned</span></span>|<span data-ttu-id="4f165-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f165-195">Boolean</span></span>|<span data-ttu-id="4f165-196">Der Wert, der angibt, ob die app mindestens eine Gruppe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="4f165-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4f165-197">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f165-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f165-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4f165-198">roleScopeTagIds</span></span>|<span data-ttu-id="4f165-199">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="4f165-199">String collection</span></span>|<span data-ttu-id="4f165-200">Liste der Bereichs-Tag-Ids für diese mobile app.</span><span class="sxs-lookup"><span data-stu-id="4f165-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4f165-201">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f165-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f165-202">appAvailability</span><span class="sxs-lookup"><span data-stu-id="4f165-202">appAvailability</span></span>|[<span data-ttu-id="4f165-203">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="4f165-203">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="4f165-204">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="4f165-204">The Application's availability.</span></span> <span data-ttu-id="4f165-205">Geerbt von [ManagedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f165-205">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="4f165-206">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="4f165-206">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="4f165-207">version</span><span class="sxs-lookup"><span data-stu-id="4f165-207">version</span></span>|<span data-ttu-id="4f165-208">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f165-208">String</span></span>|<span data-ttu-id="4f165-209">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="4f165-209">The Application's version.</span></span> <span data-ttu-id="4f165-210">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f165-210">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="4f165-211">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="4f165-211">committedContentVersion</span></span>|<span data-ttu-id="4f165-212">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f165-212">String</span></span>|<span data-ttu-id="4f165-213">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="4f165-213">The internal committed content version.</span></span> <span data-ttu-id="4f165-214">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f165-214">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4f165-215">fileName</span><span class="sxs-lookup"><span data-stu-id="4f165-215">fileName</span></span>|<span data-ttu-id="4f165-216">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f165-216">String</span></span>|<span data-ttu-id="4f165-217">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="4f165-217">The name of the main Lob application file.</span></span> <span data-ttu-id="4f165-218">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f165-218">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4f165-219">size</span><span class="sxs-lookup"><span data-stu-id="4f165-219">size</span></span>|<span data-ttu-id="4f165-220">Int64</span><span class="sxs-lookup"><span data-stu-id="4f165-220">Int64</span></span>|<span data-ttu-id="4f165-221">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="4f165-221">The total size, including all uploaded files.</span></span> <span data-ttu-id="4f165-222">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f165-222">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4f165-223">packageId</span><span class="sxs-lookup"><span data-stu-id="4f165-223">packageId</span></span>|<span data-ttu-id="4f165-224">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f165-224">String</span></span>|<span data-ttu-id="4f165-225">Bezeichner des Pakets</span><span class="sxs-lookup"><span data-stu-id="4f165-225">The package identifier.</span></span>|
|<span data-ttu-id="4f165-226">identityName</span><span class="sxs-lookup"><span data-stu-id="4f165-226">identityName</span></span>|<span data-ttu-id="4f165-227">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f165-227">String</span></span>|<span data-ttu-id="4f165-228">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="4f165-228">The Identity Name.</span></span>|
|<span data-ttu-id="4f165-229">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4f165-229">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="4f165-230">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4f165-230">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="4f165-231">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="4f165-231">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="4f165-232">versionName</span><span class="sxs-lookup"><span data-stu-id="4f165-232">versionName</span></span>|<span data-ttu-id="4f165-233">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f165-233">String</span></span>|<span data-ttu-id="4f165-234">Der Versionsname der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="4f165-234">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="4f165-235">versionCode</span><span class="sxs-lookup"><span data-stu-id="4f165-235">versionCode</span></span>|<span data-ttu-id="4f165-236">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f165-236">String</span></span>|<span data-ttu-id="4f165-237">Der Codename der verwalteten branchenspezifischen Android-App.</span><span class="sxs-lookup"><span data-stu-id="4f165-237">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="4f165-238">identityVersion</span><span class="sxs-lookup"><span data-stu-id="4f165-238">identityVersion</span></span>|<span data-ttu-id="4f165-239">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f165-239">String</span></span>|<span data-ttu-id="4f165-240">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="4f165-240">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="4f165-241">Antwort</span><span class="sxs-lookup"><span data-stu-id="4f165-241">Response</span></span>
<span data-ttu-id="4f165-242">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4f165-242">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f165-243">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4f165-243">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f165-244">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4f165-244">Request</span></span>
<span data-ttu-id="4f165-245">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4f165-245">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4f165-246">Antwort</span><span class="sxs-lookup"><span data-stu-id="4f165-246">Response</span></span>
<span data-ttu-id="4f165-p124">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4f165-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




