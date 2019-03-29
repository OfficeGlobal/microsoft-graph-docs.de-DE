---
title: deviceAndAppManagementRoleDefinitions auflisten
description: Auflisten von Eigenschaften und Beziehungen der deviceAndAppManagementRoleDefinition-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6530309293c0b678416806782fa699487300ca00
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983498"
---
# <a name="list-deviceandappmanagementroledefinitions"></a><span data-ttu-id="7b1f7-103">deviceAndAppManagementRoleDefinitions auflisten</span><span class="sxs-lookup"><span data-stu-id="7b1f7-103">List deviceAndAppManagementRoleDefinitions</span></span>

> <span data-ttu-id="7b1f7-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7b1f7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b1f7-105">Auflisten von Eigenschaften und Beziehungen der [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="7b1f7-105">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b1f7-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7b1f7-106">Prerequisites</span></span>
<span data-ttu-id="7b1f7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b1f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b1f7-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7b1f7-109">Permission type</span></span>|<span data-ttu-id="7b1f7-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7b1f7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b1f7-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7b1f7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7b1f7-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b1f7-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="7b1f7-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7b1f7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b1f7-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b1f7-114">Not supported.</span></span>|
|<span data-ttu-id="7b1f7-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7b1f7-115">Application</span></span>|<span data-ttu-id="7b1f7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b1f7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b1f7-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b1f7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="7b1f7-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7b1f7-118">Request headers</span></span>
|<span data-ttu-id="7b1f7-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7b1f7-119">Header</span></span>|<span data-ttu-id="7b1f7-120">Wert</span><span class="sxs-lookup"><span data-stu-id="7b1f7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b1f7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b1f7-121">Authorization</span></span>|<span data-ttu-id="7b1f7-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7b1f7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b1f7-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7b1f7-123">Accept</span></span>|<span data-ttu-id="7b1f7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7b1f7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b1f7-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7b1f7-125">Request body</span></span>
<span data-ttu-id="7b1f7-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7b1f7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b1f7-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b1f7-127">Response</span></span>
<span data-ttu-id="7b1f7-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Collection von [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7b1f7-128">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b1f7-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7b1f7-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b1f7-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b1f7-130">Request</span></span>
<span data-ttu-id="7b1f7-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7b1f7-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="7b1f7-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b1f7-132">Response</span></span>
<span data-ttu-id="7b1f7-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7b1f7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



