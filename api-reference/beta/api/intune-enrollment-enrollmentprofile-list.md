---
title: EnrollmentProfiles aufListen
description: AufListen von Eigenschaften und Beziehungen der enrollmentProfile-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3853beab83f8d61d068ab3d016ec6afa76f0accd
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30987839"
---
# <a name="list-enrollmentprofiles"></a><span data-ttu-id="77d59-103">EnrollmentProfiles aufListen</span><span class="sxs-lookup"><span data-stu-id="77d59-103">List enrollmentProfiles</span></span>

> <span data-ttu-id="77d59-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="77d59-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77d59-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="77d59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77d59-106">AufListen von Eigenschaften und Beziehungen der [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="77d59-106">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77d59-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="77d59-107">Prerequisites</span></span>
<span data-ttu-id="77d59-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77d59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77d59-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="77d59-110">Permission type</span></span>|<span data-ttu-id="77d59-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="77d59-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77d59-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="77d59-112">Delegated (work or school account)</span></span>|<span data-ttu-id="77d59-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="77d59-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="77d59-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="77d59-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77d59-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77d59-115">Not supported.</span></span>|
|<span data-ttu-id="77d59-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="77d59-116">Application</span></span>|<span data-ttu-id="77d59-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="77d59-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77d59-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="77d59-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="77d59-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="77d59-119">Request headers</span></span>
|<span data-ttu-id="77d59-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="77d59-120">Header</span></span>|<span data-ttu-id="77d59-121">Wert</span><span class="sxs-lookup"><span data-stu-id="77d59-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77d59-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="77d59-122">Authorization</span></span>|<span data-ttu-id="77d59-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="77d59-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77d59-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="77d59-124">Accept</span></span>|<span data-ttu-id="77d59-125">application/json</span><span class="sxs-lookup"><span data-stu-id="77d59-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77d59-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="77d59-126">Request body</span></span>
<span data-ttu-id="77d59-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="77d59-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77d59-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="77d59-128">Response</span></span>
<span data-ttu-id="77d59-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="77d59-129">If successful, this method returns a `200 OK` response code and a collection of [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77d59-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="77d59-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="77d59-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="77d59-131">Request</span></span>
<span data-ttu-id="77d59-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="77d59-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="77d59-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="77d59-133">Response</span></span>
<span data-ttu-id="77d59-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="77d59-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 484

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enrollmentProfile",
      "id": "012d8d5e-8d5e-012d-5e8d-2d015e8d2d01",
      "displayName": "Display Name value",
      "description": "Description value",
      "requiresUserAuthentication": true,
      "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
      "enableAuthenticationViaCompanyPortal": true,
      "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
    }
  ]
}
```




