---
title: WindowsPhone81SCEPCertificateProfile abrufen
description: Lesen von Eigenschaften und Beziehungen des windowsPhone81SCEPCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4fb5ae90e768e644f826289f8e81d32a429a2b35
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143211"
---
# <a name="get-windowsphone81scepcertificateprofile"></a><span data-ttu-id="bed8a-103">WindowsPhone81SCEPCertificateProfile abrufen</span><span class="sxs-lookup"><span data-stu-id="bed8a-103">Get windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="bed8a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bed8a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bed8a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="bed8a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bed8a-106">Lesen von Eigenschaften und Beziehungen des [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="bed8a-106">Read properties and relationships of the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bed8a-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bed8a-107">Prerequisites</span></span>
<span data-ttu-id="bed8a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bed8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bed8a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bed8a-110">Permission type</span></span>|<span data-ttu-id="bed8a-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bed8a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bed8a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bed8a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bed8a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bed8a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bed8a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bed8a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bed8a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bed8a-115">Not supported.</span></span>|
|<span data-ttu-id="bed8a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bed8a-116">Application</span></span>|<span data-ttu-id="bed8a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bed8a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bed8a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bed8a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bed8a-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bed8a-119">Optional query parameters</span></span>
<span data-ttu-id="bed8a-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bed8a-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bed8a-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bed8a-121">Request headers</span></span>
|<span data-ttu-id="bed8a-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bed8a-122">Header</span></span>|<span data-ttu-id="bed8a-123">Wert</span><span class="sxs-lookup"><span data-stu-id="bed8a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bed8a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bed8a-124">Authorization</span></span>|<span data-ttu-id="bed8a-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bed8a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bed8a-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bed8a-126">Accept</span></span>|<span data-ttu-id="bed8a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bed8a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bed8a-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bed8a-128">Request body</span></span>
<span data-ttu-id="bed8a-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bed8a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bed8a-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="bed8a-130">Response</span></span>
<span data-ttu-id="bed8a-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bed8a-131">If successful, this method returns a `200 OK` response code and [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bed8a-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bed8a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="bed8a-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bed8a-133">Request</span></span>
<span data-ttu-id="bed8a-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bed8a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="bed8a-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="bed8a-135">Response</span></span>
<span data-ttu-id="bed8a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bed8a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1287

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
    "id": "f070e30e-e30e-f070-0ee3-70f00ee370f0",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "renewalThresholdPercentage": 10,
    "keyStorageProvider": "useTpmKspOtherwiseFail",
    "subjectNameFormat": "commonNameIncludingEmail",
    "subjectAlternativeNameType": "emailAddress",
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months",
    "extendedKeyUsages": [
      {
        "@odata.type": "microsoft.graph.extendedKeyUsage",
        "name": "Name value",
        "objectIdentifier": "Object Identifier value"
      }
    ],
    "scepServerUrls": [
      "Scep Server Urls value"
    ],
    "subjectNameFormatString": "Subject Name Format String value",
    "keyUsage": "digitalSignature",
    "keySize": "size2048",
    "hashAlgorithm": "sha2",
    "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
  }
}
```




