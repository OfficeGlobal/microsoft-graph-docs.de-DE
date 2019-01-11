---
title: Auflisten von „windowsInformationProtectionAppLockerFile“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windowsInformationProtectionAppLockerFile auf.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: af1c2d9346abc12ab8909aceb199eab60d87432a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822925"
---
# <a name="list-windowsinformationprotectionapplockerfiles"></a><span data-ttu-id="c9299-103">Auflisten von „windowsInformationProtectionAppLockerFile“</span><span class="sxs-lookup"><span data-stu-id="c9299-103">List windowsInformationProtectionAppLockerFiles</span></span>

> <span data-ttu-id="c9299-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c9299-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9299-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c9299-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9299-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c9299-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9299-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) auf.</span><span class="sxs-lookup"><span data-stu-id="c9299-107">List properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c9299-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c9299-108">Prerequisites</span></span>
<span data-ttu-id="c9299-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9299-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9299-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c9299-111">Permission type</span></span>|<span data-ttu-id="c9299-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c9299-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9299-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c9299-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9299-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9299-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c9299-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c9299-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9299-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c9299-116">Not supported.</span></span>|
|<span data-ttu-id="c9299-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c9299-117">Application</span></span>|<span data-ttu-id="c9299-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c9299-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9299-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9299-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles
```

## <a name="request-headers"></a><span data-ttu-id="c9299-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c9299-120">Request headers</span></span>
|<span data-ttu-id="c9299-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c9299-121">Header</span></span>|<span data-ttu-id="c9299-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c9299-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9299-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9299-123">Authorization</span></span>|<span data-ttu-id="c9299-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c9299-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9299-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c9299-125">Accept</span></span>|<span data-ttu-id="c9299-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9299-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9299-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c9299-127">Request body</span></span>
<span data-ttu-id="c9299-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c9299-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9299-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9299-129">Response</span></span>
<span data-ttu-id="c9299-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c9299-130">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9299-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c9299-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c9299-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9299-132">Request</span></span>
<span data-ttu-id="c9299-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c9299-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
```

### <a name="response"></a><span data-ttu-id="c9299-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9299-134">Response</span></span>
<span data-ttu-id="c9299-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c9299-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
      "displayName": "Display Name value",
      "fileHash": "File Hash value",
      "file": "ZmlsZQ==",
      "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
      "version": "Version value"
    }
  ]
}
```





