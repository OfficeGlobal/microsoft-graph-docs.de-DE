---
title: deviceAndAppManagementRoleDefinitions auflisten
description: Auflisten von Eigenschaften und Beziehungen der deviceAndAppManagementRoleDefinition-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0420fe32ca99b7ff8ed8785b49e36a505a122ae9
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969617"
---
# <a name="list-deviceandappmanagementroledefinitions"></a><span data-ttu-id="f3a08-103">deviceAndAppManagementRoleDefinitions auflisten</span><span class="sxs-lookup"><span data-stu-id="f3a08-103">List deviceAndAppManagementRoleDefinitions</span></span>

> <span data-ttu-id="f3a08-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3a08-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3a08-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f3a08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3a08-106">Auflisten von Eigenschaften und Beziehungen der [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="f3a08-106">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3a08-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f3a08-107">Prerequisites</span></span>
<span data-ttu-id="f3a08-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3a08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3a08-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f3a08-110">Permission type</span></span>|<span data-ttu-id="f3a08-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f3a08-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3a08-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f3a08-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3a08-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="f3a08-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="f3a08-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f3a08-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3a08-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3a08-115">Not supported.</span></span>|
|<span data-ttu-id="f3a08-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f3a08-116">Application</span></span>|<span data-ttu-id="f3a08-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f3a08-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3a08-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3a08-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="f3a08-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f3a08-119">Request headers</span></span>
|<span data-ttu-id="f3a08-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f3a08-120">Header</span></span>|<span data-ttu-id="f3a08-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f3a08-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3a08-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3a08-122">Authorization</span></span>|<span data-ttu-id="f3a08-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f3a08-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3a08-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f3a08-124">Accept</span></span>|<span data-ttu-id="f3a08-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f3a08-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3a08-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f3a08-126">Request body</span></span>
<span data-ttu-id="f3a08-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f3a08-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3a08-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3a08-128">Response</span></span>
<span data-ttu-id="f3a08-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Collection von [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f3a08-129">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3a08-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f3a08-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3a08-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f3a08-131">Request</span></span>
<span data-ttu-id="f3a08-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f3a08-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="f3a08-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f3a08-133">Response</span></span>
<span data-ttu-id="f3a08-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f3a08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1499

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
      "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
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
  ]
}
```




