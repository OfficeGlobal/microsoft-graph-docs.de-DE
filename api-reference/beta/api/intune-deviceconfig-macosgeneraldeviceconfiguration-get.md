---
title: Abrufen von „macOSGeneralDeviceConfiguration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs macOSGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c1badb9178e90c08e82fc9314d40ce78424f9d5e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938580"
---
# <a name="get-macosgeneraldeviceconfiguration"></a><span data-ttu-id="47ec3-103">Abrufen von „macOSGeneralDeviceConfiguration“</span><span class="sxs-lookup"><span data-stu-id="47ec3-103">Get macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="47ec3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="47ec3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47ec3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="47ec3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="47ec3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="47ec3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47ec3-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47ec3-107">Read properties and relationships of the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="47ec3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="47ec3-108">Prerequisites</span></span>
<span data-ttu-id="47ec3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47ec3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47ec3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="47ec3-111">Permission type</span></span>|<span data-ttu-id="47ec3-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="47ec3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47ec3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="47ec3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47ec3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="47ec3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="47ec3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="47ec3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47ec3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="47ec3-116">Not supported.</span></span>|
|<span data-ttu-id="47ec3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="47ec3-117">Application</span></span>|<span data-ttu-id="47ec3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="47ec3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47ec3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="47ec3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47ec3-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="47ec3-120">Optional query parameters</span></span>
<span data-ttu-id="47ec3-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="47ec3-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="47ec3-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="47ec3-122">Request headers</span></span>
|<span data-ttu-id="47ec3-123">Header</span><span class="sxs-lookup"><span data-stu-id="47ec3-123">Header</span></span>|<span data-ttu-id="47ec3-124">Wert</span><span class="sxs-lookup"><span data-stu-id="47ec3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47ec3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="47ec3-125">Authorization</span></span>|<span data-ttu-id="47ec3-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="47ec3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47ec3-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="47ec3-127">Accept</span></span>|<span data-ttu-id="47ec3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="47ec3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47ec3-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="47ec3-129">Request body</span></span>
<span data-ttu-id="47ec3-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="47ec3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47ec3-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="47ec3-131">Response</span></span>
<span data-ttu-id="47ec3-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="47ec3-132">If successful, this method returns a `200 OK` response code and [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47ec3-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="47ec3-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="47ec3-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="47ec3-134">Request</span></span>
<span data-ttu-id="47ec3-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="47ec3-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="47ec3-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="47ec3-136">Response</span></span>
<span data-ttu-id="47ec3-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="47ec3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2054

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
    "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
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
    "passwordRequired": true,
    "keychainBlockCloudSync": true,
    "airPrintBlocked": true,
    "airPrintForceTrustedTLS": true,
    "airPrintBlockiBeaconDiscovery": true,
    "safariBlockAutofill": true,
    "cameraBlocked": true,
    "iTunesBlockMusicService": true,
    "spotlightBlockInternetResults": true,
    "keyboardBlockDictation": true,
    "definitionLookupBlocked": true,
    "appleWatchBlockAutoUnlock": true,
    "iTunesBlockFileSharing": true,
    "iCloudBlockDocumentSync": true,
    "iCloudBlockMail": true,
    "iCloudBlockAddressBook": true,
    "iCloudBlockCalendar": true,
    "iCloudBlockReminders": true,
    "iCloudBlockBookmarks": true,
    "iCloudBlockNotes": true,
    "airDropBlocked": true,
    "passwordBlockModification": true,
    "passwordBlockFingerprintUnlock": true
  }
}
```





