---
title: Abrufen von windowsIdentityProtectionConfiguration
description: Lesen Sie Eigenschaften und Beziehungen des WindowsIdentityProtectionConfiguration-Objekts.
ms.openlocfilehash: d58532b4a2f1e6b7be3e55548fa7064266e41190
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060089"
---
# <a name="get-windowsidentityprotectionconfiguration"></a><span data-ttu-id="6eb78-103">Abrufen von windowsIdentityProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="6eb78-103">Get windowsIdentityProtectionConfiguration</span></span>

> <span data-ttu-id="6eb78-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6eb78-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6eb78-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6eb78-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6eb78-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6eb78-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6eb78-107">Lesen Sie Eigenschaften und Beziehungen des [WindowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6eb78-107">Read properties and relationships of the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6eb78-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6eb78-108">Prerequisites</span></span>
<span data-ttu-id="6eb78-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6eb78-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6eb78-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6eb78-111">Permission type</span></span>|<span data-ttu-id="6eb78-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6eb78-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6eb78-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6eb78-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6eb78-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6eb78-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6eb78-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6eb78-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6eb78-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6eb78-116">Not supported.</span></span>|
|<span data-ttu-id="6eb78-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6eb78-117">Application</span></span>|<span data-ttu-id="6eb78-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6eb78-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6eb78-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6eb78-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6eb78-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6eb78-120">Optional query parameters</span></span>
<span data-ttu-id="6eb78-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6eb78-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6eb78-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6eb78-122">Request headers</span></span>
|<span data-ttu-id="6eb78-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6eb78-123">Header</span></span>|<span data-ttu-id="6eb78-124">Wert</span><span class="sxs-lookup"><span data-stu-id="6eb78-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6eb78-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6eb78-125">Authorization</span></span>|<span data-ttu-id="6eb78-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6eb78-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6eb78-127">Accept</span><span class="sxs-lookup"><span data-stu-id="6eb78-127">Accept</span></span>|<span data-ttu-id="6eb78-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6eb78-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6eb78-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6eb78-129">Request body</span></span>
<span data-ttu-id="6eb78-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6eb78-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6eb78-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="6eb78-131">Response</span></span>
<span data-ttu-id="6eb78-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [WindowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6eb78-132">If successful, this method returns a `200 OK` response code and [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6eb78-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6eb78-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="6eb78-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6eb78-134">Request</span></span>
<span data-ttu-id="6eb78-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6eb78-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="6eb78-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="6eb78-136">Response</span></span>
<span data-ttu-id="6eb78-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6eb78-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1013

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
    "id": "b2e64303-4303-b2e6-0343-e6b20343e6b2",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
    "pinMinimumLength": 0,
    "pinMaximumLength": 0,
    "pinUppercaseCharactersUsage": "required",
    "pinLowercaseCharactersUsage": "required",
    "pinSpecialCharactersUsage": "required",
    "pinExpirationInDays": 3,
    "pinPreviousBlockCount": 5,
    "pinRecoveryEnabled": true,
    "securityDeviceRequired": true,
    "unlockWithBiometricsEnabled": true,
    "useCertificatesForOnPremisesAuthEnabled": true,
    "windowsHelloForBusinessBlocked": true
  }
}
```





