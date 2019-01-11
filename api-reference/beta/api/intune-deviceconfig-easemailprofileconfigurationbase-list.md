---
title: Liste easEmailProfileConfigurationBases
description: Listeneigenschaften und Beziehungen der EasEmailProfileConfigurationBase-Objekte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3ca0c4a0fc0c6fb12a563c685836a9817337c6de
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869426"
---
# <a name="list-easemailprofileconfigurationbases"></a><span data-ttu-id="4c3dd-103">Liste easEmailProfileConfigurationBases</span><span class="sxs-lookup"><span data-stu-id="4c3dd-103">List easEmailProfileConfigurationBases</span></span>

> <span data-ttu-id="4c3dd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4c3dd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c3dd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4c3dd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c3dd-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4c3dd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c3dd-107">Listeneigenschaften und Beziehungen der [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="4c3dd-107">List properties and relationships of the [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4c3dd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4c3dd-108">Prerequisites</span></span>
<span data-ttu-id="4c3dd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c3dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c3dd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4c3dd-111">Permission type</span></span>|<span data-ttu-id="4c3dd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4c3dd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c3dd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4c3dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4c3dd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c3dd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4c3dd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4c3dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c3dd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4c3dd-116">Not supported.</span></span>|
|<span data-ttu-id="4c3dd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4c3dd-117">Application</span></span>|<span data-ttu-id="4c3dd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4c3dd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c3dd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4c3dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4c3dd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4c3dd-120">Request headers</span></span>
|<span data-ttu-id="4c3dd-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4c3dd-121">Header</span></span>|<span data-ttu-id="4c3dd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4c3dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c3dd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c3dd-123">Authorization</span></span>|<span data-ttu-id="4c3dd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4c3dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c3dd-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4c3dd-125">Accept</span></span>|<span data-ttu-id="4c3dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4c3dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c3dd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4c3dd-127">Request body</span></span>
<span data-ttu-id="4c3dd-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4c3dd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c3dd-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="4c3dd-129">Response</span></span>
<span data-ttu-id="4c3dd-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [EasEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md) .</span><span class="sxs-lookup"><span data-stu-id="4c3dd-130">If successful, this method returns a `200 OK` response code and a collection of [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c3dd-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4c3dd-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4c3dd-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4c3dd-132">Request</span></span>
<span data-ttu-id="4c3dd-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4c3dd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="4c3dd-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="4c3dd-134">Response</span></span>
<span data-ttu-id="4c3dd-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4c3dd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 715

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.easEmailProfileConfigurationBase",
      "id": "a3f96310-6310-a3f9-1063-f9a31063f9a3",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "usernameSource": "primarySmtpAddress",
      "usernameAADSource": "primarySmtpAddress",
      "userDomainNameSource": "netBiosDomainName",
      "customDomainName": "Custom Domain Name value"
    }
  ]
}
```





