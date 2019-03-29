---
title: roleDefinition aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs roleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5716202d2b6e9ca29e7561c839055096e7a6da8b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973313"
---
# <a name="update-roledefinition"></a><span data-ttu-id="58f58-103">roleDefinition aktualisieren</span><span class="sxs-lookup"><span data-stu-id="58f58-103">Update roleDefinition</span></span>

> <span data-ttu-id="58f58-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="58f58-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58f58-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="58f58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58f58-106">Aktualisiert die Eigenschaften von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="58f58-106">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58f58-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="58f58-107">Prerequisites</span></span>
<span data-ttu-id="58f58-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58f58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58f58-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="58f58-110">Permission type</span></span>|<span data-ttu-id="58f58-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="58f58-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58f58-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="58f58-112">Delegated (work or school account)</span></span>|<span data-ttu-id="58f58-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58f58-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="58f58-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="58f58-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58f58-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58f58-115">Not supported.</span></span>|
|<span data-ttu-id="58f58-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="58f58-116">Application</span></span>|<span data-ttu-id="58f58-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58f58-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58f58-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="58f58-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="58f58-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="58f58-119">Request headers</span></span>
|<span data-ttu-id="58f58-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="58f58-120">Header</span></span>|<span data-ttu-id="58f58-121">Wert</span><span class="sxs-lookup"><span data-stu-id="58f58-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58f58-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="58f58-122">Authorization</span></span>|<span data-ttu-id="58f58-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="58f58-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58f58-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="58f58-124">Accept</span></span>|<span data-ttu-id="58f58-125">application/json</span><span class="sxs-lookup"><span data-stu-id="58f58-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58f58-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="58f58-126">Request body</span></span>
<span data-ttu-id="58f58-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md) an.</span><span class="sxs-lookup"><span data-stu-id="58f58-127">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="58f58-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [roleDefinition](../resources/intune-rbac-roledefinition.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="58f58-128">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="58f58-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="58f58-129">Property</span></span>|<span data-ttu-id="58f58-130">Typ</span><span class="sxs-lookup"><span data-stu-id="58f58-130">Type</span></span>|<span data-ttu-id="58f58-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="58f58-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58f58-132">id</span><span class="sxs-lookup"><span data-stu-id="58f58-132">id</span></span>|<span data-ttu-id="58f58-133">String</span><span class="sxs-lookup"><span data-stu-id="58f58-133">String</span></span>|<span data-ttu-id="58f58-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="58f58-134">Key of the entity.</span></span> <span data-ttu-id="58f58-135">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="58f58-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="58f58-136">displayName</span><span class="sxs-lookup"><span data-stu-id="58f58-136">displayName</span></span>|<span data-ttu-id="58f58-137">String</span><span class="sxs-lookup"><span data-stu-id="58f58-137">String</span></span>|<span data-ttu-id="58f58-138">Anzeigename der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="58f58-138">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="58f58-139">description</span><span class="sxs-lookup"><span data-stu-id="58f58-139">description</span></span>|<span data-ttu-id="58f58-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="58f58-140">String</span></span>|<span data-ttu-id="58f58-141">Beschreibung der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="58f58-141">Description of the Role definition.</span></span>|
|<span data-ttu-id="58f58-142">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="58f58-142">permissions</span></span>|<span data-ttu-id="58f58-143">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="58f58-143">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="58f58-144">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="58f58-144">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="58f58-145">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="58f58-145">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="58f58-146">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="58f58-146">rolePermissions</span></span>|<span data-ttu-id="58f58-147">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="58f58-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="58f58-148">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="58f58-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="58f58-149">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="58f58-149">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="58f58-150">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="58f58-150">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="58f58-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="58f58-151">Boolean</span></span>|<span data-ttu-id="58f58-152">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="58f58-152">Type of Role.</span></span> <span data-ttu-id="58f58-153">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="58f58-153">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="58f58-154">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="58f58-154">isBuiltIn</span></span>|<span data-ttu-id="58f58-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="58f58-155">Boolean</span></span>|<span data-ttu-id="58f58-156">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="58f58-156">Type of Role.</span></span> <span data-ttu-id="58f58-157">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="58f58-157">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="58f58-158">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="58f58-158">roleScopeTagIds</span></span>|<span data-ttu-id="58f58-159">String collection</span><span class="sxs-lookup"><span data-stu-id="58f58-159">String collection</span></span>|<span data-ttu-id="58f58-160">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="58f58-160">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="58f58-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="58f58-161">Response</span></span>
<span data-ttu-id="58f58-162">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [roleDefinition](../resources/intune-rbac-roledefinition.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58f58-162">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58f58-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="58f58-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="58f58-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="58f58-164">Request</span></span>
<span data-ttu-id="58f58-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="58f58-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 1207

{
  "@odata.type": "#microsoft.graph.roleDefinition",
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
```

### <a name="response"></a><span data-ttu-id="58f58-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="58f58-166">Response</span></span>
<span data-ttu-id="58f58-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58f58-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1256

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
```




