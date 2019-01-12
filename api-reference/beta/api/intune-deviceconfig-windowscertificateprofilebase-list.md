---
title: Liste windowsCertificateProfileBases
description: Listeneigenschaften und Beziehungen der WindowsCertificateProfileBase-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 458bf035a57d5239e1baf668d6eb4afe62cc47f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914073"
---
# <a name="list-windowscertificateprofilebases"></a><span data-ttu-id="6cd52-103">Liste windowsCertificateProfileBases</span><span class="sxs-lookup"><span data-stu-id="6cd52-103">List windowsCertificateProfileBases</span></span>

> <span data-ttu-id="6cd52-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6cd52-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6cd52-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6cd52-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6cd52-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6cd52-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6cd52-107">Listeneigenschaften und Beziehungen der [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="6cd52-107">List properties and relationships of the [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6cd52-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6cd52-108">Prerequisites</span></span>
<span data-ttu-id="6cd52-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cd52-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cd52-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6cd52-111">Permission type</span></span>|<span data-ttu-id="6cd52-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6cd52-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cd52-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6cd52-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6cd52-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cd52-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6cd52-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6cd52-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cd52-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6cd52-116">Not supported.</span></span>|
|<span data-ttu-id="6cd52-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6cd52-117">Application</span></span>|<span data-ttu-id="6cd52-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6cd52-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cd52-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6cd52-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6cd52-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6cd52-120">Request headers</span></span>
|<span data-ttu-id="6cd52-121">Header</span><span class="sxs-lookup"><span data-stu-id="6cd52-121">Header</span></span>|<span data-ttu-id="6cd52-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6cd52-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cd52-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cd52-123">Authorization</span></span>|<span data-ttu-id="6cd52-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6cd52-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cd52-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6cd52-125">Accept</span></span>|<span data-ttu-id="6cd52-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6cd52-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cd52-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6cd52-127">Request body</span></span>
<span data-ttu-id="6cd52-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6cd52-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6cd52-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="6cd52-129">Response</span></span>
<span data-ttu-id="6cd52-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [WindowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="6cd52-130">If successful, this method returns a `200 OK` response code and a collection of [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cd52-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6cd52-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6cd52-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6cd52-132">Request</span></span>
<span data-ttu-id="6cd52-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6cd52-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="6cd52-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6cd52-134">Response</span></span>
<span data-ttu-id="6cd52-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6cd52-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 809

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsCertificateProfileBase",
      "id": "c0979ce1-9ce1-c097-e19c-97c0e19c97c0",
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
      "certificateValidityPeriodScale": "months"
    }
  ]
}
```





