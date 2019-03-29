---
title: deviceAndAppManagementRoleDefinition erstellen
description: Erstellen eines neuen deviceAndAppManagementRoleDefinition-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f6ca8009eeb873cd10fdec05a444e49ea74517bb
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970751"
---
# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="5e213-103">deviceAndAppManagementRoleDefinition erstellen</span><span class="sxs-lookup"><span data-stu-id="5e213-103">Create deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="5e213-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5e213-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e213-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5e213-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e213-106">Erstellen eines neuen [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5e213-106">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e213-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5e213-107">Prerequisites</span></span>
<span data-ttu-id="5e213-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e213-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e213-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5e213-110">Permission type</span></span>|<span data-ttu-id="5e213-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5e213-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e213-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5e213-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5e213-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e213-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="5e213-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5e213-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e213-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5e213-115">Not supported.</span></span>|
|<span data-ttu-id="5e213-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5e213-116">Application</span></span>|<span data-ttu-id="5e213-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5e213-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e213-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5e213-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="5e213-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5e213-119">Request headers</span></span>
|<span data-ttu-id="5e213-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5e213-120">Header</span></span>|<span data-ttu-id="5e213-121">Wert</span><span class="sxs-lookup"><span data-stu-id="5e213-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e213-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e213-122">Authorization</span></span>|<span data-ttu-id="5e213-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5e213-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e213-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5e213-124">Accept</span></span>|<span data-ttu-id="5e213-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5e213-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e213-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5e213-126">Request body</span></span>
<span data-ttu-id="5e213-127">Geben Sie im Anforderungstext eine JSON-Darstellung des deviceAndAppManagementRoleDefinition-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="5e213-127">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="5e213-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceAndAppManagementRoleDefinition erstellen.</span><span class="sxs-lookup"><span data-stu-id="5e213-128">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="5e213-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5e213-129">Property</span></span>|<span data-ttu-id="5e213-130">Typ</span><span class="sxs-lookup"><span data-stu-id="5e213-130">Type</span></span>|<span data-ttu-id="5e213-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5e213-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e213-132">id</span><span class="sxs-lookup"><span data-stu-id="5e213-132">id</span></span>|<span data-ttu-id="5e213-133">String</span><span class="sxs-lookup"><span data-stu-id="5e213-133">String</span></span>|<span data-ttu-id="5e213-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5e213-134">Key of the entity.</span></span> <span data-ttu-id="5e213-135">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="5e213-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="5e213-136">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5e213-136">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5e213-137">displayName</span><span class="sxs-lookup"><span data-stu-id="5e213-137">displayName</span></span>|<span data-ttu-id="5e213-138">String</span><span class="sxs-lookup"><span data-stu-id="5e213-138">String</span></span>|<span data-ttu-id="5e213-139">Anzeigename der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="5e213-139">Display Name of the Role definition.</span></span> <span data-ttu-id="5e213-140">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5e213-140">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5e213-141">description</span><span class="sxs-lookup"><span data-stu-id="5e213-141">description</span></span>|<span data-ttu-id="5e213-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5e213-142">String</span></span>|<span data-ttu-id="5e213-143">Beschreibung der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="5e213-143">Description of the Role definition.</span></span> <span data-ttu-id="5e213-144">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5e213-144">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5e213-145">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5e213-145">permissions</span></span>|<span data-ttu-id="5e213-146">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="5e213-146">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="5e213-147">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="5e213-147">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="5e213-148">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="5e213-148">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="5e213-149">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5e213-149">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5e213-150">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="5e213-150">rolePermissions</span></span>|<span data-ttu-id="5e213-151">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="5e213-151">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="5e213-152">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="5e213-152">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="5e213-153">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="5e213-153">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="5e213-154">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5e213-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5e213-155">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="5e213-155">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="5e213-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e213-156">Boolean</span></span>|<span data-ttu-id="5e213-157">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="5e213-157">Type of Role.</span></span> <span data-ttu-id="5e213-158">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="5e213-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="5e213-159">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5e213-159">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5e213-160">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="5e213-160">isBuiltIn</span></span>|<span data-ttu-id="5e213-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e213-161">Boolean</span></span>|<span data-ttu-id="5e213-162">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="5e213-162">Type of Role.</span></span> <span data-ttu-id="5e213-163">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="5e213-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="5e213-164">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5e213-164">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5e213-165">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="5e213-165">roleScopeTagIds</span></span>|<span data-ttu-id="5e213-166">String collection</span><span class="sxs-lookup"><span data-stu-id="5e213-166">String collection</span></span>|<span data-ttu-id="5e213-167">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="5e213-167">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5e213-168">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5e213-168">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="5e213-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="5e213-169">Response</span></span>
<span data-ttu-id="5e213-170">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5e213-170">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e213-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5e213-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e213-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5e213-172">Request</span></span>
<span data-ttu-id="5e213-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5e213-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
Content-type: application/json
Content-length: 1229

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
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

### <a name="response"></a><span data-ttu-id="5e213-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="5e213-174">Response</span></span>
<span data-ttu-id="5e213-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5e213-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1278

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
```




