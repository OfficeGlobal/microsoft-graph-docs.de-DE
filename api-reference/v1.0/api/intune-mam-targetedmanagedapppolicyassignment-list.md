---
title: Auflisten von „targetedManagedAppPolicyAssignment“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs targetedManagedAppPolicyAssignment auf.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 829ba67b6e9cf75c9c6cd6d03a367a4e051757a1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867165"
---
# <a name="list-targetedmanagedapppolicyassignments"></a><span data-ttu-id="f3e1b-103">Auflisten von „targetedManagedAppPolicyAssignment“</span><span class="sxs-lookup"><span data-stu-id="f3e1b-103">List targetedManagedAppPolicyAssignments</span></span>

> <span data-ttu-id="f3e1b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f3e1b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3e1b-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) auf.</span><span class="sxs-lookup"><span data-stu-id="f3e1b-105">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f3e1b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f3e1b-106">Prerequisites</span></span>
<span data-ttu-id="f3e1b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3e1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3e1b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f3e1b-109">Permission type</span></span>|<span data-ttu-id="f3e1b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f3e1b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3e1b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f3e1b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f3e1b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f3e1b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f3e1b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f3e1b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3e1b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3e1b-114">Not supported.</span></span>|
|<span data-ttu-id="f3e1b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f3e1b-115">Application</span></span>|<span data-ttu-id="f3e1b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3e1b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3e1b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3e1b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="f3e1b-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f3e1b-118">Request headers</span></span>
|<span data-ttu-id="f3e1b-119">Header</span><span class="sxs-lookup"><span data-stu-id="f3e1b-119">Header</span></span>|<span data-ttu-id="f3e1b-120">Wert</span><span class="sxs-lookup"><span data-stu-id="f3e1b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3e1b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3e1b-121">Authorization</span></span>|<span data-ttu-id="f3e1b-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f3e1b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3e1b-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f3e1b-123">Accept</span></span>|<span data-ttu-id="f3e1b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f3e1b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3e1b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f3e1b-125">Request body</span></span>
<span data-ttu-id="f3e1b-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f3e1b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3e1b-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3e1b-127">Response</span></span>
<span data-ttu-id="f3e1b-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f3e1b-128">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3e1b-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f3e1b-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="f3e1b-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3e1b-130">Request</span></span>
<span data-ttu-id="f3e1b-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f3e1b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
```

### <a name="response"></a><span data-ttu-id="f3e1b-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3e1b-132">Response</span></span>
<span data-ttu-id="f3e1b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f3e1b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 276

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



