---
title: Liste iosCertificateProfileBases
description: Listeneigenschaften und Beziehungen der IosCertificateProfileBase-Objekte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 974e8abe750c84fa5dcc82665705c0f884cd15c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836897"
---
# <a name="list-ioscertificateprofilebases"></a><span data-ttu-id="9a399-103">Liste iosCertificateProfileBases</span><span class="sxs-lookup"><span data-stu-id="9a399-103">List iosCertificateProfileBases</span></span>

> <span data-ttu-id="9a399-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9a399-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9a399-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9a399-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9a399-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9a399-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9a399-107">Listeneigenschaften und Beziehungen der [IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="9a399-107">List properties and relationships of the [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9a399-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9a399-108">Prerequisites</span></span>
<span data-ttu-id="9a399-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a399-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a399-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9a399-111">Permission type</span></span>|<span data-ttu-id="9a399-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9a399-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a399-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9a399-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a399-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a399-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9a399-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9a399-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a399-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9a399-116">Not supported.</span></span>|
|<span data-ttu-id="9a399-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9a399-117">Application</span></span>|<span data-ttu-id="9a399-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9a399-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a399-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a399-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9a399-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9a399-120">Request headers</span></span>
|<span data-ttu-id="9a399-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9a399-121">Header</span></span>|<span data-ttu-id="9a399-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9a399-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a399-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a399-123">Authorization</span></span>|<span data-ttu-id="9a399-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9a399-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a399-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9a399-125">Accept</span></span>|<span data-ttu-id="9a399-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a399-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a399-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9a399-127">Request body</span></span>
<span data-ttu-id="9a399-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9a399-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a399-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a399-129">Response</span></span>
<span data-ttu-id="9a399-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [IosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="9a399-130">If successful, this method returns a `200 OK` response code and a collection of [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a399-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9a399-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="9a399-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a399-132">Request</span></span>
<span data-ttu-id="9a399-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9a399-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="9a399-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a399-134">Response</span></span>
<span data-ttu-id="9a399-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9a399-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 743

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCertificateProfileBase",
      "id": "b90209cb-09cb-b902-cb09-02b9cb0902b9",
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
      "certificateValidityPeriodScale": "months"
    }
  ]
}
```





