---
title: managedIOSLobApp aktualisieren
description: Aktualisieren der Eigenschaften eines managedIOSLobApp-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aa276827960b0ac0b73489402ac7ba309c58c098
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412926"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="a2b05-103">managedIOSLobApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a2b05-103">Update managedIOSLobApp</span></span>

> <span data-ttu-id="a2b05-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="a2b05-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a2b05-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a2b05-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a2b05-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a2b05-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2b05-107">Aktualisieren der Eigenschaften eines [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="a2b05-107">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2b05-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a2b05-108">Prerequisites</span></span>
<span data-ttu-id="a2b05-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a2b05-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a2b05-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a2b05-111">Permission type</span></span>|<span data-ttu-id="a2b05-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a2b05-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2b05-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a2b05-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2b05-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2b05-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a2b05-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a2b05-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2b05-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2b05-116">Not supported.</span></span>|
|<span data-ttu-id="a2b05-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a2b05-117">Application</span></span>|<span data-ttu-id="a2b05-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a2b05-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2b05-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2b05-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="a2b05-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a2b05-120">Request headers</span></span>
|<span data-ttu-id="a2b05-121">Header</span><span class="sxs-lookup"><span data-stu-id="a2b05-121">Header</span></span>|<span data-ttu-id="a2b05-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a2b05-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2b05-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a2b05-123">Authorization</span></span>|<span data-ttu-id="a2b05-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a2b05-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2b05-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a2b05-125">Accept</span></span>|<span data-ttu-id="a2b05-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2b05-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2b05-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a2b05-127">Request body</span></span>
<span data-ttu-id="a2b05-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="a2b05-128">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="a2b05-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="a2b05-129">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="a2b05-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a2b05-130">Property</span></span>|<span data-ttu-id="a2b05-131">Typ</span><span class="sxs-lookup"><span data-stu-id="a2b05-131">Type</span></span>|<span data-ttu-id="a2b05-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a2b05-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2b05-133">id</span><span class="sxs-lookup"><span data-stu-id="a2b05-133">id</span></span>|<span data-ttu-id="a2b05-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2b05-134">String</span></span>|<span data-ttu-id="a2b05-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a2b05-135">Key of the entity.</span></span> <span data-ttu-id="a2b05-136">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2b05-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2b05-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a2b05-137">displayName</span></span>|<span data-ttu-id="a2b05-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2b05-138">String</span></span>|<span data-ttu-id="a2b05-139">Der vom Administrator bereitgestellte oder importierte Titel der App.</span><span class="sxs-lookup"><span data-stu-id="a2b05-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a2b05-140">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2b05-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2b05-141">description</span><span class="sxs-lookup"><span data-stu-id="a2b05-141">description</span></span>|<span data-ttu-id="a2b05-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2b05-142">String</span></span>|<span data-ttu-id="a2b05-143">Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="a2b05-143">The description of the app.</span></span> <span data-ttu-id="a2b05-144">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2b05-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2b05-145">publisher</span><span class="sxs-lookup"><span data-stu-id="a2b05-145">publisher</span></span>|<span data-ttu-id="a2b05-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2b05-146">String</span></span>|<span data-ttu-id="a2b05-147">Der Herausgeber der App.</span><span class="sxs-lookup"><span data-stu-id="a2b05-147">The publisher of the app.</span></span> <span data-ttu-id="a2b05-148">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2b05-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2b05-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a2b05-149">largeIcon</span></span>|[<span data-ttu-id="a2b05-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a2b05-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a2b05-151">Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="a2b05-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a2b05-152">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2b05-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2b05-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2b05-153">createdDateTime</span></span>|<span data-ttu-id="a2b05-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2b05-154">DateTimeOffset</span></span>|<span data-ttu-id="a2b05-155">Datum und Uhrzeit der Erstellung der App.</span><span class="sxs-lookup"><span data-stu-id="a2b05-155">The date and time the app was created.</span></span> <span data-ttu-id="a2b05-156">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2b05-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2b05-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2b05-157">lastModifiedDateTime</span></span>|<span data-ttu-id="a2b05-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2b05-158">DateTimeOffset</span></span>|<span data-ttu-id="a2b05-159">Datum und Uhrzeit der letzten Änderung der App.</span><span class="sxs-lookup"><span data-stu-id="a2b05-159">The date and time the app was last modified.</span></span> <span data-ttu-id="a2b05-160">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2b05-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2b05-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a2b05-161">isFeatured</span></span>|<span data-ttu-id="a2b05-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2b05-162">Boolean</span></span>|<span data-ttu-id="a2b05-163">Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2b05-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2b05-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a2b05-164">privacyInformationUrl</span></span>|<span data-ttu-id="a2b05-165">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2b05-165">String</span></span>|<span data-ttu-id="a2b05-166">URL zur Datenschutzerklärung.</span><span class="sxs-lookup"><span data-stu-id="a2b05-166">The privacy statement Url.</span></span> <span data-ttu-id="a2b05-167">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2b05-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2b05-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a2b05-168">informationUrl</span></span>|<span data-ttu-id="a2b05-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2b05-169">String</span></span>|<span data-ttu-id="a2b05-170">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="a2b05-170">The more information Url.</span></span> <span data-ttu-id="a2b05-171">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2b05-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2b05-172">owner</span><span class="sxs-lookup"><span data-stu-id="a2b05-172">owner</span></span>|<span data-ttu-id="a2b05-173">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2b05-173">String</span></span>|<span data-ttu-id="a2b05-174">Der Besitzer der App.</span><span class="sxs-lookup"><span data-stu-id="a2b05-174">The owner of the app.</span></span> <span data-ttu-id="a2b05-175">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2b05-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2b05-176">developer</span><span class="sxs-lookup"><span data-stu-id="a2b05-176">developer</span></span>|<span data-ttu-id="a2b05-177">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2b05-177">String</span></span>|<span data-ttu-id="a2b05-178">Der Entwickler der App.</span><span class="sxs-lookup"><span data-stu-id="a2b05-178">The developer of the app.</span></span> <span data-ttu-id="a2b05-179">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2b05-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2b05-180">notes</span><span class="sxs-lookup"><span data-stu-id="a2b05-180">notes</span></span>|<span data-ttu-id="a2b05-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2b05-181">String</span></span>|<span data-ttu-id="a2b05-182">Hinweise zur App.</span><span class="sxs-lookup"><span data-stu-id="a2b05-182">Notes for the app.</span></span> <span data-ttu-id="a2b05-183">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2b05-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2b05-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="a2b05-184">uploadState</span></span>|<span data-ttu-id="a2b05-185">Int32</span><span class="sxs-lookup"><span data-stu-id="a2b05-185">Int32</span></span>|<span data-ttu-id="a2b05-186">Der Upload-Zustand.</span><span class="sxs-lookup"><span data-stu-id="a2b05-186">The upload state.</span></span> <span data-ttu-id="a2b05-187">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2b05-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2b05-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="a2b05-188">publishingState</span></span>|[<span data-ttu-id="a2b05-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a2b05-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a2b05-190">Der Veröffentlichungsstatus der App.</span><span class="sxs-lookup"><span data-stu-id="a2b05-190">The publishing state for the app.</span></span> <span data-ttu-id="a2b05-191">Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="a2b05-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a2b05-192">Geerbt von [MobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2b05-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a2b05-193">Mögliche Werte sind: `notPublished`, `processing` und `published`.</span><span class="sxs-lookup"><span data-stu-id="a2b05-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a2b05-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a2b05-194">isAssigned</span></span>|<span data-ttu-id="a2b05-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2b05-195">Boolean</span></span>|<span data-ttu-id="a2b05-196">Der Wert, der angibt, ob die app mindestens eine Gruppe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="a2b05-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="a2b05-197">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2b05-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2b05-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a2b05-198">roleScopeTagIds</span></span>|<span data-ttu-id="a2b05-199">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="a2b05-199">String collection</span></span>|<span data-ttu-id="a2b05-200">Liste der Bereichs-Tag-Ids für diese mobile app.</span><span class="sxs-lookup"><span data-stu-id="a2b05-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="a2b05-201">Geerbt von [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2b05-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a2b05-202">appAvailability</span><span class="sxs-lookup"><span data-stu-id="a2b05-202">appAvailability</span></span>|[<span data-ttu-id="a2b05-203">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="a2b05-203">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="a2b05-204">Die Verfügbarkeit der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="a2b05-204">The Application's availability.</span></span> <span data-ttu-id="a2b05-205">Geerbt von [ManagedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2b05-205">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="a2b05-206">Mögliche Werte: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="a2b05-206">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="a2b05-207">version</span><span class="sxs-lookup"><span data-stu-id="a2b05-207">version</span></span>|<span data-ttu-id="a2b05-208">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2b05-208">String</span></span>|<span data-ttu-id="a2b05-209">Die Version der Anwendung.</span><span class="sxs-lookup"><span data-stu-id="a2b05-209">The Application's version.</span></span> <span data-ttu-id="a2b05-210">Geerbt von [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="a2b05-210">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="a2b05-211">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="a2b05-211">committedContentVersion</span></span>|<span data-ttu-id="a2b05-212">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2b05-212">String</span></span>|<span data-ttu-id="a2b05-213">Die interne zugesicherte Inhaltsversion.</span><span class="sxs-lookup"><span data-stu-id="a2b05-213">The internal committed content version.</span></span> <span data-ttu-id="a2b05-214">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2b05-214">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="a2b05-215">fileName</span><span class="sxs-lookup"><span data-stu-id="a2b05-215">fileName</span></span>|<span data-ttu-id="a2b05-216">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2b05-216">String</span></span>|<span data-ttu-id="a2b05-217">Name der Hauptdatei der Branchenanwendung.</span><span class="sxs-lookup"><span data-stu-id="a2b05-217">The name of the main Lob application file.</span></span> <span data-ttu-id="a2b05-218">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2b05-218">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="a2b05-219">size</span><span class="sxs-lookup"><span data-stu-id="a2b05-219">size</span></span>|<span data-ttu-id="a2b05-220">Int64</span><span class="sxs-lookup"><span data-stu-id="a2b05-220">Int64</span></span>|<span data-ttu-id="a2b05-221">Gesamtgröße einschließlich aller hochgeladenen Dateien.</span><span class="sxs-lookup"><span data-stu-id="a2b05-221">The total size, including all uploaded files.</span></span> <span data-ttu-id="a2b05-222">Geerbt von [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a2b05-222">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="a2b05-223">bundleId</span><span class="sxs-lookup"><span data-stu-id="a2b05-223">bundleId</span></span>|<span data-ttu-id="a2b05-224">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2b05-224">String</span></span>|<span data-ttu-id="a2b05-225">Identitätsname</span><span class="sxs-lookup"><span data-stu-id="a2b05-225">The Identity Name.</span></span>|
|<span data-ttu-id="a2b05-226">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="a2b05-226">applicableDeviceType</span></span>|[<span data-ttu-id="a2b05-227">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="a2b05-227">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="a2b05-228">Die iOS-Architektur, für die diese App ausgeführt werden kann.</span><span class="sxs-lookup"><span data-stu-id="a2b05-228">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="a2b05-229">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a2b05-229">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="a2b05-230">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a2b05-230">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="a2b05-231">Der Wert für die Mindestversion des verwendbaren Betriebssystems.</span><span class="sxs-lookup"><span data-stu-id="a2b05-231">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="a2b05-232">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a2b05-232">expirationDateTime</span></span>|<span data-ttu-id="a2b05-233">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2b05-233">DateTimeOffset</span></span>|<span data-ttu-id="a2b05-234">Das Ablaufdatum.</span><span class="sxs-lookup"><span data-stu-id="a2b05-234">The expiration time.</span></span>|
|<span data-ttu-id="a2b05-235">versionNumber</span><span class="sxs-lookup"><span data-stu-id="a2b05-235">versionNumber</span></span>|<span data-ttu-id="a2b05-236">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2b05-236">String</span></span>|<span data-ttu-id="a2b05-237">Die Versionsnummer der verwalteten branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="a2b05-237">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="a2b05-238">buildNumber</span><span class="sxs-lookup"><span data-stu-id="a2b05-238">buildNumber</span></span>|<span data-ttu-id="a2b05-239">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2b05-239">String</span></span>|<span data-ttu-id="a2b05-240">Die Buildnummer der verwalteten branchenspezifischen iOS-App.</span><span class="sxs-lookup"><span data-stu-id="a2b05-240">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="a2b05-241">identityVersion</span><span class="sxs-lookup"><span data-stu-id="a2b05-241">identityVersion</span></span>|<span data-ttu-id="a2b05-242">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a2b05-242">String</span></span>|<span data-ttu-id="a2b05-243">Die Version der Identität</span><span class="sxs-lookup"><span data-stu-id="a2b05-243">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="a2b05-244">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2b05-244">Response</span></span>
<span data-ttu-id="a2b05-245">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a2b05-245">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2b05-246">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a2b05-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2b05-247">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2b05-247">Request</span></span>
<span data-ttu-id="a2b05-248">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a2b05-248">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="a2b05-249">Antwort</span><span class="sxs-lookup"><span data-stu-id="a2b05-249">Response</span></span>
<span data-ttu-id="a2b05-p124">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a2b05-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




