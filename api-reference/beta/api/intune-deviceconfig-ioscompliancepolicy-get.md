---
title: iosCompliancePolicy abrufen
description: Lesen von Eigenschaften und Beziehungen des iosCompliancePolicy-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c8c5ed3263a85b9f1fa2ddf9c2b10e77fa8fa8f8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877861"
---
# <a name="get-ioscompliancepolicy"></a><span data-ttu-id="c70d5-103">iosCompliancePolicy abrufen</span><span class="sxs-lookup"><span data-stu-id="c70d5-103">Get iosCompliancePolicy</span></span>

> <span data-ttu-id="c70d5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c70d5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c70d5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c70d5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c70d5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c70d5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c70d5-107">Lesen von Eigenschaften und Beziehungen des [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c70d5-107">Read properties and relationships of the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c70d5-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c70d5-108">Prerequisites</span></span>
<span data-ttu-id="c70d5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c70d5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c70d5-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c70d5-111">Permission type</span></span>|<span data-ttu-id="c70d5-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c70d5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c70d5-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c70d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c70d5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c70d5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c70d5-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c70d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c70d5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c70d5-116">Not supported.</span></span>|
|<span data-ttu-id="c70d5-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c70d5-117">Application</span></span>|<span data-ttu-id="c70d5-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c70d5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c70d5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c70d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c70d5-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c70d5-120">Optional query parameters</span></span>
<span data-ttu-id="c70d5-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c70d5-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c70d5-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c70d5-122">Request headers</span></span>
|<span data-ttu-id="c70d5-123">Header</span><span class="sxs-lookup"><span data-stu-id="c70d5-123">Header</span></span>|<span data-ttu-id="c70d5-124">Wert</span><span class="sxs-lookup"><span data-stu-id="c70d5-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c70d5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c70d5-125">Authorization</span></span>|<span data-ttu-id="c70d5-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c70d5-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c70d5-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c70d5-127">Accept</span></span>|<span data-ttu-id="c70d5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c70d5-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c70d5-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c70d5-129">Request body</span></span>
<span data-ttu-id="c70d5-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c70d5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c70d5-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="c70d5-131">Response</span></span>
<span data-ttu-id="c70d5-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c70d5-132">If successful, this method returns a `200 OK` response code and [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c70d5-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c70d5-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="c70d5-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c70d5-134">Request</span></span>
<span data-ttu-id="c70d5-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c70d5-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="c70d5-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="c70d5-136">Response</span></span>
<span data-ttu-id="c70d5-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c70d5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1376

{
  "value": {
    "@odata.type": "#microsoft.graph.iosCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "4f501351-1351-4f50-5113-504f5113504f",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passcodeBlockSimple": true,
    "passcodeExpirationDays": 6,
    "passcodeMinimumLength": 5,
    "passcodeMinutesOfInactivityBeforeLock": 5,
    "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
    "passcodePreviousPasscodeBlockCount": 2,
    "passcodeMinimumCharacterSetCount": 0,
    "passcodeRequiredType": "alphanumeric",
    "passcodeRequired": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "securityBlockJailbrokenDevices": true,
    "deviceThreatProtectionEnabled": true,
    "deviceThreatProtectionRequiredSecurityLevel": "secured",
    "managedEmailProfileRequired": true,
    "restrictedApps": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ]
  }
}
```





