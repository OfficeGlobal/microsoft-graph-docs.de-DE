---
title: deviceAndAppManagementRoleDefinition erstellen
description: Erstellen eines neuen deviceAndAppManagementRoleDefinition-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9017d2cd02fa7ef9594efb62b168ce70fc4dd259
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139578"
---
# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="ca7e7-103">deviceAndAppManagementRoleDefinition erstellen</span><span class="sxs-lookup"><span data-stu-id="ca7e7-103">Create deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="ca7e7-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ca7e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca7e7-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ca7e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca7e7-106">Erstellen eines neuen [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ca7e7-106">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca7e7-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ca7e7-107">Prerequisites</span></span>
<span data-ttu-id="ca7e7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ca7e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ca7e7-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ca7e7-110">Permission type</span></span>|<span data-ttu-id="ca7e7-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ca7e7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca7e7-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ca7e7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ca7e7-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca7e7-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="ca7e7-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ca7e7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca7e7-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ca7e7-115">Not supported.</span></span>|
|<span data-ttu-id="ca7e7-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ca7e7-116">Application</span></span>|<span data-ttu-id="ca7e7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ca7e7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca7e7-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ca7e7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="ca7e7-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ca7e7-119">Request headers</span></span>
|<span data-ttu-id="ca7e7-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ca7e7-120">Header</span></span>|<span data-ttu-id="ca7e7-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ca7e7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca7e7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca7e7-122">Authorization</span></span>|<span data-ttu-id="ca7e7-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ca7e7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca7e7-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ca7e7-124">Accept</span></span>|<span data-ttu-id="ca7e7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ca7e7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca7e7-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ca7e7-126">Request body</span></span>
<span data-ttu-id="ca7e7-127">Geben Sie im Anforderungstext eine JSON-Darstellung des deviceAndAppManagementRoleDefinition-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="ca7e7-127">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="ca7e7-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceAndAppManagementRoleDefinition erstellen.</span><span class="sxs-lookup"><span data-stu-id="ca7e7-128">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="ca7e7-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ca7e7-129">Property</span></span>|<span data-ttu-id="ca7e7-130">Typ</span><span class="sxs-lookup"><span data-stu-id="ca7e7-130">Type</span></span>|<span data-ttu-id="ca7e7-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ca7e7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca7e7-132">id</span><span class="sxs-lookup"><span data-stu-id="ca7e7-132">id</span></span>|<span data-ttu-id="ca7e7-133">String</span><span class="sxs-lookup"><span data-stu-id="ca7e7-133">String</span></span>|<span data-ttu-id="ca7e7-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ca7e7-134">Key of the entity.</span></span> <span data-ttu-id="ca7e7-135">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="ca7e7-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="ca7e7-136">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ca7e7-136">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ca7e7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ca7e7-137">displayName</span></span>|<span data-ttu-id="ca7e7-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca7e7-138">String</span></span>|<span data-ttu-id="ca7e7-139">Anzeigename der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="ca7e7-139">Display Name of the Role definition.</span></span> <span data-ttu-id="ca7e7-140">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ca7e7-140">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ca7e7-141">description</span><span class="sxs-lookup"><span data-stu-id="ca7e7-141">description</span></span>|<span data-ttu-id="ca7e7-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca7e7-142">String</span></span>|<span data-ttu-id="ca7e7-143">Beschreibung der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="ca7e7-143">Description of the Role definition.</span></span> <span data-ttu-id="ca7e7-144">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ca7e7-144">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ca7e7-145">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ca7e7-145">permissions</span></span>|<span data-ttu-id="ca7e7-146">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="ca7e7-146">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="ca7e7-147">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="ca7e7-147">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="ca7e7-148">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="ca7e7-148">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="ca7e7-149">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ca7e7-149">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ca7e7-150">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="ca7e7-150">rolePermissions</span></span>|<span data-ttu-id="ca7e7-151">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="ca7e7-151">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="ca7e7-152">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="ca7e7-152">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="ca7e7-153">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="ca7e7-153">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="ca7e7-154">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ca7e7-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ca7e7-155">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ca7e7-155">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="ca7e7-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ca7e7-156">Boolean</span></span>|<span data-ttu-id="ca7e7-157">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="ca7e7-157">Type of Role.</span></span> <span data-ttu-id="ca7e7-158">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="ca7e7-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="ca7e7-159">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ca7e7-159">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ca7e7-160">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="ca7e7-160">isBuiltIn</span></span>|<span data-ttu-id="ca7e7-161">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ca7e7-161">Boolean</span></span>|<span data-ttu-id="ca7e7-162">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="ca7e7-162">Type of Role.</span></span> <span data-ttu-id="ca7e7-163">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="ca7e7-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="ca7e7-164">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ca7e7-164">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ca7e7-165">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="ca7e7-165">roleScopeTagIds</span></span>|<span data-ttu-id="ca7e7-166">String collection</span><span class="sxs-lookup"><span data-stu-id="ca7e7-166">String collection</span></span>|<span data-ttu-id="ca7e7-167">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="ca7e7-167">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ca7e7-168">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ca7e7-168">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ca7e7-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="ca7e7-169">Response</span></span>
<span data-ttu-id="ca7e7-170">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ca7e7-170">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca7e7-171">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ca7e7-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca7e7-172">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ca7e7-172">Request</span></span>
<span data-ttu-id="ca7e7-173">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ca7e7-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ca7e7-174">Antwort</span><span class="sxs-lookup"><span data-stu-id="ca7e7-174">Response</span></span>
<span data-ttu-id="ca7e7-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ca7e7-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




