---
title: Windows10ImportedPFXCertificateProfiles aufListen
description: AufListen von Eigenschaften und Beziehungen der windows10ImportedPFXCertificateProfile-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 815203daa58997a3cf1afcde5700c64748be71d9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167326"
---
# <a name="list-windows10importedpfxcertificateprofiles"></a><span data-ttu-id="b4e56-103">Windows10ImportedPFXCertificateProfiles aufListen</span><span class="sxs-lookup"><span data-stu-id="b4e56-103">List windows10ImportedPFXCertificateProfiles</span></span>

> <span data-ttu-id="b4e56-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b4e56-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4e56-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b4e56-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4e56-106">AufListen von Eigenschaften und Beziehungen der [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="b4e56-106">List properties and relationships of the [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4e56-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b4e56-107">Prerequisites</span></span>
<span data-ttu-id="b4e56-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b4e56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b4e56-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b4e56-110">Permission type</span></span>|<span data-ttu-id="b4e56-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b4e56-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4e56-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b4e56-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b4e56-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4e56-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b4e56-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b4e56-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4e56-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4e56-115">Not supported.</span></span>|
|<span data-ttu-id="b4e56-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b4e56-116">Application</span></span>|<span data-ttu-id="b4e56-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4e56-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4e56-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4e56-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b4e56-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b4e56-119">Request headers</span></span>
|<span data-ttu-id="b4e56-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b4e56-120">Header</span></span>|<span data-ttu-id="b4e56-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b4e56-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4e56-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4e56-122">Authorization</span></span>|<span data-ttu-id="b4e56-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b4e56-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4e56-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b4e56-124">Accept</span></span>|<span data-ttu-id="b4e56-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b4e56-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4e56-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b4e56-126">Request body</span></span>
<span data-ttu-id="b4e56-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b4e56-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4e56-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4e56-128">Response</span></span>
<span data-ttu-id="b4e56-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b4e56-129">If successful, this method returns a `200 OK` response code and a collection of [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4e56-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b4e56-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4e56-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4e56-131">Request</span></span>
<span data-ttu-id="b4e56-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b4e56-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="b4e56-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4e56-133">Response</span></span>
<span data-ttu-id="b4e56-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b4e56-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 863

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10ImportedPFXCertificateProfile",
      "id": "b582514b-514b-b582-4b51-82b54b5182b5",
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
      "intendedPurpose": "smimeEncryption"
    }
  ]
}
```




