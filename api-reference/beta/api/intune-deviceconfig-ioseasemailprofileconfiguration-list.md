---
title: IosEasEmailProfileConfigurations aufListen
description: AufListen von Eigenschaften und Beziehungen der iosEasEmailProfileConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 474f9db71660f7e332127c4a020e120141450250
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975735"
---
# <a name="list-ioseasemailprofileconfigurations"></a><span data-ttu-id="207b1-103">IosEasEmailProfileConfigurations aufListen</span><span class="sxs-lookup"><span data-stu-id="207b1-103">List iosEasEmailProfileConfigurations</span></span>

> <span data-ttu-id="207b1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="207b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="207b1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="207b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="207b1-106">AufListen von Eigenschaften und Beziehungen der [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="207b1-106">List properties and relationships of the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="207b1-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="207b1-107">Prerequisites</span></span>
<span data-ttu-id="207b1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="207b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="207b1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="207b1-110">Permission type</span></span>|<span data-ttu-id="207b1-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="207b1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="207b1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="207b1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="207b1-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="207b1-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="207b1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="207b1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="207b1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="207b1-115">Not supported.</span></span>|
|<span data-ttu-id="207b1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="207b1-116">Application</span></span>|<span data-ttu-id="207b1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="207b1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="207b1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="207b1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="207b1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="207b1-119">Request headers</span></span>
|<span data-ttu-id="207b1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="207b1-120">Header</span></span>|<span data-ttu-id="207b1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="207b1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="207b1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="207b1-122">Authorization</span></span>|<span data-ttu-id="207b1-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="207b1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="207b1-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="207b1-124">Accept</span></span>|<span data-ttu-id="207b1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="207b1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="207b1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="207b1-126">Request body</span></span>
<span data-ttu-id="207b1-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="207b1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="207b1-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="207b1-128">Response</span></span>
<span data-ttu-id="207b1-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="207b1-129">If successful, this method returns a `200 OK` response code and a collection of [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="207b1-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="207b1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="207b1-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="207b1-131">Request</span></span>
<span data-ttu-id="207b1-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="207b1-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="207b1-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="207b1-133">Response</span></span>
<span data-ttu-id="207b1-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="207b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1530

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
      "id": "e03086da-86da-e030-da86-30e0da8630e0",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "usernameSource": "primarySmtpAddress",
      "usernameAADSource": "primarySmtpAddress",
      "userDomainNameSource": "netBiosDomainName",
      "customDomainName": "Custom Domain Name value",
      "accountName": "Account Name value",
      "authenticationMethod": "certificate",
      "blockMovingMessagesToOtherEmailAccounts": true,
      "blockSendingEmailFromThirdPartyApps": true,
      "blockSyncingRecentlyUsedEmailAddresses": true,
      "durationOfEmailToSync": "oneDay",
      "emailAddressSource": "primarySmtpAddress",
      "hostName": "Host Name value",
      "requireSmime": true,
      "smimeEnablePerMessageSwitch": true,
      "smimeEncryptByDefaultEnabled": true,
      "smimeSigningEnabled": true,
      "smimeSigningUserOverrideEnabled": true,
      "smimeEncryptByDefaultUserOverrideEnabled": true,
      "smimeSigningCertificateUserOverrideEnabled": true,
      "smimeEncryptionCertificateUserOverrideEnabled": true,
      "requireSsl": true,
      "useOAuth": true
    }
  ]
}
```




