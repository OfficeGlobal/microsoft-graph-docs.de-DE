---
title: managedIOSLobApp erstellen
description: Erstellen eines neuen managedIOSLobApp-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9ae2e7e362881731122b1a9f783d378c3f0ff5a4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409055"
---
# <a name="create-managedioslobapp"></a><span data-ttu-id="5c1f7-103">managedIOSLobApp erstellen</span><span class="sxs-lookup"><span data-stu-id="5c1f7-103">Create managedIOSLobApp</span></span>

> <span data-ttu-id="5c1f7-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5c1f7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5c1f7-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c1f7-107">Erstellen eines neuen [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-107">Create a new [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c1f7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5c1f7-108">Prerequisites</span></span>
<span data-ttu-id="5c1f7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5c1f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5c1f7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5c1f7-111">Permission type</span></span>|<span data-ttu-id="5c1f7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5c1f7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c1f7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5c1f7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5c1f7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c1f7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5c1f7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5c1f7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c1f7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5c1f7-116">Not supported.</span></span>|
|<span data-ttu-id="5c1f7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5c1f7-117">Application</span></span>|<span data-ttu-id="5c1f7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5c1f7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c1f7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5c1f7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="5c1f7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5c1f7-120">Request headers</span></span>
|<span data-ttu-id="5c1f7-121">Header</span><span class="sxs-lookup"><span data-stu-id="5c1f7-121">Header</span></span>|<span data-ttu-id="5c1f7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5c1f7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c1f7-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5c1f7-123">Authorization</span></span>|<span data-ttu-id="5c1f7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5c1f7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c1f7-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5c1f7-125">Accept</span></span>|<span data-ttu-id="5c1f7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5c1f7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c1f7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5c1f7-127">Request body</span></span>
<span data-ttu-id="5c1f7-128">Geben Sie im Anforderungstext eine JSON-Darstellung des managedIOSLobApp-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-128">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="5c1f7-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managedIOSLobApp erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-129">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="5c1f7-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5c1f7-130">Property</span></span>|<span data-ttu-id="5c1f7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5c1f7-131">Type</span></span>|<span data-ttu-id="5c1f7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5c1f7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c1f7-133">id</span><span class="sxs-lookup"><span data-stu-id="5c1f7-133">id</span></span>|<span data-ttu-id="5c1f7-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c1f7-134">String</span></span>|<span data-ttu-id="5c1f7-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5c1f7-135">Key of the entity.</span></span> <span data-ttu-id="5c1f7-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c1f7-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c1f7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="5c1f7-137">displayName</span></span>|<span data-ttu-id="5c1f7-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c1f7-138">String</span></span>|<span data-ttu-id="5c1f7-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5c1f7-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c1f7-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c1f7-141">description</span><span class="sxs-lookup"><span data-stu-id="5c1f7-141">description</span></span>|<span data-ttu-id="5c1f7-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c1f7-142">String</span></span>|<span data-ttu-id="5c1f7-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-143">The description of the app.</span></span> <span data-ttu-id="5c1f7-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c1f7-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c1f7-145">publisher</span><span class="sxs-lookup"><span data-stu-id="5c1f7-145">publisher</span></span>|<span data-ttu-id="5c1f7-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c1f7-146">String</span></span>|<span data-ttu-id="5c1f7-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-147">The publisher of the app.</span></span> <span data-ttu-id="5c1f7-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c1f7-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c1f7-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5c1f7-149">largeIcon</span></span>|[<span data-ttu-id="5c1f7-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5c1f7-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5c1f7-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5c1f7-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c1f7-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c1f7-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c1f7-153">createdDateTime</span></span>|<span data-ttu-id="5c1f7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c1f7-154">DateTimeOffset</span></span>|<span data-ttu-id="5c1f7-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-155">The date and time the app was created.</span></span> <span data-ttu-id="5c1f7-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c1f7-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c1f7-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c1f7-157">lastModifiedDateTime</span></span>|<span data-ttu-id="5c1f7-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c1f7-158">DateTimeOffset</span></span>|<span data-ttu-id="5c1f7-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-159">The date and time the app was last modified.</span></span> <span data-ttu-id="5c1f7-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c1f7-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c1f7-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5c1f7-161">isFeatured</span></span>|<span data-ttu-id="5c1f7-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c1f7-162">Boolean</span></span>|<span data-ttu-id="5c1f7-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c1f7-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c1f7-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5c1f7-164">privacyInformationUrl</span></span>|<span data-ttu-id="5c1f7-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c1f7-165">String</span></span>|<span data-ttu-id="5c1f7-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-166">The privacy statement Url.</span></span> <span data-ttu-id="5c1f7-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c1f7-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c1f7-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5c1f7-168">informationUrl</span></span>|<span data-ttu-id="5c1f7-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c1f7-169">String</span></span>|<span data-ttu-id="5c1f7-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-170">The more information Url.</span></span> <span data-ttu-id="5c1f7-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c1f7-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c1f7-172">owner</span><span class="sxs-lookup"><span data-stu-id="5c1f7-172">owner</span></span>|<span data-ttu-id="5c1f7-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c1f7-173">String</span></span>|<span data-ttu-id="5c1f7-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-174">The owner of the app.</span></span> <span data-ttu-id="5c1f7-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c1f7-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c1f7-176">developer</span><span class="sxs-lookup"><span data-stu-id="5c1f7-176">developer</span></span>|<span data-ttu-id="5c1f7-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c1f7-177">String</span></span>|<span data-ttu-id="5c1f7-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-178">The developer of the app.</span></span> <span data-ttu-id="5c1f7-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c1f7-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c1f7-180">notes</span><span class="sxs-lookup"><span data-stu-id="5c1f7-180">notes</span></span>|<span data-ttu-id="5c1f7-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c1f7-181">String</span></span>|<span data-ttu-id="5c1f7-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-182">Notes for the app.</span></span> <span data-ttu-id="5c1f7-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c1f7-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c1f7-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="5c1f7-184">uploadState</span></span>|<span data-ttu-id="5c1f7-185">Int32</span><span class="sxs-lookup"><span data-stu-id="5c1f7-185">Int32</span></span>|<span data-ttu-id="5c1f7-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-186">The upload state.</span></span> <span data-ttu-id="5c1f7-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c1f7-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c1f7-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="5c1f7-188">publishingState</span></span>|[<span data-ttu-id="5c1f7-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="5c1f7-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="5c1f7-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-190">The publishing state for the app.</span></span> <span data-ttu-id="5c1f7-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5c1f7-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c1f7-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="5c1f7-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5c1f7-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="5c1f7-194">isAssigned</span></span>|<span data-ttu-id="5c1f7-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c1f7-195">Boolean</span></span>|<span data-ttu-id="5c1f7-196">Der Wert, der angibt, ob die app mindestens eine Gruppe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="5c1f7-197">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c1f7-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c1f7-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5c1f7-198">roleScopeTagIds</span></span>|<span data-ttu-id="5c1f7-199">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="5c1f7-199">String collection</span></span>|<span data-ttu-id="5c1f7-200">Liste der Bereichs-Tag-Ids für diese mobile app.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="5c1f7-201">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c1f7-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c1f7-202">appAvailability</span><span class="sxs-lookup"><span data-stu-id="5c1f7-202">appAvailability</span></span>|[<span data-ttu-id="5c1f7-203">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="5c1f7-203">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="5c1f7-204">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-204">The Application's availability.</span></span> <span data-ttu-id="5c1f7-205">Geerbt von [ManagedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c1f7-205">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="5c1f7-206">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-206">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="5c1f7-207">version</span><span class="sxs-lookup"><span data-stu-id="5c1f7-207">version</span></span>|<span data-ttu-id="5c1f7-208">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c1f7-208">String</span></span>|<span data-ttu-id="5c1f7-209">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-209">The Application's version.</span></span> <span data-ttu-id="5c1f7-210">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="5c1f7-210">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="5c1f7-211">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="5c1f7-211">committedContentVersion</span></span>|<span data-ttu-id="5c1f7-212">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c1f7-212">String</span></span>|<span data-ttu-id="5c1f7-213">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-213">The internal committed content version.</span></span> <span data-ttu-id="5c1f7-214">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c1f7-214">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="5c1f7-215">fileName</span><span class="sxs-lookup"><span data-stu-id="5c1f7-215">fileName</span></span>|<span data-ttu-id="5c1f7-216">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c1f7-216">String</span></span>|<span data-ttu-id="5c1f7-217">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-217">The name of the main Lob application file.</span></span> <span data-ttu-id="5c1f7-218">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c1f7-218">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="5c1f7-219">size</span><span class="sxs-lookup"><span data-stu-id="5c1f7-219">size</span></span>|<span data-ttu-id="5c1f7-220">Int64</span><span class="sxs-lookup"><span data-stu-id="5c1f7-220">Int64</span></span>|<span data-ttu-id="5c1f7-221">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-221">The total size, including all uploaded files.</span></span> <span data-ttu-id="5c1f7-222">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="5c1f7-222">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="5c1f7-223">bundleId</span><span class="sxs-lookup"><span data-stu-id="5c1f7-223">bundleId</span></span>|<span data-ttu-id="5c1f7-224">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c1f7-224">String</span></span>|<span data-ttu-id="5c1f7-225">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="5c1f7-225">The Identity Name.</span></span>|
|<span data-ttu-id="5c1f7-226">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="5c1f7-226">applicableDeviceType</span></span>|[<span data-ttu-id="5c1f7-227">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="5c1f7-227">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="5c1f7-228">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-228">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="5c1f7-229">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5c1f7-229">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="5c1f7-230">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5c1f7-230">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="5c1f7-231">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-231">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="5c1f7-232">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5c1f7-232">expirationDateTime</span></span>|<span data-ttu-id="5c1f7-233">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c1f7-233">DateTimeOffset</span></span>|<span data-ttu-id="5c1f7-234">Das Ablaufdatum.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-234">The expiration time.</span></span>|
|<span data-ttu-id="5c1f7-235">versionNumber</span><span class="sxs-lookup"><span data-stu-id="5c1f7-235">versionNumber</span></span>|<span data-ttu-id="5c1f7-236">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c1f7-236">String</span></span>|<span data-ttu-id="5c1f7-237">Die Versionsnummer der verwalteten branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-237">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="5c1f7-238">buildNumber</span><span class="sxs-lookup"><span data-stu-id="5c1f7-238">buildNumber</span></span>|<span data-ttu-id="5c1f7-239">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c1f7-239">String</span></span>|<span data-ttu-id="5c1f7-240">Die Buildnummer der verwalteten branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-240">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="5c1f7-241">identityVersion</span><span class="sxs-lookup"><span data-stu-id="5c1f7-241">identityVersion</span></span>|<span data-ttu-id="5c1f7-242">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5c1f7-242">String</span></span>|<span data-ttu-id="5c1f7-243">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="5c1f7-243">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="5c1f7-244">Antwort</span><span class="sxs-lookup"><span data-stu-id="5c1f7-244">Response</span></span>
<span data-ttu-id="5c1f7-245">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-245">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c1f7-246">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5c1f7-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c1f7-247">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5c1f7-247">Request</span></span>
<span data-ttu-id="5c1f7-248">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-248">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1442

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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
  "bundleId": "Bundle Id value",
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
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="5c1f7-249">Antwort</span><span class="sxs-lookup"><span data-stu-id="5c1f7-249">Response</span></span>
<span data-ttu-id="5c1f7-p124">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5c1f7-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1614

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
  "bundleId": "Bundle Id value",
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
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```




