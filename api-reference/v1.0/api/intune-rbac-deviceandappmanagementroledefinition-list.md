---
title: deviceAndAppManagementRoleDefinitions auflisten
description: Auflisten von Eigenschaften und Beziehungen der deviceAndAppManagementRoleDefinition-Objekte.
ms.openlocfilehash: 5cefb4694c3faf481ac6122356e879ec103469a1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017765"
---
# <a name="list-deviceandappmanagementroledefinitions"></a><span data-ttu-id="5fb0a-103">deviceAndAppManagementRoleDefinitions auflisten</span><span class="sxs-lookup"><span data-stu-id="5fb0a-103">List deviceAndAppManagementRoleDefinitions</span></span>

> <span data-ttu-id="5fb0a-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5fb0a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5fb0a-105">Auflisten von Eigenschaften und Beziehungen der [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="5fb0a-105">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5fb0a-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5fb0a-106">Prerequisites</span></span>
<span data-ttu-id="5fb0a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fb0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fb0a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5fb0a-109">Permission type</span></span>|<span data-ttu-id="5fb0a-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5fb0a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5fb0a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5fb0a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5fb0a-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="5fb0a-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="5fb0a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5fb0a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fb0a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5fb0a-114">Not supported.</span></span>|
|<span data-ttu-id="5fb0a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5fb0a-115">Application</span></span>|<span data-ttu-id="5fb0a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5fb0a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5fb0a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5fb0a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="5fb0a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5fb0a-118">Request headers</span></span>
|<span data-ttu-id="5fb0a-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5fb0a-119">Header</span></span>|<span data-ttu-id="5fb0a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="5fb0a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5fb0a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5fb0a-121">Authorization</span></span>|<span data-ttu-id="5fb0a-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5fb0a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5fb0a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5fb0a-123">Accept</span></span>|<span data-ttu-id="5fb0a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5fb0a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fb0a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5fb0a-125">Request body</span></span>
<span data-ttu-id="5fb0a-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5fb0a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5fb0a-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="5fb0a-127">Response</span></span>
<span data-ttu-id="5fb0a-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Collection von [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5fb0a-128">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fb0a-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5fb0a-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="5fb0a-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5fb0a-130">Request</span></span>
<span data-ttu-id="5fb0a-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5fb0a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="5fb0a-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="5fb0a-132">Response</span></span>
<span data-ttu-id="5fb0a-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5fb0a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 768

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
      "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
      "displayName": "Display Name value",
      "description": "Description value",
      "rolePermissions": [
        {
          "@odata.type": "microsoft.graph.rolePermission",
          "resourceActions": [
            {
              "@odata.type": "microsoft.graph.resourceAction",
              "allowedResourceActions": [
                "Allowed Resource Actions value"
              ],
              "notAllowedResourceActions": [
                "Not Allowed Resource Actions value"
              ]
            }
          ]
        }
      ],
      "isBuiltIn": true
    }
  ]
}
```



