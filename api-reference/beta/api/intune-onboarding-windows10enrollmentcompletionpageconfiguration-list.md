---
title: Windows10EnrollmentCompletionPageConfigurations aufListen
description: AufListen von Eigenschaften und Beziehungen der windows10EnrollmentCompletionPageConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 294e6db6593e11bf4c4c9e3c1e717892a71b12f8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964332"
---
# <a name="list-windows10enrollmentcompletionpageconfigurations"></a><span data-ttu-id="e0cef-103">Windows10EnrollmentCompletionPageConfigurations aufListen</span><span class="sxs-lookup"><span data-stu-id="e0cef-103">List windows10EnrollmentCompletionPageConfigurations</span></span>

> <span data-ttu-id="e0cef-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e0cef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0cef-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e0cef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0cef-106">AufListen von Eigenschaften und Beziehungen der [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="e0cef-106">List properties and relationships of the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0cef-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e0cef-107">Prerequisites</span></span>
<span data-ttu-id="e0cef-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0cef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0cef-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e0cef-110">Permission type</span></span>|<span data-ttu-id="e0cef-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e0cef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0cef-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e0cef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e0cef-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0cef-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e0cef-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e0cef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0cef-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e0cef-115">Not supported.</span></span>|
|<span data-ttu-id="e0cef-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e0cef-116">Application</span></span>|<span data-ttu-id="e0cef-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e0cef-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0cef-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0cef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e0cef-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e0cef-119">Request headers</span></span>
|<span data-ttu-id="e0cef-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e0cef-120">Header</span></span>|<span data-ttu-id="e0cef-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e0cef-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0cef-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0cef-122">Authorization</span></span>|<span data-ttu-id="e0cef-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e0cef-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0cef-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e0cef-124">Accept</span></span>|<span data-ttu-id="e0cef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e0cef-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0cef-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e0cef-126">Request body</span></span>
<span data-ttu-id="e0cef-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e0cef-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0cef-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0cef-128">Response</span></span>
<span data-ttu-id="e0cef-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e0cef-129">If successful, this method returns a `200 OK` response code and a collection of [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0cef-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e0cef-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0cef-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e0cef-131">Request</span></span>
<span data-ttu-id="e0cef-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e0cef-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="e0cef-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="e0cef-133">Response</span></span>
<span data-ttu-id="e0cef-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e0cef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 860

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
      "id": "77bf8248-8248-77bf-4882-bf774882bf77",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7,
      "showInstallationProgress": true,
      "blockDeviceSetupRetryByUser": true,
      "allowDeviceResetOnInstallFailure": true,
      "allowLogCollectionOnInstallFailure": true,
      "customErrorMessage": "Custom Error Message value",
      "installProgressTimeoutInMinutes": 15,
      "allowDeviceUseOnInstallFailure": true,
      "selectedMobileAppIds": [
        "Selected Mobile App Ids value"
      ]
    }
  ]
}
```




