---
title: Liste iosImportedPFXCertificateProfiles
description: Listeneigenschaften und Beziehungen der IosImportedPFXCertificateProfile-Objekte.
ms.openlocfilehash: 39d2269a63e440fcaeb5e93a82936c3708b1bffe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064493"
---
# <a name="list-iosimportedpfxcertificateprofiles"></a><span data-ttu-id="b44ea-103">Liste iosImportedPFXCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="b44ea-103">List iosImportedPFXCertificateProfiles</span></span>

> <span data-ttu-id="b44ea-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b44ea-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b44ea-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b44ea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b44ea-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b44ea-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b44ea-107">Listeneigenschaften und Beziehungen der [IosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="b44ea-107">List properties and relationships of the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b44ea-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b44ea-108">Prerequisites</span></span>
<span data-ttu-id="b44ea-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b44ea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b44ea-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b44ea-111">Permission type</span></span>|<span data-ttu-id="b44ea-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b44ea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b44ea-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b44ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b44ea-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b44ea-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b44ea-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b44ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b44ea-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b44ea-116">Not supported.</span></span>|
|<span data-ttu-id="b44ea-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b44ea-117">Application</span></span>|<span data-ttu-id="b44ea-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b44ea-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b44ea-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b44ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b44ea-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b44ea-120">Request headers</span></span>
|<span data-ttu-id="b44ea-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b44ea-121">Header</span></span>|<span data-ttu-id="b44ea-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b44ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b44ea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b44ea-123">Authorization</span></span>|<span data-ttu-id="b44ea-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b44ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b44ea-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b44ea-125">Accept</span></span>|<span data-ttu-id="b44ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b44ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b44ea-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b44ea-127">Request body</span></span>
<span data-ttu-id="b44ea-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b44ea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b44ea-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b44ea-129">Response</span></span>
<span data-ttu-id="b44ea-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [IosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b44ea-130">If successful, this method returns a `200 OK` response code and a collection of [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b44ea-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b44ea-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b44ea-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b44ea-132">Request</span></span>
<span data-ttu-id="b44ea-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b44ea-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="b44ea-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b44ea-134">Response</span></span>
<span data-ttu-id="b44ea-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b44ea-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





