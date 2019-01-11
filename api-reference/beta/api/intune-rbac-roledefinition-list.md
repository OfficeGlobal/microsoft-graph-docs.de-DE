---
title: roleDefinitions auflisten
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs roleDefinition auf.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bb6280c1d106ed8b93da3a0b80894200f5afa4fc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851870"
---
# <a name="list-roledefinitions"></a><span data-ttu-id="5f7af-103">roleDefinitions auflisten</span><span class="sxs-lookup"><span data-stu-id="5f7af-103">List roleDefinitions</span></span>

> <span data-ttu-id="5f7af-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5f7af-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f7af-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5f7af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5f7af-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5f7af-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f7af-107">Listet die Eigenschaften und Beziehungen von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md) auf.</span><span class="sxs-lookup"><span data-stu-id="5f7af-107">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5f7af-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5f7af-108">Prerequisites</span></span>
<span data-ttu-id="5f7af-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f7af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f7af-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5f7af-111">Permission type</span></span>|<span data-ttu-id="5f7af-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5f7af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f7af-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5f7af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5f7af-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f7af-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="5f7af-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5f7af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f7af-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f7af-116">Not supported.</span></span>|
|<span data-ttu-id="5f7af-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5f7af-117">Application</span></span>|<span data-ttu-id="5f7af-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f7af-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f7af-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f7af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="5f7af-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5f7af-120">Request headers</span></span>
|<span data-ttu-id="5f7af-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5f7af-121">Header</span></span>|<span data-ttu-id="5f7af-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5f7af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f7af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f7af-123">Authorization</span></span>|<span data-ttu-id="5f7af-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5f7af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f7af-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5f7af-125">Accept</span></span>|<span data-ttu-id="5f7af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5f7af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f7af-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5f7af-127">Request body</span></span>
<span data-ttu-id="5f7af-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5f7af-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f7af-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f7af-129">Response</span></span>
<span data-ttu-id="5f7af-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [roleDefinition](../resources/intune-rbac-roledefinition.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f7af-130">If successful, this method returns a `200 OK` response code and a collection of [roleDefinition](../resources/intune-rbac-roledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f7af-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5f7af-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="5f7af-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f7af-132">Request</span></span>
<span data-ttu-id="5f7af-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5f7af-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="5f7af-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f7af-134">Response</span></span>
<span data-ttu-id="5f7af-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f7af-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1403

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
      "isBuiltIn": true
    }
  ]
}
```





