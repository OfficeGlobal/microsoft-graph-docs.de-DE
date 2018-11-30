---
title: deviceAndAppManagementRoleDefinition abrufen
description: Lesen von Eigenschaften und Beziehungen des deviceAndAppManagementRoleDefinition-Objekts.
ms.openlocfilehash: bac40bf39fa4e4a5bdf303d54e9f4da006c09b1b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018034"
---
# <a name="get-deviceandappmanagementroledefinition"></a><span data-ttu-id="44021-103">deviceAndAppManagementRoleDefinition abrufen</span><span class="sxs-lookup"><span data-stu-id="44021-103">Get deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="44021-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="44021-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44021-105">Lesen von Eigenschaften und Beziehungen des [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="44021-105">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="44021-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="44021-106">Prerequisites</span></span>
<span data-ttu-id="44021-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44021-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44021-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="44021-109">Permission type</span></span>|<span data-ttu-id="44021-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="44021-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44021-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="44021-111">Delegated (work or school account)</span></span>|<span data-ttu-id="44021-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="44021-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="44021-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="44021-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44021-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="44021-114">Not supported.</span></span>|
|<span data-ttu-id="44021-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="44021-115">Application</span></span>|<span data-ttu-id="44021-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="44021-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44021-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="44021-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="optional-query-parameters"></a><span data-ttu-id="44021-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="44021-118">Optional query parameters</span></span>
<span data-ttu-id="44021-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="44021-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="44021-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="44021-120">Request headers</span></span>
|<span data-ttu-id="44021-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="44021-121">Header</span></span>|<span data-ttu-id="44021-122">Wert</span><span class="sxs-lookup"><span data-stu-id="44021-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44021-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="44021-123">Authorization</span></span>|<span data-ttu-id="44021-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="44021-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44021-125">Accept</span><span class="sxs-lookup"><span data-stu-id="44021-125">Accept</span></span>|<span data-ttu-id="44021-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44021-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44021-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="44021-127">Request body</span></span>
<span data-ttu-id="44021-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="44021-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44021-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="44021-129">Response</span></span>
<span data-ttu-id="44021-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="44021-130">If successful, this method returns a `200 OK` response code and [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44021-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="44021-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="44021-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="44021-132">Request</span></span>
<span data-ttu-id="44021-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="44021-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="44021-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="44021-134">Response</span></span>
<span data-ttu-id="44021-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="44021-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 712

{
  "value": {
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
}
```



