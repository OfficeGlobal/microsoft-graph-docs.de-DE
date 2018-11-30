---
title: Auflisten von „iosCompliancePolicy“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs iosCompliancePolicy auf.
ms.openlocfilehash: ce993f849e2a42526e04ee68807e340c694ae7b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064496"
---
# <a name="list-ioscompliancepolicies"></a><span data-ttu-id="2ab04-103">Auflisten von „iosCompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="2ab04-103">List iosCompliancePolicies</span></span>

> <span data-ttu-id="2ab04-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2ab04-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2ab04-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2ab04-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2ab04-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2ab04-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ab04-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) auf.</span><span class="sxs-lookup"><span data-stu-id="2ab04-107">List properties and relationships of the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2ab04-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2ab04-108">Prerequisites</span></span>
<span data-ttu-id="2ab04-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ab04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ab04-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2ab04-111">Permission type</span></span>|<span data-ttu-id="2ab04-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2ab04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ab04-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2ab04-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2ab04-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ab04-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2ab04-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2ab04-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ab04-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2ab04-116">Not supported.</span></span>|
|<span data-ttu-id="2ab04-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2ab04-117">Application</span></span>|<span data-ttu-id="2ab04-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2ab04-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ab04-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2ab04-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="2ab04-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2ab04-120">Request headers</span></span>
|<span data-ttu-id="2ab04-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2ab04-121">Header</span></span>|<span data-ttu-id="2ab04-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2ab04-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ab04-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ab04-123">Authorization</span></span>|<span data-ttu-id="2ab04-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2ab04-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ab04-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2ab04-125">Accept</span></span>|<span data-ttu-id="2ab04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2ab04-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ab04-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2ab04-127">Request body</span></span>
<span data-ttu-id="2ab04-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2ab04-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ab04-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="2ab04-129">Response</span></span>
<span data-ttu-id="2ab04-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2ab04-130">If successful, this method returns a `200 OK` response code and a collection of [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ab04-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2ab04-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="2ab04-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2ab04-132">Request</span></span>
<span data-ttu-id="2ab04-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2ab04-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="2ab04-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="2ab04-134">Response</span></span>
<span data-ttu-id="2ab04-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2ab04-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1458

{
  "value": [
    {
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
  ]
}
```





