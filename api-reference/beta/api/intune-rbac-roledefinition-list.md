---
title: roleDefinitions auflisten
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs roleDefinition auf.
ms.openlocfilehash: e9048d232ffbb6a2a3a91a6e5b4085720363eb75
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063988"
---
# <a name="list-roledefinitions"></a><span data-ttu-id="1d01a-103">roleDefinitions auflisten</span><span class="sxs-lookup"><span data-stu-id="1d01a-103">List roleDefinitions</span></span>

> <span data-ttu-id="1d01a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1d01a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d01a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1d01a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d01a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1d01a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d01a-107">Listet die Eigenschaften und Beziehungen von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md) auf.</span><span class="sxs-lookup"><span data-stu-id="1d01a-107">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1d01a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1d01a-108">Prerequisites</span></span>
<span data-ttu-id="1d01a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d01a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d01a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1d01a-111">Permission type</span></span>|<span data-ttu-id="1d01a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1d01a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d01a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1d01a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1d01a-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d01a-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="1d01a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1d01a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d01a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1d01a-116">Not supported.</span></span>|
|<span data-ttu-id="1d01a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1d01a-117">Application</span></span>|<span data-ttu-id="1d01a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1d01a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d01a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1d01a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="1d01a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1d01a-120">Request headers</span></span>
|<span data-ttu-id="1d01a-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1d01a-121">Header</span></span>|<span data-ttu-id="1d01a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1d01a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d01a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d01a-123">Authorization</span></span>|<span data-ttu-id="1d01a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1d01a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d01a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1d01a-125">Accept</span></span>|<span data-ttu-id="1d01a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1d01a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d01a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1d01a-127">Request body</span></span>
<span data-ttu-id="1d01a-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1d01a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d01a-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="1d01a-129">Response</span></span>
<span data-ttu-id="1d01a-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [roleDefinition](../resources/intune-rbac-roledefinition.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1d01a-130">If successful, this method returns a `200 OK` response code and a collection of [roleDefinition](../resources/intune-rbac-roledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d01a-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1d01a-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1d01a-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1d01a-132">Request</span></span>
<span data-ttu-id="1d01a-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1d01a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="1d01a-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="1d01a-134">Response</span></span>
<span data-ttu-id="1d01a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1d01a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





