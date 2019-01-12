---
title: IntuneBrandingProfile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines IntuneBrandingProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0840852d0668cc6e2b4d18b4345792166a2d5193
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964466"
---
# <a name="update-intunebrandingprofile"></a><span data-ttu-id="0d752-103">IntuneBrandingProfile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0d752-103">Update intuneBrandingProfile</span></span>

> <span data-ttu-id="0d752-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0d752-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d752-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0d752-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0d752-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0d752-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0d752-107">Aktualisieren Sie die Eigenschaften eines [IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0d752-107">Update the properties of a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0d752-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0d752-108">Prerequisites</span></span>
<span data-ttu-id="0d752-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d752-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d752-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0d752-111">Permission type</span></span>|<span data-ttu-id="0d752-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0d752-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d752-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0d752-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d752-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d752-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0d752-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0d752-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d752-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d752-116">Not supported.</span></span>|
|<span data-ttu-id="0d752-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0d752-117">Application</span></span>|<span data-ttu-id="0d752-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d752-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d752-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d752-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="0d752-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0d752-120">Request headers</span></span>
|<span data-ttu-id="0d752-121">Header</span><span class="sxs-lookup"><span data-stu-id="0d752-121">Header</span></span>|<span data-ttu-id="0d752-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0d752-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d752-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d752-123">Authorization</span></span>|<span data-ttu-id="0d752-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0d752-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d752-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0d752-125">Accept</span></span>|<span data-ttu-id="0d752-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d752-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d752-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0d752-127">Request body</span></span>
<span data-ttu-id="0d752-128">Geben Sie im Textkörper Anforderung für das Objekt [IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="0d752-128">In the request body, supply a JSON representation for the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

<span data-ttu-id="0d752-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="0d752-129">The following table shows the properties that are required when you create the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span></span>

|<span data-ttu-id="0d752-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0d752-130">Property</span></span>|<span data-ttu-id="0d752-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0d752-131">Type</span></span>|<span data-ttu-id="0d752-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d752-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d752-133">id</span><span class="sxs-lookup"><span data-stu-id="0d752-133">id</span></span>|<span data-ttu-id="0d752-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d752-134">String</span></span>|<span data-ttu-id="0d752-135">Profil-Taste</span><span class="sxs-lookup"><span data-stu-id="0d752-135">Profile Key</span></span>|
|<span data-ttu-id="0d752-136">Profilname</span><span class="sxs-lookup"><span data-stu-id="0d752-136">profileName</span></span>|<span data-ttu-id="0d752-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d752-137">String</span></span>|<span data-ttu-id="0d752-138">Name des Profils</span><span class="sxs-lookup"><span data-stu-id="0d752-138">Name of the profile</span></span>|
|<span data-ttu-id="0d752-139">profileDescription</span><span class="sxs-lookup"><span data-stu-id="0d752-139">profileDescription</span></span>|<span data-ttu-id="0d752-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d752-140">String</span></span>|<span data-ttu-id="0d752-141">Beschreibung des Profils</span><span class="sxs-lookup"><span data-stu-id="0d752-141">Description of the profile</span></span>|
|<span data-ttu-id="0d752-142">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="0d752-142">isDefaultProfile</span></span>|<span data-ttu-id="0d752-143">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0d752-143">Boolean</span></span>|<span data-ttu-id="0d752-144">Zeigt an, wenn das Profil für standardmäßig verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="0d752-144">Presents if the profile is used for default.</span></span>|
|<span data-ttu-id="0d752-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0d752-145">createdDateTime</span></span>|<span data-ttu-id="0d752-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d752-146">DateTimeOffset</span></span>|<span data-ttu-id="0d752-147">Wenn die BrandingProfile erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="0d752-147">When the BrandingProfile was created.</span></span>|
|<span data-ttu-id="0d752-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d752-148">lastModifiedDateTime</span></span>|<span data-ttu-id="0d752-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d752-149">DateTimeOffset</span></span>|<span data-ttu-id="0d752-150">Wann die BrandingProfile zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="0d752-150">When the BrandingProfile was last modified.</span></span>|
|<span data-ttu-id="0d752-151">displayName</span><span class="sxs-lookup"><span data-stu-id="0d752-151">displayName</span></span>|<span data-ttu-id="0d752-152">String</span><span class="sxs-lookup"><span data-stu-id="0d752-152">String</span></span>|<span data-ttu-id="0d752-153">Unternehmensname/Organisationsname, der Endbenutzern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="0d752-153">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="0d752-154">contactITName</span><span class="sxs-lookup"><span data-stu-id="0d752-154">contactITName</span></span>|<span data-ttu-id="0d752-155">String</span><span class="sxs-lookup"><span data-stu-id="0d752-155">String</span></span>|<span data-ttu-id="0d752-156">Name der für den IT-Support zuständigen Person/Organisation</span><span class="sxs-lookup"><span data-stu-id="0d752-156">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="0d752-157">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="0d752-157">contactITPhoneNumber</span></span>|<span data-ttu-id="0d752-158">String</span><span class="sxs-lookup"><span data-stu-id="0d752-158">String</span></span>|<span data-ttu-id="0d752-159">Telefonnummer der für den IT-Support zuständigen Person/Organisation</span><span class="sxs-lookup"><span data-stu-id="0d752-159">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="0d752-160">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="0d752-160">contactITEmailAddress</span></span>|<span data-ttu-id="0d752-161">String</span><span class="sxs-lookup"><span data-stu-id="0d752-161">String</span></span>|<span data-ttu-id="0d752-162">E-Mail-Adresse der für den IT-Support zuständigen Person/Organisation</span><span class="sxs-lookup"><span data-stu-id="0d752-162">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="0d752-163">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="0d752-163">contactITNotes</span></span>|<span data-ttu-id="0d752-164">String</span><span class="sxs-lookup"><span data-stu-id="0d752-164">String</span></span>|<span data-ttu-id="0d752-165">Textkommentare zu der für den IT-Support zuständigen Person/Organisation</span><span class="sxs-lookup"><span data-stu-id="0d752-165">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="0d752-166">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="0d752-166">privacyUrl</span></span>|<span data-ttu-id="0d752-167">String</span><span class="sxs-lookup"><span data-stu-id="0d752-167">String</span></span>|<span data-ttu-id="0d752-168">URL zur Datenschutzrichtlinie des Unternehmens/der Organisation</span><span class="sxs-lookup"><span data-stu-id="0d752-168">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="0d752-169">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="0d752-169">onlineSupportSiteUrl</span></span>|<span data-ttu-id="0d752-170">String</span><span class="sxs-lookup"><span data-stu-id="0d752-170">String</span></span>|<span data-ttu-id="0d752-171">URL zur IT-Helpdesk-Website des Unternehmens/der Organisation</span><span class="sxs-lookup"><span data-stu-id="0d752-171">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="0d752-172">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="0d752-172">onlineSupportSiteName</span></span>|<span data-ttu-id="0d752-173">String</span><span class="sxs-lookup"><span data-stu-id="0d752-173">String</span></span>|<span data-ttu-id="0d752-174">Anzeigename der IT-Helpdesk-Website des Unternehmens/der Organisation</span><span class="sxs-lookup"><span data-stu-id="0d752-174">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="0d752-175">themeColor</span><span class="sxs-lookup"><span data-stu-id="0d752-175">themeColor</span></span>|[<span data-ttu-id="0d752-176">rgbColor</span><span class="sxs-lookup"><span data-stu-id="0d752-176">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="0d752-177">Primäres Farbdesign für die Unternehmensportal-Anwendungen und das Webportal</span><span class="sxs-lookup"><span data-stu-id="0d752-177">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="0d752-178">showLogo</span><span class="sxs-lookup"><span data-stu-id="0d752-178">showLogo</span></span>|<span data-ttu-id="0d752-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d752-179">Boolean</span></span>|<span data-ttu-id="0d752-180">Boolescher Wert, der angibt, ob die vom Administrator bereitgestellten Logobilder angezeigt werden sollen</span><span class="sxs-lookup"><span data-stu-id="0d752-180">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="0d752-181">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="0d752-181">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="0d752-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d752-182">Boolean</span></span>|<span data-ttu-id="0d752-183">Boolescher Wert, der angibt, ob der vom Administrator angegebene Anzeigename neben dem Logobild angezeigt werden soll</span><span class="sxs-lookup"><span data-stu-id="0d752-183">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="0d752-184">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="0d752-184">themeColorLogo</span></span>|[<span data-ttu-id="0d752-185">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0d752-185">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0d752-186">Logo-Bilds im Unternehmensportal apps auf Design farbigen Hintergrund angezeigt.</span><span class="sxs-lookup"><span data-stu-id="0d752-186">Logo image displayed in Company Portal apps on theme color backgrounds.</span></span>|
|<span data-ttu-id="0d752-187">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="0d752-187">lightBackgroundLogo</span></span>|[<span data-ttu-id="0d752-188">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0d752-188">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0d752-189">Logo-Bilds im Unternehmensportal apps heller Hintergrund angezeigt.</span><span class="sxs-lookup"><span data-stu-id="0d752-189">Logo image displayed in Company Portal apps on light backgrounds.</span></span>|
|<span data-ttu-id="0d752-190">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="0d752-190">landingPageCustomizedImage</span></span>|[<span data-ttu-id="0d752-191">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0d752-191">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0d752-192">Angepasste Bild im Unternehmensportal apps Zielseite</span><span class="sxs-lookup"><span data-stu-id="0d752-192">Customized image displayed in Company Portal apps landing page</span></span>|



## <a name="response"></a><span data-ttu-id="0d752-193">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d752-193">Response</span></span>
<span data-ttu-id="0d752-194">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0d752-194">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d752-195">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0d752-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="0d752-196">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d752-196">Request</span></span>
<span data-ttu-id="0d752-197">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0d752-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
Content-type: application/json
Content-length: 1209

{
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```

### <a name="response"></a><span data-ttu-id="0d752-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d752-198">Response</span></span>
<span data-ttu-id="0d752-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0d752-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1377

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "fcd6136c-136c-fcd6-6c13-d6fc6c13d6fc",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```





