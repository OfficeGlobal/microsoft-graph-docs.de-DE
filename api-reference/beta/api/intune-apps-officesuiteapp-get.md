---
title: Abrufen von officeSuiteApp
description: Lesen Sie Eigenschaften und Beziehungen des OfficeSuiteApp-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 10bc2933d498e9397a5c9d71b97db6e32d58efe2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424490"
---
# <a name="get-officesuiteapp"></a><span data-ttu-id="4e0dd-103">Abrufen von officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="4e0dd-103">Get officeSuiteApp</span></span>

> <span data-ttu-id="4e0dd-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="4e0dd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4e0dd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4e0dd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e0dd-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4e0dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e0dd-107">Lesen Sie Eigenschaften und Beziehungen des [OfficeSuiteApp](../resources/intune-apps-officesuiteapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4e0dd-107">Read properties and relationships of the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e0dd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4e0dd-108">Prerequisites</span></span>
<span data-ttu-id="4e0dd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4e0dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4e0dd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4e0dd-111">Permission type</span></span>|<span data-ttu-id="4e0dd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4e0dd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e0dd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4e0dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e0dd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e0dd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4e0dd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4e0dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e0dd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4e0dd-116">Not supported.</span></span>|
|<span data-ttu-id="4e0dd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4e0dd-117">Application</span></span>|<span data-ttu-id="4e0dd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4e0dd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e0dd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e0dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4e0dd-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4e0dd-120">Optional query parameters</span></span>
<span data-ttu-id="4e0dd-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4e0dd-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4e0dd-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4e0dd-122">Request headers</span></span>
|<span data-ttu-id="4e0dd-123">Header</span><span class="sxs-lookup"><span data-stu-id="4e0dd-123">Header</span></span>|<span data-ttu-id="4e0dd-124">Wert</span><span class="sxs-lookup"><span data-stu-id="4e0dd-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e0dd-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4e0dd-125">Authorization</span></span>|<span data-ttu-id="4e0dd-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4e0dd-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e0dd-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4e0dd-127">Accept</span></span>|<span data-ttu-id="4e0dd-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4e0dd-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e0dd-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4e0dd-129">Request body</span></span>
<span data-ttu-id="4e0dd-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4e0dd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e0dd-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e0dd-131">Response</span></span>
<span data-ttu-id="4e0dd-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [OfficeSuiteApp](../resources/intune-apps-officesuiteapp.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4e0dd-132">If successful, this method returns a `200 OK` response code and [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e0dd-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4e0dd-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e0dd-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e0dd-134">Request</span></span>
<span data-ttu-id="4e0dd-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4e0dd-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="4e0dd-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e0dd-136">Response</span></span>
<span data-ttu-id="4e0dd-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4e0dd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1853

{
  "value": {
    "@odata.type": "#microsoft.graph.officeSuiteApp",
    "id": "9b263b46-3b46-9b26-463b-269b463b269b",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "largeIcon": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "isFeatured": true,
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
    "informationUrl": "https://example.com/informationUrl/",
    "owner": "Owner value",
    "developer": "Developer value",
    "notes": "Notes value",
    "uploadState": 11,
    "publishingState": "processing",
    "isAssigned": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "autoAcceptEula": true,
    "productIds": [
      "o365BusinessRetail"
    ],
    "excludedApps": {
      "@odata.type": "microsoft.graph.excludedApps",
      "access": true,
      "excel": true,
      "groove": true,
      "infoPath": true,
      "lync": true,
      "oneDrive": true,
      "oneNote": true,
      "outlook": true,
      "powerPoint": true,
      "publisher": true,
      "sharePointDesigner": true,
      "visio": true,
      "word": true
    },
    "useSharedComputerActivation": true,
    "updateChannel": "current",
    "officePlatformArchitecture": "x86",
    "localesToInstall": [
      "Locales To Install value"
    ],
    "installProgressDisplayLevel": "full",
    "shouldUninstallOlderVersionsOfOffice": true,
    "targetVersion": "Target Version value",
    "updateVersion": "Update Version value",
    "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
  }
}
```




