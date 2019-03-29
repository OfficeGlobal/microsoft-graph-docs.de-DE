---
title: IosScepCertificateProfiles aufListen
description: AufListen von Eigenschaften und Beziehungen der Iosscepcertificateprofile hinzugefügt-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 87e082784eb2a575b538d3b6938816aeecb8b200
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975399"
---
# <a name="list-iosscepcertificateprofiles"></a><span data-ttu-id="9e2a7-103">IosScepCertificateProfiles aufListen</span><span class="sxs-lookup"><span data-stu-id="9e2a7-103">List iosScepCertificateProfiles</span></span>

> <span data-ttu-id="9e2a7-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e2a7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e2a7-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9e2a7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e2a7-106">AufListen von Eigenschaften und Beziehungen der [iosscepcertificateprofile hinzugefügt](../resources/intune-deviceconfig-iosscepcertificateprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="9e2a7-106">List properties and relationships of the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e2a7-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9e2a7-107">Prerequisites</span></span>
<span data-ttu-id="9e2a7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e2a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e2a7-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9e2a7-110">Permission type</span></span>|<span data-ttu-id="9e2a7-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9e2a7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e2a7-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9e2a7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9e2a7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e2a7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9e2a7-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9e2a7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e2a7-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e2a7-115">Not supported.</span></span>|
|<span data-ttu-id="9e2a7-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9e2a7-116">Application</span></span>|<span data-ttu-id="9e2a7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e2a7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e2a7-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9e2a7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9e2a7-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9e2a7-119">Request headers</span></span>
|<span data-ttu-id="9e2a7-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9e2a7-120">Header</span></span>|<span data-ttu-id="9e2a7-121">Wert</span><span class="sxs-lookup"><span data-stu-id="9e2a7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e2a7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e2a7-122">Authorization</span></span>|<span data-ttu-id="9e2a7-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9e2a7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e2a7-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9e2a7-124">Accept</span></span>|<span data-ttu-id="9e2a7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9e2a7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e2a7-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9e2a7-126">Request body</span></span>
<span data-ttu-id="9e2a7-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9e2a7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e2a7-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="9e2a7-128">Response</span></span>
<span data-ttu-id="9e2a7-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [iosscepcertificateprofile hinzugefügt](../resources/intune-deviceconfig-iosscepcertificateprofile.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9e2a7-129">If successful, this method returns a `200 OK` response code and a collection of [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e2a7-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9e2a7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e2a7-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9e2a7-131">Request</span></span>
<span data-ttu-id="9e2a7-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9e2a7-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="9e2a7-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="9e2a7-133">Response</span></span>
<span data-ttu-id="9e2a7-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9e2a7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1516

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
      "id": "0deb8dbf-8dbf-0deb-bf8d-eb0dbf8deb0d",
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
      "subjectNameFormat": "commonNameAsEmail",
      "subjectAlternativeNameType": "emailAddress",
      "certificateValidityPeriodValue": 14,
      "certificateValidityPeriodScale": "months",
      "scepServerUrls": [
        "Scep Server Urls value"
      ],
      "subjectNameFormatString": "Subject Name Format String value",
      "keyUsage": "digitalSignature",
      "keySize": "size2048",
      "extendedKeyUsages": [
        {
          "@odata.type": "microsoft.graph.extendedKeyUsage",
          "name": "Name value",
          "objectIdentifier": "Object Identifier value"
        }
      ],
      "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
      "certificateStore": "machine",
      "customSubjectAlternativeNames": [
        {
          "@odata.type": "microsoft.graph.customSubjectAlternativeName",
          "sanType": "emailAddress",
          "name": "Name value"
        }
      ]
    }
  ]
}
```




