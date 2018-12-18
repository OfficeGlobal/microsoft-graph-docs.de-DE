---
title: Abrufen von „windows10MobileCompliancePolicy“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs windows10MobileCompliancePolicy.
author: tfitzmac
ms.openlocfilehash: e30e61c0e50696079de267debfd9f43da70ed8f4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336134"
---
# <a name="get-windows10mobilecompliancepolicy"></a><span data-ttu-id="b8028-103">Abrufen von „windows10MobileCompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="b8028-103">Get windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="b8028-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b8028-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8028-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b8028-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8028-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b8028-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8028-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b8028-107">Read properties and relationships of the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b8028-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b8028-108">Prerequisites</span></span>
<span data-ttu-id="b8028-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8028-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8028-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b8028-111">Permission type</span></span>|<span data-ttu-id="b8028-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b8028-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8028-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b8028-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b8028-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8028-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b8028-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b8028-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8028-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8028-116">Not supported.</span></span>|
|<span data-ttu-id="b8028-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b8028-117">Application</span></span>|<span data-ttu-id="b8028-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8028-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8028-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8028-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b8028-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b8028-120">Optional query parameters</span></span>
<span data-ttu-id="b8028-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b8028-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b8028-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b8028-122">Request headers</span></span>
|<span data-ttu-id="b8028-123">Header</span><span class="sxs-lookup"><span data-stu-id="b8028-123">Header</span></span>|<span data-ttu-id="b8028-124">Wert</span><span class="sxs-lookup"><span data-stu-id="b8028-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8028-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b8028-125">Authorization</span></span>|<span data-ttu-id="b8028-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b8028-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8028-127">Accept</span><span class="sxs-lookup"><span data-stu-id="b8028-127">Accept</span></span>|<span data-ttu-id="b8028-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b8028-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8028-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b8028-129">Request body</span></span>
<span data-ttu-id="b8028-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b8028-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8028-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8028-131">Response</span></span>
<span data-ttu-id="b8028-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b8028-132">If successful, this method returns a `200 OK` response code and [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8028-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b8028-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="b8028-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8028-134">Request</span></span>
<span data-ttu-id="b8028-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b8028-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="b8028-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8028-136">Response</span></span>
<span data-ttu-id="b8028-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8028-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1419

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "3d4237b0-37b0-3d42-b037-423db037423d",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordRequired": true,
    "passwordBlockSimple": true,
    "passwordMinimumLength": 5,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "passwordExpirationDays": 6,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordRequireToUnlockFromIdle": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "earlyLaunchAntiMalwareDriverEnabled": true,
    "bitLockerEnabled": true,
    "secureBootEnabled": true,
    "codeIntegrityEnabled": true,
    "storageRequireEncryption": true,
    "activeFirewallRequired": true,
    "validOperatingSystemBuildRanges": [
      {
        "@odata.type": "microsoft.graph.operatingSystemVersionRange",
        "description": "Description value",
        "lowestVersion": "Lowest Version value",
        "highestVersion": "Highest Version value"
      }
    ]
  }
}
```





