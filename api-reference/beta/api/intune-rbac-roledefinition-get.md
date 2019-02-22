---
title: roleDefinition abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs roleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e63146c79bbf2fb383f4f5a1026f115fe034ad94
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170119"
---
# <a name="get-roledefinition"></a><span data-ttu-id="813b7-103">roleDefinition abrufen</span><span class="sxs-lookup"><span data-stu-id="813b7-103">Get roleDefinition</span></span>

> <span data-ttu-id="813b7-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="813b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="813b7-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="813b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="813b7-106">Liest die Eigenschaften und Beziehungen von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="813b7-106">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="813b7-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="813b7-107">Prerequisites</span></span>
<span data-ttu-id="813b7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="813b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="813b7-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="813b7-110">Permission type</span></span>|<span data-ttu-id="813b7-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="813b7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="813b7-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="813b7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="813b7-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="813b7-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="813b7-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="813b7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="813b7-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="813b7-115">Not supported.</span></span>|
|<span data-ttu-id="813b7-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="813b7-116">Application</span></span>|<span data-ttu-id="813b7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="813b7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="813b7-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="813b7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="optional-query-parameters"></a><span data-ttu-id="813b7-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="813b7-119">Optional query parameters</span></span>
<span data-ttu-id="813b7-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="813b7-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="813b7-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="813b7-121">Request headers</span></span>
|<span data-ttu-id="813b7-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="813b7-122">Header</span></span>|<span data-ttu-id="813b7-123">Wert</span><span class="sxs-lookup"><span data-stu-id="813b7-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="813b7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="813b7-124">Authorization</span></span>|<span data-ttu-id="813b7-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="813b7-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="813b7-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="813b7-126">Accept</span></span>|<span data-ttu-id="813b7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="813b7-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="813b7-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="813b7-128">Request body</span></span>
<span data-ttu-id="813b7-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="813b7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="813b7-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="813b7-130">Response</span></span>
<span data-ttu-id="813b7-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [roleDefinition](../resources/intune-rbac-roledefinition.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="813b7-131">If successful, this method returns a `200 OK` response code and [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="813b7-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="813b7-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="813b7-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="813b7-133">Request</span></span>
<span data-ttu-id="813b7-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="813b7-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="813b7-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="813b7-135">Response</span></span>
<span data-ttu-id="813b7-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="813b7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1369

{
  "value": {
    "@odata.type": "#microsoft.graph.roleDefinition",
    "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
    "displayName": "Display Name value",
    "description": "Description value",
    "permissions": [
      {
        "@odata.type": "microsoft.graph.rolePermission",
        "actions": [
          "Actions value"
        ],
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
    "rolePermissions": [
      {
        "@odata.type": "microsoft.graph.rolePermission",
        "actions": [
          "Actions value"
        ],
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
    "isBuiltInRoleDefinition": true,
    "isBuiltIn": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```




