---
title: Abrufen von „macOSGeneralDeviceConfiguration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs macOSGeneralDeviceConfiguration.
ms.openlocfilehash: 683ccbe38bc2380763bc0673383b0e47403f019a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016294"
---
# <a name="get-macosgeneraldeviceconfiguration"></a><span data-ttu-id="e57e3-103">Abrufen von „macOSGeneralDeviceConfiguration“</span><span class="sxs-lookup"><span data-stu-id="e57e3-103">Get macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="e57e3-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e57e3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e57e3-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e57e3-105">Read properties and relationships of the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e57e3-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e57e3-106">Prerequisites</span></span>
<span data-ttu-id="e57e3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e57e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e57e3-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e57e3-109">Permission type</span></span>|<span data-ttu-id="e57e3-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e57e3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e57e3-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e57e3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e57e3-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e57e3-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e57e3-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e57e3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e57e3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e57e3-114">Not supported.</span></span>|
|<span data-ttu-id="e57e3-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e57e3-115">Application</span></span>|<span data-ttu-id="e57e3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e57e3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e57e3-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e57e3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e57e3-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e57e3-118">Optional query parameters</span></span>
<span data-ttu-id="e57e3-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e57e3-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e57e3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e57e3-120">Request headers</span></span>
|<span data-ttu-id="e57e3-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e57e3-121">Header</span></span>|<span data-ttu-id="e57e3-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e57e3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e57e3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e57e3-123">Authorization</span></span>|<span data-ttu-id="e57e3-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e57e3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e57e3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e57e3-125">Accept</span></span>|<span data-ttu-id="e57e3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e57e3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e57e3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e57e3-127">Request body</span></span>
<span data-ttu-id="e57e3-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e57e3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e57e3-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e57e3-129">Response</span></span>
<span data-ttu-id="e57e3-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e57e3-130">If successful, this method returns a `200 OK` response code and [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e57e3-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e57e3-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e57e3-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e57e3-132">Request</span></span>
<span data-ttu-id="e57e3-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e57e3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e57e3-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e57e3-134">Response</span></span>
<span data-ttu-id="e57e3-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e57e3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1155

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
    "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "compliantAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "compliantAppListType": "appsInListCompliant",
    "emailInDomainSuffixes": [
      "Email In Domain Suffixes value"
    ],
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumCharacterSetCount": 0,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordRequiredType": "alphanumeric",
    "passwordRequired": true
  }
}
```


