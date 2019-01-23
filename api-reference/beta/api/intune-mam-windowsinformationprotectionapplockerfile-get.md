---
title: Abrufen von „windowsInformationProtectionAppLockerFile“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs windowsInformationProtectionAppLockerFile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bf563c5e4afbec829803c3fc78029990e0a08f50
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414991"
---
# <a name="get-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="04696-103">Abrufen von „windowsInformationProtectionAppLockerFile“</span><span class="sxs-lookup"><span data-stu-id="04696-103">Get windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="04696-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="04696-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="04696-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="04696-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04696-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="04696-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04696-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="04696-107">Read properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04696-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="04696-108">Prerequisites</span></span>
<span data-ttu-id="04696-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="04696-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="04696-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="04696-111">Permission type</span></span>|<span data-ttu-id="04696-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="04696-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04696-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="04696-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04696-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="04696-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="04696-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="04696-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04696-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="04696-116">Not supported.</span></span>|
|<span data-ttu-id="04696-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="04696-117">Application</span></span>|<span data-ttu-id="04696-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="04696-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04696-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="04696-119">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="04696-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="04696-120">Optional query parameters</span></span>
<span data-ttu-id="04696-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="04696-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="04696-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="04696-122">Request headers</span></span>
|<span data-ttu-id="04696-123">Header</span><span class="sxs-lookup"><span data-stu-id="04696-123">Header</span></span>|<span data-ttu-id="04696-124">Wert</span><span class="sxs-lookup"><span data-stu-id="04696-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04696-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="04696-125">Authorization</span></span>|<span data-ttu-id="04696-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="04696-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04696-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="04696-127">Accept</span></span>|<span data-ttu-id="04696-128">application/json</span><span class="sxs-lookup"><span data-stu-id="04696-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04696-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="04696-129">Request body</span></span>
<span data-ttu-id="04696-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="04696-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04696-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="04696-131">Response</span></span>
<span data-ttu-id="04696-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="04696-132">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04696-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="04696-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="04696-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04696-134">Request</span></span>
<span data-ttu-id="04696-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="04696-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

### <a name="response"></a><span data-ttu-id="04696-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="04696-136">Response</span></span>
<span data-ttu-id="04696-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04696-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




