---
title: IosImportedPFXCertificateProfiles aufListen
description: AufListen von Eigenschaften und Beziehungen der iosImportedPFXCertificateProfile-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bdaae1ade08bcee3663dc0ef98580599e6a73412
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967510"
---
# <a name="list-iosimportedpfxcertificateprofiles"></a><span data-ttu-id="9e164-103">IosImportedPFXCertificateProfiles aufListen</span><span class="sxs-lookup"><span data-stu-id="9e164-103">List iosImportedPFXCertificateProfiles</span></span>

> <span data-ttu-id="9e164-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9e164-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e164-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9e164-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e164-106">AufListen von Eigenschaften und Beziehungen der [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="9e164-106">List properties and relationships of the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e164-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9e164-107">Prerequisites</span></span>
<span data-ttu-id="9e164-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e164-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e164-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9e164-110">Permission type</span></span>|<span data-ttu-id="9e164-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9e164-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e164-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9e164-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9e164-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e164-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9e164-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9e164-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e164-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e164-115">Not supported.</span></span>|
|<span data-ttu-id="9e164-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9e164-116">Application</span></span>|<span data-ttu-id="9e164-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e164-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e164-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9e164-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9e164-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9e164-119">Request headers</span></span>
|<span data-ttu-id="9e164-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9e164-120">Header</span></span>|<span data-ttu-id="9e164-121">Wert</span><span class="sxs-lookup"><span data-stu-id="9e164-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e164-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e164-122">Authorization</span></span>|<span data-ttu-id="9e164-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9e164-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e164-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9e164-124">Accept</span></span>|<span data-ttu-id="9e164-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9e164-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e164-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9e164-126">Request body</span></span>
<span data-ttu-id="9e164-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9e164-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e164-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="9e164-128">Response</span></span>
<span data-ttu-id="9e164-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9e164-129">If successful, this method returns a `200 OK` response code and a collection of [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e164-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9e164-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e164-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9e164-131">Request</span></span>
<span data-ttu-id="9e164-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9e164-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="9e164-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="9e164-133">Response</span></span>
<span data-ttu-id="9e164-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9e164-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 556

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosImportedPFXCertificateProfile",
      "id": "583b9d8c-9d8c-583b-8c9d-3b588c9d3b58",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "intendedPurpose": "smimeEncryption"
    }
  ]
}
```




