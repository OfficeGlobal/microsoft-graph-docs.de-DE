---
title: Liste depEnrollmentBaseProfiles
description: Listeneigenschaften und Beziehungen der DepEnrollmentBaseProfile-Objekte.
author: tfitzmac
ms.openlocfilehash: ce7edb9558864323ca08a4379ae0e6e8949c6875
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340957"
---
# <a name="list-depenrollmentbaseprofiles"></a><span data-ttu-id="55237-103">Liste depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="55237-103">List depEnrollmentBaseProfiles</span></span>

> <span data-ttu-id="55237-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="55237-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55237-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="55237-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="55237-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="55237-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55237-107">Listeneigenschaften und Beziehungen der [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="55237-107">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="55237-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="55237-108">Prerequisites</span></span>
<span data-ttu-id="55237-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55237-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55237-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="55237-111">Permission type</span></span>|<span data-ttu-id="55237-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="55237-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55237-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="55237-113">Delegated (work or school account)</span></span>|<span data-ttu-id="55237-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="55237-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="55237-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="55237-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55237-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="55237-116">Not supported.</span></span>|
|<span data-ttu-id="55237-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="55237-117">Application</span></span>|<span data-ttu-id="55237-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="55237-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55237-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="55237-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="55237-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="55237-120">Request headers</span></span>
|<span data-ttu-id="55237-121">Header</span><span class="sxs-lookup"><span data-stu-id="55237-121">Header</span></span>|<span data-ttu-id="55237-122">Wert</span><span class="sxs-lookup"><span data-stu-id="55237-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55237-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="55237-123">Authorization</span></span>|<span data-ttu-id="55237-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="55237-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55237-125">Accept</span><span class="sxs-lookup"><span data-stu-id="55237-125">Accept</span></span>|<span data-ttu-id="55237-126">application/json</span><span class="sxs-lookup"><span data-stu-id="55237-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55237-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="55237-127">Request body</span></span>
<span data-ttu-id="55237-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="55237-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55237-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="55237-129">Response</span></span>
<span data-ttu-id="55237-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="55237-130">If successful, this method returns a `200 OK` response code and a collection of [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55237-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="55237-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="55237-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="55237-132">Request</span></span>
<span data-ttu-id="55237-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="55237-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="55237-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="55237-134">Response</span></span>
<span data-ttu-id="55237-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="55237-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1000

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.depEnrollmentBaseProfile",
      "id": "db378868-8868-db37-6888-37db688837db",
      "displayName": "Display Name value",
      "description": "Description value",
      "requiresUserAuthentication": true,
      "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
      "enableAuthenticationViaCompanyPortal": true,
      "isDefault": true,
      "supervisedModeEnabled": true,
      "supportDepartment": "Support Department value",
      "passCodeDisabled": true,
      "isMandatory": true,
      "locationDisabled": true,
      "supportPhoneNumber": "Support Phone Number value",
      "profileRemovalDisabled": true,
      "restoreBlocked": true,
      "appleIdDisabled": true,
      "termsAndConditionsDisabled": true,
      "touchIdDisabled": true,
      "applePayDisabled": true,
      "zoomDisabled": true,
      "siriDisabled": true,
      "diagnosticsDisabled": true
    }
  ]
}
```





