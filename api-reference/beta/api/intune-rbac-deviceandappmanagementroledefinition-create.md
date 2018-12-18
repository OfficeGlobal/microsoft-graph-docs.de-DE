---
title: deviceAndAppManagementRoleDefinition erstellen
description: Erstellen eines neuen deviceAndAppManagementRoleDefinition-Objekts.
author: tfitzmac
ms.openlocfilehash: fdf6e4b1a4c80456c51b8a155974c5cd8d9728bc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339942"
---
# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="d4d12-103">deviceAndAppManagementRoleDefinition erstellen</span><span class="sxs-lookup"><span data-stu-id="d4d12-103">Create deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="d4d12-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d4d12-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4d12-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d4d12-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4d12-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d4d12-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4d12-107">Erstellen eines neuen [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d4d12-107">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d4d12-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d4d12-108">Prerequisites</span></span>
<span data-ttu-id="d4d12-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4d12-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4d12-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d4d12-111">Permission type</span></span>|<span data-ttu-id="d4d12-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d4d12-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4d12-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d4d12-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4d12-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4d12-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="d4d12-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d4d12-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4d12-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4d12-116">Not supported.</span></span>|
|<span data-ttu-id="d4d12-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d4d12-117">Application</span></span>|<span data-ttu-id="d4d12-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4d12-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4d12-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4d12-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="d4d12-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d4d12-120">Request headers</span></span>
|<span data-ttu-id="d4d12-121">Header</span><span class="sxs-lookup"><span data-stu-id="d4d12-121">Header</span></span>|<span data-ttu-id="d4d12-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d4d12-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4d12-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d4d12-123">Authorization</span></span>|<span data-ttu-id="d4d12-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d4d12-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4d12-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d4d12-125">Accept</span></span>|<span data-ttu-id="d4d12-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4d12-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4d12-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d4d12-127">Request body</span></span>
<span data-ttu-id="d4d12-128">Geben Sie im Anforderungstext eine JSON-Darstellung des deviceAndAppManagementRoleDefinition-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="d4d12-128">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="d4d12-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs deviceAndAppManagementRoleDefinition erstellen.</span><span class="sxs-lookup"><span data-stu-id="d4d12-129">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="d4d12-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d4d12-130">Property</span></span>|<span data-ttu-id="d4d12-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d4d12-131">Type</span></span>|<span data-ttu-id="d4d12-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4d12-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4d12-133">id</span><span class="sxs-lookup"><span data-stu-id="d4d12-133">id</span></span>|<span data-ttu-id="d4d12-134">String</span><span class="sxs-lookup"><span data-stu-id="d4d12-134">String</span></span>|<span data-ttu-id="d4d12-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d4d12-135">Key of the entity.</span></span> <span data-ttu-id="d4d12-136">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="d4d12-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="d4d12-137">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d4d12-137">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="d4d12-138">displayName</span><span class="sxs-lookup"><span data-stu-id="d4d12-138">displayName</span></span>|<span data-ttu-id="d4d12-139">String</span><span class="sxs-lookup"><span data-stu-id="d4d12-139">String</span></span>|<span data-ttu-id="d4d12-140">Anzeigename der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="d4d12-140">Display Name of the Role definition.</span></span> <span data-ttu-id="d4d12-141">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d4d12-141">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="d4d12-142">description</span><span class="sxs-lookup"><span data-stu-id="d4d12-142">description</span></span>|<span data-ttu-id="d4d12-143">String</span><span class="sxs-lookup"><span data-stu-id="d4d12-143">String</span></span>|<span data-ttu-id="d4d12-144">Beschreibung der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="d4d12-144">Description of the Role definition.</span></span> <span data-ttu-id="d4d12-145">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d4d12-145">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="d4d12-146">permissions</span><span class="sxs-lookup"><span data-stu-id="d4d12-146">permissions</span></span>|<span data-ttu-id="d4d12-147">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="d4d12-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="d4d12-148">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="d4d12-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="d4d12-149">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="d4d12-149">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="d4d12-150">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d4d12-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="d4d12-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="d4d12-151">rolePermissions</span></span>|<span data-ttu-id="d4d12-152">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="d4d12-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="d4d12-153">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="d4d12-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="d4d12-154">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="d4d12-154">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="d4d12-155">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d4d12-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="d4d12-156">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d4d12-156">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="d4d12-157">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d4d12-157">Boolean</span></span>|<span data-ttu-id="d4d12-158">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="d4d12-158">Type of Role.</span></span> <span data-ttu-id="d4d12-159">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="d4d12-159">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="d4d12-160">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d4d12-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="d4d12-161">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="d4d12-161">isBuiltIn</span></span>|<span data-ttu-id="d4d12-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d4d12-162">Boolean</span></span>|<span data-ttu-id="d4d12-163">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="d4d12-163">Type of Role.</span></span> <span data-ttu-id="d4d12-164">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="d4d12-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="d4d12-165">Geerbt von [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d4d12-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d4d12-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4d12-166">Response</span></span>
<span data-ttu-id="d4d12-167">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d4d12-167">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4d12-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d4d12-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="d4d12-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4d12-169">Request</span></span>
<span data-ttu-id="d4d12-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d4d12-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
Content-type: application/json
Content-length: 1167

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
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="d4d12-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4d12-171">Response</span></span>
<span data-ttu-id="d4d12-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d4d12-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1216

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
  "isBuiltIn": true
}
```





