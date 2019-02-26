---
title: IntuneBrandingProfiles aufListen
description: AufListen von Eigenschaften und Beziehungen der intuneBrandingProfile-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9b4a1cbe9492783618dc01ad71bb75749d196a06
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151310"
---
# <a name="list-intunebrandingprofiles"></a><span data-ttu-id="9f060-103">IntuneBrandingProfiles aufListen</span><span class="sxs-lookup"><span data-stu-id="9f060-103">List intuneBrandingProfiles</span></span>

> <span data-ttu-id="9f060-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9f060-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f060-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9f060-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f060-106">AufListen von Eigenschaften und Beziehungen der [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="9f060-106">List properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f060-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9f060-107">Prerequisites</span></span>
<span data-ttu-id="9f060-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9f060-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9f060-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9f060-110">Permission type</span></span>|<span data-ttu-id="9f060-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9f060-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f060-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9f060-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f060-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f060-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9f060-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9f060-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f060-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f060-115">Not supported.</span></span>|
|<span data-ttu-id="9f060-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9f060-116">Application</span></span>|<span data-ttu-id="9f060-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f060-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f060-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f060-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="9f060-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9f060-119">Request headers</span></span>
|<span data-ttu-id="9f060-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9f060-120">Header</span></span>|<span data-ttu-id="9f060-121">Wert</span><span class="sxs-lookup"><span data-stu-id="9f060-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f060-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f060-122">Authorization</span></span>|<span data-ttu-id="9f060-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9f060-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f060-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9f060-124">Accept</span></span>|<span data-ttu-id="9f060-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9f060-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f060-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9f060-126">Request body</span></span>
<span data-ttu-id="9f060-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9f060-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f060-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f060-128">Response</span></span>
<span data-ttu-id="9f060-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9f060-129">If successful, this method returns a `200 OK` response code and a collection of [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f060-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9f060-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f060-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f060-131">Request</span></span>
<span data-ttu-id="9f060-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9f060-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
```

### <a name="response"></a><span data-ttu-id="9f060-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f060-133">Response</span></span>
<span data-ttu-id="9f060-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f060-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




