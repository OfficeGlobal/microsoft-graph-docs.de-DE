---
title: Auflisten von „appleDeviceFeaturesConfigurationBase“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs appleDeviceFeaturesConfigurationBase auf.
ms.openlocfilehash: c3391b8fa416f01b50f11c1dd387bb3da2060e31
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060214"
---
# <a name="list-appledevicefeaturesconfigurationbases"></a><span data-ttu-id="ed281-103">Auflisten von „appleDeviceFeaturesConfigurationBase“</span><span class="sxs-lookup"><span data-stu-id="ed281-103">List appleDeviceFeaturesConfigurationBases</span></span>

> <span data-ttu-id="ed281-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ed281-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed281-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ed281-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed281-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ed281-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed281-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) auf.</span><span class="sxs-lookup"><span data-stu-id="ed281-107">List properties and relationships of the [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ed281-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ed281-108">Prerequisites</span></span>
<span data-ttu-id="ed281-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed281-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed281-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ed281-111">Permission type</span></span>|<span data-ttu-id="ed281-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ed281-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed281-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ed281-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ed281-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed281-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ed281-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ed281-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed281-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed281-116">Not supported.</span></span>|
|<span data-ttu-id="ed281-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ed281-117">Application</span></span>|<span data-ttu-id="ed281-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed281-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed281-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed281-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ed281-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ed281-120">Request headers</span></span>
|<span data-ttu-id="ed281-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ed281-121">Header</span></span>|<span data-ttu-id="ed281-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ed281-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed281-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed281-123">Authorization</span></span>|<span data-ttu-id="ed281-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ed281-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed281-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ed281-125">Accept</span></span>|<span data-ttu-id="ed281-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed281-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed281-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ed281-127">Request body</span></span>
<span data-ttu-id="ed281-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ed281-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed281-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed281-129">Response</span></span>
<span data-ttu-id="ed281-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ed281-130">If successful, this method returns a `200 OK` response code and a collection of [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed281-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ed281-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ed281-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed281-132">Request</span></span>
<span data-ttu-id="ed281-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ed281-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="ed281-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed281-134">Response</span></span>
<span data-ttu-id="ed281-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ed281-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 789

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.appleDeviceFeaturesConfigurationBase",
      "id": "ca0bb5ff-b5ff-ca0b-ffb5-0bcaffb50bca",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "airPrintDestinations": [
        {
          "@odata.type": "microsoft.graph.airPrintDestination",
          "ipAddress": "Ip Address value",
          "resourcePath": "Resource Path value",
          "port": 4,
          "forceTls": true
        }
      ]
    }
  ]
}
```





