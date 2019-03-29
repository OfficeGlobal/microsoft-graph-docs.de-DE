---
title: Abrufen von „windows81GeneralConfiguration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs windows81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 48b251abe0626048109271894ff24e6c87c2a5f5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958137"
---
# <a name="get-windows81generalconfiguration"></a><span data-ttu-id="30dd6-103">Abrufen von „windows81GeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="30dd6-103">Get windows81GeneralConfiguration</span></span>

> <span data-ttu-id="30dd6-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="30dd6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30dd6-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="30dd6-105">Read properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30dd6-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="30dd6-106">Prerequisites</span></span>
<span data-ttu-id="30dd6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30dd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30dd6-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="30dd6-109">Permission type</span></span>|<span data-ttu-id="30dd6-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="30dd6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30dd6-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="30dd6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="30dd6-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="30dd6-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="30dd6-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="30dd6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30dd6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="30dd6-114">Not supported.</span></span>|
|<span data-ttu-id="30dd6-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="30dd6-115">Application</span></span>|<span data-ttu-id="30dd6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="30dd6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30dd6-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="30dd6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="30dd6-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="30dd6-118">Optional query parameters</span></span>
<span data-ttu-id="30dd6-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="30dd6-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30dd6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="30dd6-120">Request headers</span></span>
|<span data-ttu-id="30dd6-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="30dd6-121">Header</span></span>|<span data-ttu-id="30dd6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="30dd6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30dd6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="30dd6-123">Authorization</span></span>|<span data-ttu-id="30dd6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="30dd6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30dd6-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="30dd6-125">Accept</span></span>|<span data-ttu-id="30dd6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30dd6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30dd6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="30dd6-127">Request body</span></span>
<span data-ttu-id="30dd6-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="30dd6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30dd6-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="30dd6-129">Response</span></span>
<span data-ttu-id="30dd6-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="30dd6-130">If successful, this method returns a `200 OK` response code and [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30dd6-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="30dd6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="30dd6-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="30dd6-132">Request</span></span>
<span data-ttu-id="30dd6-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="30dd6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="30dd6-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="30dd6-134">Response</span></span>
<span data-ttu-id="30dd6-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="30dd6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1964

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
    "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "accountsBlockAddingNonMicrosoftAccountEmail": true,
    "applyOnlyToWindows81": true,
    "browserBlockAutofill": true,
    "browserBlockAutomaticDetectionOfIntranetSites": true,
    "browserBlockEnterpriseModeAccess": true,
    "browserBlockJavaScript": true,
    "browserBlockPlugins": true,
    "browserBlockPopups": true,
    "browserBlockSendingDoNotTrackHeader": true,
    "browserBlockSingleWordEntryOnIntranetSites": true,
    "browserRequireSmartScreen": true,
    "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
    "browserInternetSecurityLevel": "medium",
    "browserIntranetSecurityLevel": "low",
    "browserLoggingReportLocation": "Browser Logging Report Location value",
    "browserRequireHighSecurityForRestrictedSites": true,
    "browserRequireFirewall": true,
    "browserRequireFraudWarning": true,
    "browserTrustedSitesSecurityLevel": "low",
    "cellularBlockDataRoaming": true,
    "diagnosticsBlockDataSubmission": true,
    "passwordBlockPicturePasswordAndPin": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordMinimumCharacterSetCount": 0,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordRequiredType": "alphanumeric",
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "storageRequireDeviceEncryption": true,
    "updatesRequireAutomaticUpdates": true,
    "userAccountControlSettings": "alwaysNotify",
    "workFoldersUrl": "https://example.com/workFoldersUrl/"
  }
}
```



