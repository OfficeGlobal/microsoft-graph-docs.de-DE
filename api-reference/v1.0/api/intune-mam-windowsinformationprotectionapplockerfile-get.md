---
title: Abrufen von „windowsInformationProtectionAppLockerFile“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs windowsInformationProtectionAppLockerFile.
author: tfitzmac
ms.openlocfilehash: c4c23d4aacfdba6bc6dd2482c583bc160462f646
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323548"
---
# <a name="get-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="e8e24-103">Abrufen von „windowsInformationProtectionAppLockerFile“</span><span class="sxs-lookup"><span data-stu-id="e8e24-103">Get windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="e8e24-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e8e24-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8e24-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="e8e24-105">Read properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e8e24-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e8e24-106">Prerequisites</span></span>
<span data-ttu-id="e8e24-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8e24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8e24-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e8e24-109">Permission type</span></span>|<span data-ttu-id="e8e24-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e8e24-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8e24-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e8e24-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e8e24-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8e24-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e8e24-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e8e24-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8e24-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e8e24-114">Not supported.</span></span>|
|<span data-ttu-id="e8e24-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e8e24-115">Application</span></span>|<span data-ttu-id="e8e24-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e8e24-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8e24-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e8e24-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8e24-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e8e24-118">Optional query parameters</span></span>
<span data-ttu-id="e8e24-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e8e24-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e8e24-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e8e24-120">Request headers</span></span>
|<span data-ttu-id="e8e24-121">Header</span><span class="sxs-lookup"><span data-stu-id="e8e24-121">Header</span></span>|<span data-ttu-id="e8e24-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e8e24-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8e24-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e8e24-123">Authorization</span></span>|<span data-ttu-id="e8e24-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e8e24-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8e24-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e8e24-125">Accept</span></span>|<span data-ttu-id="e8e24-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e8e24-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8e24-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e8e24-127">Request body</span></span>
<span data-ttu-id="e8e24-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e8e24-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8e24-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e8e24-129">Response</span></span>
<span data-ttu-id="e8e24-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e8e24-130">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8e24-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e8e24-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e8e24-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e8e24-132">Request</span></span>
<span data-ttu-id="e8e24-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e8e24-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

### <a name="response"></a><span data-ttu-id="e8e24-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e8e24-134">Response</span></span>
<span data-ttu-id="e8e24-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e8e24-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
    "displayName": "Display Name value",
    "fileHash": "File Hash value",
    "file": "ZmlsZQ==",
    "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
    "version": "Version value"
  }
}
```



