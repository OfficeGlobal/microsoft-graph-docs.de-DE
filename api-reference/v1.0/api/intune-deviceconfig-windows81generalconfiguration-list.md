---
title: Auflisten von „windows81GeneralConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windows81GeneralConfiguration auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b0f9e7886b3bb9ce16442162d3c797ba087db042
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262650"
---
# <a name="list-windows81generalconfigurations"></a><span data-ttu-id="5a94b-103">Auflisten von „windows81GeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="5a94b-103">List windows81GeneralConfigurations</span></span>

> <span data-ttu-id="5a94b-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5a94b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a94b-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="5a94b-105">List properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a94b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5a94b-106">Prerequisites</span></span>
<span data-ttu-id="5a94b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5a94b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5a94b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5a94b-109">Permission type</span></span>|<span data-ttu-id="5a94b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5a94b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a94b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5a94b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5a94b-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a94b-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5a94b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5a94b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a94b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a94b-114">Not supported.</span></span>|
|<span data-ttu-id="5a94b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5a94b-115">Application</span></span>|<span data-ttu-id="5a94b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a94b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a94b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a94b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5a94b-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5a94b-118">Request headers</span></span>
|<span data-ttu-id="5a94b-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5a94b-119">Header</span></span>|<span data-ttu-id="5a94b-120">Wert</span><span class="sxs-lookup"><span data-stu-id="5a94b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a94b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a94b-121">Authorization</span></span>|<span data-ttu-id="5a94b-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5a94b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a94b-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5a94b-123">Accept</span></span>|<span data-ttu-id="5a94b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5a94b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a94b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5a94b-125">Request body</span></span>
<span data-ttu-id="5a94b-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5a94b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a94b-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a94b-127">Response</span></span>
<span data-ttu-id="5a94b-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5a94b-128">If successful, this method returns a `200 OK` response code and a collection of [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a94b-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5a94b-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a94b-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a94b-130">Request</span></span>
<span data-ttu-id="5a94b-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5a94b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="5a94b-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a94b-132">Response</span></span>
<span data-ttu-id="5a94b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a94b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2058

{
  "value": [
    {
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
  ]
}
```



