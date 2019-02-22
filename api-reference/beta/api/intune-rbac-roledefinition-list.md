---
title: roleDefinitions auflisten
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs roleDefinition auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 105680c19d514764ab2adc609eeb356d240b8312
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156546"
---
# <a name="list-roledefinitions"></a><span data-ttu-id="47b92-103">roleDefinitions auflisten</span><span class="sxs-lookup"><span data-stu-id="47b92-103">List roleDefinitions</span></span>

> <span data-ttu-id="47b92-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="47b92-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47b92-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="47b92-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47b92-106">Listet die Eigenschaften und Beziehungen von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md) auf.</span><span class="sxs-lookup"><span data-stu-id="47b92-106">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47b92-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="47b92-107">Prerequisites</span></span>
<span data-ttu-id="47b92-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="47b92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="47b92-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="47b92-110">Permission type</span></span>|<span data-ttu-id="47b92-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="47b92-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47b92-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="47b92-112">Delegated (work or school account)</span></span>|<span data-ttu-id="47b92-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="47b92-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="47b92-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="47b92-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47b92-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="47b92-115">Not supported.</span></span>|
|<span data-ttu-id="47b92-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="47b92-116">Application</span></span>|<span data-ttu-id="47b92-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="47b92-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47b92-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="47b92-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="47b92-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="47b92-119">Request headers</span></span>
|<span data-ttu-id="47b92-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="47b92-120">Header</span></span>|<span data-ttu-id="47b92-121">Wert</span><span class="sxs-lookup"><span data-stu-id="47b92-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47b92-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="47b92-122">Authorization</span></span>|<span data-ttu-id="47b92-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="47b92-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47b92-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="47b92-124">Accept</span></span>|<span data-ttu-id="47b92-125">application/json</span><span class="sxs-lookup"><span data-stu-id="47b92-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47b92-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="47b92-126">Request body</span></span>
<span data-ttu-id="47b92-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="47b92-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47b92-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="47b92-128">Response</span></span>
<span data-ttu-id="47b92-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [roleDefinition](../resources/intune-rbac-roledefinition.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="47b92-129">If successful, this method returns a `200 OK` response code and a collection of [roleDefinition](../resources/intune-rbac-roledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47b92-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="47b92-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="47b92-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="47b92-131">Request</span></span>
<span data-ttu-id="47b92-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="47b92-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="47b92-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="47b92-133">Response</span></span>
<span data-ttu-id="47b92-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="47b92-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1477

{
  "value": [
    {
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
  ]
}
```




