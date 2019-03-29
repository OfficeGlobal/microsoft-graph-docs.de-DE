---
title: AndroidWorkProfileScepCertificateProfiles aufListen
description: AufListen von Eigenschaften und Beziehungen der androidWorkProfileScepCertificateProfile-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4032f422acd151cd456d425bc5849a7d581dde6d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965746"
---
# <a name="list-androidworkprofilescepcertificateprofiles"></a><span data-ttu-id="025bb-103">AndroidWorkProfileScepCertificateProfiles aufListen</span><span class="sxs-lookup"><span data-stu-id="025bb-103">List androidWorkProfileScepCertificateProfiles</span></span>

> <span data-ttu-id="025bb-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="025bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="025bb-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="025bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="025bb-106">AufListen von Eigenschaften und Beziehungen der [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="025bb-106">List properties and relationships of the [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="025bb-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="025bb-107">Prerequisites</span></span>
<span data-ttu-id="025bb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="025bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="025bb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="025bb-110">Permission type</span></span>|<span data-ttu-id="025bb-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="025bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="025bb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="025bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="025bb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="025bb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="025bb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="025bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="025bb-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="025bb-115">Not supported.</span></span>|
|<span data-ttu-id="025bb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="025bb-116">Application</span></span>|<span data-ttu-id="025bb-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="025bb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="025bb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="025bb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="025bb-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="025bb-119">Request headers</span></span>
|<span data-ttu-id="025bb-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="025bb-120">Header</span></span>|<span data-ttu-id="025bb-121">Wert</span><span class="sxs-lookup"><span data-stu-id="025bb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="025bb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="025bb-122">Authorization</span></span>|<span data-ttu-id="025bb-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="025bb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="025bb-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="025bb-124">Accept</span></span>|<span data-ttu-id="025bb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="025bb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="025bb-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="025bb-126">Request body</span></span>
<span data-ttu-id="025bb-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="025bb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="025bb-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="025bb-128">Response</span></span>
<span data-ttu-id="025bb-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="025bb-129">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileScepCertificateProfile](../resources/intune-deviceconfig-androidworkprofilescepcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="025bb-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="025bb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="025bb-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="025bb-131">Request</span></span>
<span data-ttu-id="025bb-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="025bb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="025bb-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="025bb-133">Response</span></span>
<span data-ttu-id="025bb-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="025bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1570

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileScepCertificateProfile",
      "id": "6f494abf-4abf-6f49-bf4a-496fbf4a496f",
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
      "subjectNameFormat": "commonNameIncludingEmail",
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
      "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
      "certificateStore": "machine",
      "customSubjectAlternativeNames": [
        {
          "@odata.type": "microsoft.graph.customSubjectAlternativeName",
          "sanType": "emailAddress",
          "name": "Name value"
        }
      ],
      "subjectAlternativeNameType": "emailAddress"
    }
  ]
}
```




