---
title: Ressourcentyp „intuneBrand“
description: „intuneBrand“ enthält Daten, mit denen das Aussehen der Unternehmensportal-Anwendungen und des Endbenutzer-Webportals angepasst wird.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ab8465390b6b0a9e4f35e8a713f082dfb9325eb3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957683"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="fb05b-103">Ressourcentyp „intuneBrand“</span><span class="sxs-lookup"><span data-stu-id="fb05b-103">intuneBrand resource type</span></span>

> <span data-ttu-id="fb05b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fb05b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb05b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fb05b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb05b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fb05b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb05b-107">„intuneBrand“ enthält Daten, mit denen das Aussehen der Unternehmensportal-Anwendungen und des Endbenutzer-Webportals angepasst wird.</span><span class="sxs-lookup"><span data-stu-id="fb05b-107">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>
## <a name="properties"></a><span data-ttu-id="fb05b-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fb05b-108">Properties</span></span>
|<span data-ttu-id="fb05b-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fb05b-109">Property</span></span>|<span data-ttu-id="fb05b-110">Typ</span><span class="sxs-lookup"><span data-stu-id="fb05b-110">Type</span></span>|<span data-ttu-id="fb05b-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fb05b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb05b-112">displayName</span><span class="sxs-lookup"><span data-stu-id="fb05b-112">displayName</span></span>|<span data-ttu-id="fb05b-113">String</span><span class="sxs-lookup"><span data-stu-id="fb05b-113">String</span></span>|<span data-ttu-id="fb05b-114">Unternehmensname/Organisationsname, der Endbenutzern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="fb05b-114">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="fb05b-115">contactITName</span><span class="sxs-lookup"><span data-stu-id="fb05b-115">contactITName</span></span>|<span data-ttu-id="fb05b-116">String</span><span class="sxs-lookup"><span data-stu-id="fb05b-116">String</span></span>|<span data-ttu-id="fb05b-117">Name der für den IT-Support zuständigen Person/Organisation</span><span class="sxs-lookup"><span data-stu-id="fb05b-117">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="fb05b-118">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="fb05b-118">contactITPhoneNumber</span></span>|<span data-ttu-id="fb05b-119">String</span><span class="sxs-lookup"><span data-stu-id="fb05b-119">String</span></span>|<span data-ttu-id="fb05b-120">Telefonnummer der für den IT-Support zuständigen Person/Organisation</span><span class="sxs-lookup"><span data-stu-id="fb05b-120">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="fb05b-121">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="fb05b-121">contactITEmailAddress</span></span>|<span data-ttu-id="fb05b-122">String</span><span class="sxs-lookup"><span data-stu-id="fb05b-122">String</span></span>|<span data-ttu-id="fb05b-123">E-Mail-Adresse der für den IT-Support zuständigen Person/Organisation</span><span class="sxs-lookup"><span data-stu-id="fb05b-123">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="fb05b-124">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="fb05b-124">contactITNotes</span></span>|<span data-ttu-id="fb05b-125">String</span><span class="sxs-lookup"><span data-stu-id="fb05b-125">String</span></span>|<span data-ttu-id="fb05b-126">Textkommentare zu der für den IT-Support zuständigen Person/Organisation</span><span class="sxs-lookup"><span data-stu-id="fb05b-126">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="fb05b-127">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="fb05b-127">privacyUrl</span></span>|<span data-ttu-id="fb05b-128">String</span><span class="sxs-lookup"><span data-stu-id="fb05b-128">String</span></span>|<span data-ttu-id="fb05b-129">URL zur Datenschutzrichtlinie des Unternehmens/der Organisation</span><span class="sxs-lookup"><span data-stu-id="fb05b-129">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="fb05b-130">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="fb05b-130">onlineSupportSiteUrl</span></span>|<span data-ttu-id="fb05b-131">String</span><span class="sxs-lookup"><span data-stu-id="fb05b-131">String</span></span>|<span data-ttu-id="fb05b-132">URL zur IT-Helpdesk-Website des Unternehmens/der Organisation</span><span class="sxs-lookup"><span data-stu-id="fb05b-132">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="fb05b-133">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="fb05b-133">onlineSupportSiteName</span></span>|<span data-ttu-id="fb05b-134">String</span><span class="sxs-lookup"><span data-stu-id="fb05b-134">String</span></span>|<span data-ttu-id="fb05b-135">Anzeigename der IT-Helpdesk-Website des Unternehmens/der Organisation</span><span class="sxs-lookup"><span data-stu-id="fb05b-135">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="fb05b-136">themeColor</span><span class="sxs-lookup"><span data-stu-id="fb05b-136">themeColor</span></span>|[<span data-ttu-id="fb05b-137">rgbColor</span><span class="sxs-lookup"><span data-stu-id="fb05b-137">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="fb05b-138">Primäres Farbdesign für die Unternehmensportal-Anwendungen und das Webportal</span><span class="sxs-lookup"><span data-stu-id="fb05b-138">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="fb05b-139">showLogo</span><span class="sxs-lookup"><span data-stu-id="fb05b-139">showLogo</span></span>|<span data-ttu-id="fb05b-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb05b-140">Boolean</span></span>|<span data-ttu-id="fb05b-141">Boolescher Wert, der angibt, ob die vom Administrator bereitgestellten Logobilder angezeigt werden sollen</span><span class="sxs-lookup"><span data-stu-id="fb05b-141">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="fb05b-142">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="fb05b-142">lightBackgroundLogo</span></span>|[<span data-ttu-id="fb05b-143">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fb05b-143">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fb05b-144">Logobild, das in Unternehmensportal-Apps mit hellem Hintergrund hinter dem Logo angezeigt werden soll</span><span class="sxs-lookup"><span data-stu-id="fb05b-144">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="fb05b-145">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="fb05b-145">darkBackgroundLogo</span></span>|[<span data-ttu-id="fb05b-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fb05b-146">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fb05b-147">Logobild, das in Unternehmensportal-Apps mit dunklem Hintergrund hinter dem Logo angezeigt werden soll</span><span class="sxs-lookup"><span data-stu-id="fb05b-147">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="fb05b-148">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="fb05b-148">showNameNextToLogo</span></span>|<span data-ttu-id="fb05b-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb05b-149">Boolean</span></span>|<span data-ttu-id="fb05b-150">Boolescher Wert, der angibt, ob der vom Administrator angegebene Anzeigename neben dem Logobild angezeigt werden soll</span><span class="sxs-lookup"><span data-stu-id="fb05b-150">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="fb05b-151">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="fb05b-151">landingPageCustomizedImage</span></span>|[<span data-ttu-id="fb05b-152">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fb05b-152">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fb05b-153">Angepasste Bild im Unternehmen Portal-Angebotsseite</span><span class="sxs-lookup"><span data-stu-id="fb05b-153">Customized image displayed in Compnay Portal app landing page</span></span>|
|<span data-ttu-id="fb05b-154">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="fb05b-154">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="fb05b-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb05b-155">Boolean</span></span>|<span data-ttu-id="fb05b-156">Boolescher Wert, der angibt, ob der vom Administrator angegebene Anzeigename neben dem Logobild angezeigt werden soll</span><span class="sxs-lookup"><span data-stu-id="fb05b-156">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb05b-157">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fb05b-157">Relationships</span></span>
<span data-ttu-id="fb05b-158">Keine</span><span class="sxs-lookup"><span data-stu-id="fb05b-158">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fb05b-159">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fb05b-159">JSON Representation</span></span>
<span data-ttu-id="fb05b-160">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fb05b-160">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.intuneBrand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrand",
  "displayName": "String",
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "privacyUrl": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1024,
    "g": 1024,
    "b": 1024
  },
  "showLogo": true,
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "darkBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showNameNextToLogo": true,
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showDisplayNameNextToLogo": true
}
```





