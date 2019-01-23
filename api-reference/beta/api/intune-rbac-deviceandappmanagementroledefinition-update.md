---
title: deviceAndAppManagementRoleDefinition aktualisieren
description: Aktualisieren der Eigenschaften eines deviceAndAppManagementRoleDefinition-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a881c0242a8414b071c03de85a733ad9296200b2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394012"
---
# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="f1735-103">deviceAndAppManagementRoleDefinition aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f1735-103">Update deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="f1735-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f1735-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f1735-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f1735-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1735-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f1735-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1735-107">Aktualisieren der Eigenschaften eines [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f1735-107">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1735-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f1735-108">Prerequisites</span></span>
<span data-ttu-id="f1735-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f1735-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f1735-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f1735-111">Permission type</span></span>|<span data-ttu-id="f1735-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f1735-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1735-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f1735-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1735-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1735-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="f1735-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f1735-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1735-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1735-116">Not supported.</span></span>|
|<span data-ttu-id="f1735-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f1735-117">Application</span></span>|<span data-ttu-id="f1735-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1735-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1735-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1735-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="f1735-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f1735-120">Request headers</span></span>
|<span data-ttu-id="f1735-121">Header</span><span class="sxs-lookup"><span data-stu-id="f1735-121">Header</span></span>|<span data-ttu-id="f1735-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f1735-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1735-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f1735-123">Authorization</span></span>|<span data-ttu-id="f1735-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f1735-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1735-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f1735-125">Accept</span></span>|<span data-ttu-id="f1735-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1735-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1735-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f1735-127">Request body</span></span>
<span data-ttu-id="f1735-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f1735-128">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="f1735-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="f1735-129">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="f1735-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f1735-130">Property</span></span>|<span data-ttu-id="f1735-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f1735-131">Type</span></span>|<span data-ttu-id="f1735-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f1735-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1735-133">id</span><span class="sxs-lookup"><span data-stu-id="f1735-133">id</span></span>|<span data-ttu-id="f1735-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f1735-134">String</span></span>|<span data-ttu-id="f1735-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f1735-135">Key of the entity.</span></span> <span data-ttu-id="f1735-136">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="f1735-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="f1735-137">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f1735-137">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f1735-138">displayName</span><span class="sxs-lookup"><span data-stu-id="f1735-138">displayName</span></span>|<span data-ttu-id="f1735-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f1735-139">String</span></span>|<span data-ttu-id="f1735-140">Anzeigename der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="f1735-140">Display Name of the Role definition.</span></span> <span data-ttu-id="f1735-141">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f1735-141">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f1735-142">description</span><span class="sxs-lookup"><span data-stu-id="f1735-142">description</span></span>|<span data-ttu-id="f1735-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f1735-143">String</span></span>|<span data-ttu-id="f1735-144">Beschreibung der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="f1735-144">Description of the Role definition.</span></span> <span data-ttu-id="f1735-145">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f1735-145">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f1735-146">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f1735-146">permissions</span></span>|<span data-ttu-id="f1735-147">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="f1735-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="f1735-148">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="f1735-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="f1735-149">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="f1735-149">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="f1735-150">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f1735-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f1735-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="f1735-151">rolePermissions</span></span>|<span data-ttu-id="f1735-152">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="f1735-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="f1735-153">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="f1735-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="f1735-154">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="f1735-154">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="f1735-155">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f1735-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f1735-156">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="f1735-156">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="f1735-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1735-157">Boolean</span></span>|<span data-ttu-id="f1735-158">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="f1735-158">Type of Role.</span></span> <span data-ttu-id="f1735-159">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="f1735-159">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="f1735-160">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f1735-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f1735-161">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="f1735-161">isBuiltIn</span></span>|<span data-ttu-id="f1735-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1735-162">Boolean</span></span>|<span data-ttu-id="f1735-163">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="f1735-163">Type of Role.</span></span> <span data-ttu-id="f1735-164">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="f1735-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="f1735-165">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f1735-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="f1735-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f1735-166">roleScopeTagIds</span></span>|<span data-ttu-id="f1735-167">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="f1735-167">String collection</span></span>|<span data-ttu-id="f1735-168">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="f1735-168">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f1735-169">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f1735-169">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f1735-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1735-170">Response</span></span>
<span data-ttu-id="f1735-171">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f1735-171">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1735-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f1735-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1735-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1735-173">Request</span></span>
<span data-ttu-id="f1735-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f1735-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}
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

### <a name="response"></a><span data-ttu-id="f1735-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1735-175">Response</span></span>
<span data-ttu-id="f1735-p111">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f1735-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




