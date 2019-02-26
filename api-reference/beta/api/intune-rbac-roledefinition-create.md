---
title: roleDefinition erstellen
description: Erstellt neue Objekte des Typs roleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e65aea19cfd10b08ec9db088e7df22250b85068b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153368"
---
# <a name="create-roledefinition"></a><span data-ttu-id="a4d76-103">roleDefinition erstellen</span><span class="sxs-lookup"><span data-stu-id="a4d76-103">Create roleDefinition</span></span>

> <span data-ttu-id="a4d76-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a4d76-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4d76-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a4d76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4d76-106">Erstellt neue Objekte des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a4d76-106">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4d76-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a4d76-107">Prerequisites</span></span>
<span data-ttu-id="a4d76-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a4d76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a4d76-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a4d76-110">Permission type</span></span>|<span data-ttu-id="a4d76-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a4d76-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4d76-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a4d76-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a4d76-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4d76-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="a4d76-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a4d76-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4d76-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a4d76-115">Not supported.</span></span>|
|<span data-ttu-id="a4d76-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a4d76-116">Application</span></span>|<span data-ttu-id="a4d76-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a4d76-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4d76-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a4d76-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="a4d76-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a4d76-119">Request headers</span></span>
|<span data-ttu-id="a4d76-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a4d76-120">Header</span></span>|<span data-ttu-id="a4d76-121">Wert</span><span class="sxs-lookup"><span data-stu-id="a4d76-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4d76-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4d76-122">Authorization</span></span>|<span data-ttu-id="a4d76-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a4d76-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4d76-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a4d76-124">Accept</span></span>|<span data-ttu-id="a4d76-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a4d76-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4d76-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a4d76-126">Request body</span></span>
<span data-ttu-id="a4d76-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs roleDefinition an.</span><span class="sxs-lookup"><span data-stu-id="a4d76-127">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="a4d76-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der roleDefinition erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="a4d76-128">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="a4d76-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a4d76-129">Property</span></span>|<span data-ttu-id="a4d76-130">Typ</span><span class="sxs-lookup"><span data-stu-id="a4d76-130">Type</span></span>|<span data-ttu-id="a4d76-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a4d76-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4d76-132">id</span><span class="sxs-lookup"><span data-stu-id="a4d76-132">id</span></span>|<span data-ttu-id="a4d76-133">String</span><span class="sxs-lookup"><span data-stu-id="a4d76-133">String</span></span>|<span data-ttu-id="a4d76-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a4d76-134">Key of the entity.</span></span> <span data-ttu-id="a4d76-135">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="a4d76-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="a4d76-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a4d76-136">displayName</span></span>|<span data-ttu-id="a4d76-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a4d76-137">String</span></span>|<span data-ttu-id="a4d76-138">Anzeigename der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="a4d76-138">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="a4d76-139">description</span><span class="sxs-lookup"><span data-stu-id="a4d76-139">description</span></span>|<span data-ttu-id="a4d76-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a4d76-140">String</span></span>|<span data-ttu-id="a4d76-141">Beschreibung der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="a4d76-141">Description of the Role definition.</span></span>|
|<span data-ttu-id="a4d76-142">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a4d76-142">permissions</span></span>|<span data-ttu-id="a4d76-143">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="a4d76-143">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="a4d76-144">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="a4d76-144">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="a4d76-145">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="a4d76-145">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="a4d76-146">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="a4d76-146">rolePermissions</span></span>|<span data-ttu-id="a4d76-147">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="a4d76-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="a4d76-148">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="a4d76-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="a4d76-149">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="a4d76-149">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="a4d76-150">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="a4d76-150">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="a4d76-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4d76-151">Boolean</span></span>|<span data-ttu-id="a4d76-152">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="a4d76-152">Type of Role.</span></span> <span data-ttu-id="a4d76-153">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="a4d76-153">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="a4d76-154">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="a4d76-154">isBuiltIn</span></span>|<span data-ttu-id="a4d76-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4d76-155">Boolean</span></span>|<span data-ttu-id="a4d76-156">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="a4d76-156">Type of Role.</span></span> <span data-ttu-id="a4d76-157">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="a4d76-157">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="a4d76-158">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="a4d76-158">roleScopeTagIds</span></span>|<span data-ttu-id="a4d76-159">String collection</span><span class="sxs-lookup"><span data-stu-id="a4d76-159">String collection</span></span>|<span data-ttu-id="a4d76-160">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="a4d76-160">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="a4d76-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="a4d76-161">Response</span></span>
<span data-ttu-id="a4d76-162">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [roleDefinition](../resources/intune-rbac-roledefinition.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a4d76-162">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4d76-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a4d76-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4d76-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a4d76-164">Request</span></span>
<span data-ttu-id="a4d76-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a4d76-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
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

### <a name="response"></a><span data-ttu-id="a4d76-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="a4d76-166">Response</span></span>
<span data-ttu-id="a4d76-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a4d76-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




