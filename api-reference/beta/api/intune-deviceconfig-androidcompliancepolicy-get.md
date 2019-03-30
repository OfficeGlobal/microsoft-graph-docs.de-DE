---
title: Abrufen von „androidCompliancePolicy“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs androidCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6d0799008c563cee4b4b47c7f0475757ff3aacfe
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964717"
---
# <a name="get-androidcompliancepolicy"></a><span data-ttu-id="5017d-103">Abrufen von „androidCompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="5017d-103">Get androidCompliancePolicy</span></span>

> <span data-ttu-id="5017d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5017d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5017d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5017d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5017d-106">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5017d-106">Read properties and relationships of the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5017d-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5017d-107">Prerequisites</span></span>
<span data-ttu-id="5017d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5017d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5017d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5017d-110">Permission type</span></span>|<span data-ttu-id="5017d-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5017d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5017d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5017d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5017d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5017d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5017d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5017d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5017d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5017d-115">Not supported.</span></span>|
|<span data-ttu-id="5017d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5017d-116">Application</span></span>|<span data-ttu-id="5017d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5017d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5017d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5017d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5017d-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5017d-119">Optional query parameters</span></span>
<span data-ttu-id="5017d-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5017d-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5017d-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5017d-121">Request headers</span></span>
|<span data-ttu-id="5017d-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5017d-122">Header</span></span>|<span data-ttu-id="5017d-123">Wert</span><span class="sxs-lookup"><span data-stu-id="5017d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5017d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5017d-124">Authorization</span></span>|<span data-ttu-id="5017d-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5017d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5017d-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5017d-126">Accept</span></span>|<span data-ttu-id="5017d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5017d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5017d-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5017d-128">Request body</span></span>
<span data-ttu-id="5017d-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5017d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5017d-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="5017d-130">Response</span></span>
<span data-ttu-id="5017d-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5017d-131">If successful, this method returns a `200 OK` response code and [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5017d-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5017d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5017d-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5017d-133">Request</span></span>
<span data-ttu-id="5017d-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5017d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="5017d-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="5017d-135">Response</span></span>
<span data-ttu-id="5017d-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5017d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1863

{
  "value": {
    "@odata.type": "#microsoft.graph.androidCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "752c820f-820f-752c-0f82-2c750f822c75",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordRequired": true,
    "passwordMinimumLength": 5,
    "passwordRequiredType": "alphabetic",
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordExpirationDays": 6,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "securityPreventInstallAppsFromUnknownSources": true,
    "securityDisableUsbDebugging": true,
    "securityRequireVerifyApps": true,
    "deviceThreatProtectionEnabled": true,
    "deviceThreatProtectionRequiredSecurityLevel": "secured",
    "securityBlockJailbrokenDevices": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
    "storageRequireEncryption": true,
    "securityRequireSafetyNetAttestationBasicIntegrity": true,
    "securityRequireSafetyNetAttestationCertifiedDevice": true,
    "securityRequireGooglePlayServices": true,
    "securityRequireUpToDateSecurityProviders": true,
    "securityRequireCompanyPortalAppIntegrity": true,
    "conditionStatementId": "Condition Statement Id value",
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




