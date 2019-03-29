---
title: OfficeSuiteApp abrufen
description: Lesen von Eigenschaften und Beziehungen des officeSuiteApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa744933f90af9c0dd174a5fc22bc1993b9105c5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958865"
---
# <a name="get-officesuiteapp"></a><span data-ttu-id="526f7-103">OfficeSuiteApp abrufen</span><span class="sxs-lookup"><span data-stu-id="526f7-103">Get officeSuiteApp</span></span>

> <span data-ttu-id="526f7-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="526f7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="526f7-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="526f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="526f7-106">Lesen von Eigenschaften und Beziehungen des [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="526f7-106">Read properties and relationships of the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="526f7-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="526f7-107">Prerequisites</span></span>
<span data-ttu-id="526f7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="526f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="526f7-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="526f7-110">Permission type</span></span>|<span data-ttu-id="526f7-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="526f7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="526f7-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="526f7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="526f7-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="526f7-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="526f7-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="526f7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="526f7-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="526f7-115">Not supported.</span></span>|
|<span data-ttu-id="526f7-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="526f7-116">Application</span></span>|<span data-ttu-id="526f7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="526f7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="526f7-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="526f7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="526f7-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="526f7-119">Optional query parameters</span></span>
<span data-ttu-id="526f7-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="526f7-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="526f7-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="526f7-121">Request headers</span></span>
|<span data-ttu-id="526f7-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="526f7-122">Header</span></span>|<span data-ttu-id="526f7-123">Wert</span><span class="sxs-lookup"><span data-stu-id="526f7-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="526f7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="526f7-124">Authorization</span></span>|<span data-ttu-id="526f7-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="526f7-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="526f7-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="526f7-126">Accept</span></span>|<span data-ttu-id="526f7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="526f7-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="526f7-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="526f7-128">Request body</span></span>
<span data-ttu-id="526f7-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="526f7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="526f7-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="526f7-130">Response</span></span>
<span data-ttu-id="526f7-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="526f7-131">If successful, this method returns a `200 OK` response code and [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="526f7-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="526f7-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="526f7-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="526f7-133">Request</span></span>
<span data-ttu-id="526f7-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="526f7-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="526f7-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="526f7-135">Response</span></span>
<span data-ttu-id="526f7-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="526f7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1875

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
      "teams": true,
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




