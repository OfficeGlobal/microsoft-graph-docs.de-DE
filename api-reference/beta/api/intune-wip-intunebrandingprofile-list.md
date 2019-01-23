---
title: Liste intuneBrandingProfiles
description: Listeneigenschaften und Beziehungen der IntuneBrandingProfile-Objekte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 49841c700c24343c0b46b680978cc853acc52fb1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399864"
---
# <a name="list-intunebrandingprofiles"></a><span data-ttu-id="13385-103">Liste intuneBrandingProfiles</span><span class="sxs-lookup"><span data-stu-id="13385-103">List intuneBrandingProfiles</span></span>

> <span data-ttu-id="13385-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="13385-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="13385-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="13385-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="13385-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="13385-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13385-107">Listeneigenschaften und Beziehungen der [IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="13385-107">List properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13385-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="13385-108">Prerequisites</span></span>
<span data-ttu-id="13385-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="13385-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="13385-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="13385-111">Permission type</span></span>|<span data-ttu-id="13385-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="13385-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13385-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="13385-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13385-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="13385-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="13385-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="13385-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13385-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="13385-116">Not supported.</span></span>|
|<span data-ttu-id="13385-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="13385-117">Application</span></span>|<span data-ttu-id="13385-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="13385-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13385-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="13385-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="13385-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="13385-120">Request headers</span></span>
|<span data-ttu-id="13385-121">Header</span><span class="sxs-lookup"><span data-stu-id="13385-121">Header</span></span>|<span data-ttu-id="13385-122">Wert</span><span class="sxs-lookup"><span data-stu-id="13385-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13385-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="13385-123">Authorization</span></span>|<span data-ttu-id="13385-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="13385-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13385-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="13385-125">Accept</span></span>|<span data-ttu-id="13385-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13385-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13385-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="13385-127">Request body</span></span>
<span data-ttu-id="13385-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="13385-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13385-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="13385-129">Response</span></span>
<span data-ttu-id="13385-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="13385-130">If successful, this method returns a `200 OK` response code and a collection of [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13385-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="13385-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="13385-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="13385-132">Request</span></span>
<span data-ttu-id="13385-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="13385-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
```

### <a name="response"></a><span data-ttu-id="13385-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="13385-134">Response</span></span>
<span data-ttu-id="13385-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="13385-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1562

{
  "value": [
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
  ]
}
```




