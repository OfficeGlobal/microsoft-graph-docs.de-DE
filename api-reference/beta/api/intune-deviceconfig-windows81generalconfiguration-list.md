---
title: Auflisten von „windows81GeneralConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windows81GeneralConfiguration auf.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8de52c48f773259bca1c959bc1b221ba5537cc4d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425421"
---
# <a name="list-windows81generalconfigurations"></a><span data-ttu-id="4ecf2-103">Auflisten von „windows81GeneralConfiguration“</span><span class="sxs-lookup"><span data-stu-id="4ecf2-103">List windows81GeneralConfigurations</span></span>

> <span data-ttu-id="4ecf2-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="4ecf2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4ecf2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4ecf2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4ecf2-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4ecf2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ecf2-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="4ecf2-107">List properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ecf2-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4ecf2-108">Prerequisites</span></span>
<span data-ttu-id="4ecf2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4ecf2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4ecf2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4ecf2-111">Permission type</span></span>|<span data-ttu-id="4ecf2-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4ecf2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ecf2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4ecf2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4ecf2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ecf2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4ecf2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4ecf2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ecf2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4ecf2-116">Not supported.</span></span>|
|<span data-ttu-id="4ecf2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4ecf2-117">Application</span></span>|<span data-ttu-id="4ecf2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4ecf2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ecf2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ecf2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4ecf2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4ecf2-120">Request headers</span></span>
|<span data-ttu-id="4ecf2-121">Header</span><span class="sxs-lookup"><span data-stu-id="4ecf2-121">Header</span></span>|<span data-ttu-id="4ecf2-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4ecf2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ecf2-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4ecf2-123">Authorization</span></span>|<span data-ttu-id="4ecf2-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4ecf2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ecf2-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4ecf2-125">Accept</span></span>|<span data-ttu-id="4ecf2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4ecf2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ecf2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4ecf2-127">Request body</span></span>
<span data-ttu-id="4ecf2-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4ecf2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ecf2-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ecf2-129">Response</span></span>
<span data-ttu-id="4ecf2-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4ecf2-130">If successful, this method returns a `200 OK` response code and a collection of [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ecf2-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4ecf2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ecf2-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ecf2-132">Request</span></span>
<span data-ttu-id="4ecf2-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4ecf2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="4ecf2-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ecf2-134">Response</span></span>
<span data-ttu-id="4ecf2-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4ecf2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2313

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
      "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
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
      "minimumAutoInstallClassification": "recommendedAndImportant",
      "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
      "updatesRequireAutomaticUpdates": true,
      "userAccountControlSettings": "alwaysNotify",
      "workFoldersUrl": "https://example.com/workFoldersUrl/"
    }
  ]
}
```




