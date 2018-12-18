---
title: Liste androidForWorkCertificateProfileBases
description: Listeneigenschaften und Beziehungen der AndroidForWorkCertificateProfileBase-Objekte.
author: tfitzmac
ms.openlocfilehash: 2a0bd2de1408ad6fa41bb8b1e7be9d691460ceb9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318158"
---
# <a name="list-androidforworkcertificateprofilebases"></a><span data-ttu-id="beeac-103">Liste androidForWorkCertificateProfileBases</span><span class="sxs-lookup"><span data-stu-id="beeac-103">List androidForWorkCertificateProfileBases</span></span>

> <span data-ttu-id="beeac-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="beeac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="beeac-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="beeac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="beeac-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="beeac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="beeac-107">Listeneigenschaften und Beziehungen der [AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="beeac-107">List properties and relationships of the [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="beeac-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="beeac-108">Prerequisites</span></span>
<span data-ttu-id="beeac-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="beeac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="beeac-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="beeac-111">Permission type</span></span>|<span data-ttu-id="beeac-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="beeac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="beeac-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="beeac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="beeac-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="beeac-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="beeac-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="beeac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="beeac-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="beeac-116">Not supported.</span></span>|
|<span data-ttu-id="beeac-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="beeac-117">Application</span></span>|<span data-ttu-id="beeac-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="beeac-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="beeac-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="beeac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="beeac-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="beeac-120">Request headers</span></span>
|<span data-ttu-id="beeac-121">Header</span><span class="sxs-lookup"><span data-stu-id="beeac-121">Header</span></span>|<span data-ttu-id="beeac-122">Wert</span><span class="sxs-lookup"><span data-stu-id="beeac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="beeac-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="beeac-123">Authorization</span></span>|<span data-ttu-id="beeac-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="beeac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="beeac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="beeac-125">Accept</span></span>|<span data-ttu-id="beeac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="beeac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="beeac-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="beeac-127">Request body</span></span>
<span data-ttu-id="beeac-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="beeac-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="beeac-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="beeac-129">Response</span></span>
<span data-ttu-id="beeac-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="beeac-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="beeac-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="beeac-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="beeac-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="beeac-132">Request</span></span>
<span data-ttu-id="beeac-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="beeac-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="beeac-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="beeac-134">Response</span></span>
<span data-ttu-id="beeac-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="beeac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 922

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkCertificateProfileBase",
      "id": "87f1d53b-d53b-87f1-3bd5-f1873bd5f187",
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
      ]
    }
  ]
}
```





