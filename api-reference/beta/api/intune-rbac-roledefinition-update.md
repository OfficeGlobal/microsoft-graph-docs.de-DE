---
title: roleDefinition aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs roleDefinition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dc06b734c0f18101c58347a239fffb60ffc158d0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149693"
---
# <a name="update-roledefinition"></a><span data-ttu-id="b54f3-103">roleDefinition aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b54f3-103">Update roleDefinition</span></span>

> <span data-ttu-id="b54f3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b54f3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b54f3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b54f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b54f3-106">Aktualisiert die Eigenschaften von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b54f3-106">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b54f3-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b54f3-107">Prerequisites</span></span>
<span data-ttu-id="b54f3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b54f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b54f3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b54f3-110">Permission type</span></span>|<span data-ttu-id="b54f3-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b54f3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b54f3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b54f3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b54f3-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b54f3-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="b54f3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b54f3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b54f3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b54f3-115">Not supported.</span></span>|
|<span data-ttu-id="b54f3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b54f3-116">Application</span></span>|<span data-ttu-id="b54f3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b54f3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b54f3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b54f3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="b54f3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b54f3-119">Request headers</span></span>
|<span data-ttu-id="b54f3-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b54f3-120">Header</span></span>|<span data-ttu-id="b54f3-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b54f3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b54f3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b54f3-122">Authorization</span></span>|<span data-ttu-id="b54f3-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b54f3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b54f3-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b54f3-124">Accept</span></span>|<span data-ttu-id="b54f3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b54f3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b54f3-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b54f3-126">Request body</span></span>
<span data-ttu-id="b54f3-127">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md) an.</span><span class="sxs-lookup"><span data-stu-id="b54f3-127">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="b54f3-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [roleDefinition](../resources/intune-rbac-roledefinition.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="b54f3-128">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="b54f3-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b54f3-129">Property</span></span>|<span data-ttu-id="b54f3-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b54f3-130">Type</span></span>|<span data-ttu-id="b54f3-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b54f3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b54f3-132">id</span><span class="sxs-lookup"><span data-stu-id="b54f3-132">id</span></span>|<span data-ttu-id="b54f3-133">String</span><span class="sxs-lookup"><span data-stu-id="b54f3-133">String</span></span>|<span data-ttu-id="b54f3-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b54f3-134">Key of the entity.</span></span> <span data-ttu-id="b54f3-135">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="b54f3-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="b54f3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b54f3-136">displayName</span></span>|<span data-ttu-id="b54f3-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b54f3-137">String</span></span>|<span data-ttu-id="b54f3-138">Anzeigename der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="b54f3-138">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="b54f3-139">description</span><span class="sxs-lookup"><span data-stu-id="b54f3-139">description</span></span>|<span data-ttu-id="b54f3-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b54f3-140">String</span></span>|<span data-ttu-id="b54f3-141">Beschreibung der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="b54f3-141">Description of the Role definition.</span></span>|
|<span data-ttu-id="b54f3-142">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b54f3-142">permissions</span></span>|<span data-ttu-id="b54f3-143">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="b54f3-143">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="b54f3-144">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="b54f3-144">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="b54f3-145">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="b54f3-145">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="b54f3-146">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="b54f3-146">rolePermissions</span></span>|<span data-ttu-id="b54f3-147">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="b54f3-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="b54f3-148">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="b54f3-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="b54f3-149">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="b54f3-149">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="b54f3-150">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="b54f3-150">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="b54f3-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="b54f3-151">Boolean</span></span>|<span data-ttu-id="b54f3-152">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="b54f3-152">Type of Role.</span></span> <span data-ttu-id="b54f3-153">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="b54f3-153">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="b54f3-154">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="b54f3-154">isBuiltIn</span></span>|<span data-ttu-id="b54f3-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="b54f3-155">Boolean</span></span>|<span data-ttu-id="b54f3-156">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="b54f3-156">Type of Role.</span></span> <span data-ttu-id="b54f3-157">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="b54f3-157">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="b54f3-158">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="b54f3-158">roleScopeTagIds</span></span>|<span data-ttu-id="b54f3-159">String collection</span><span class="sxs-lookup"><span data-stu-id="b54f3-159">String collection</span></span>|<span data-ttu-id="b54f3-160">Liste der Bereichs Tags für diese Entitätsinstanz.</span><span class="sxs-lookup"><span data-stu-id="b54f3-160">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="b54f3-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="b54f3-161">Response</span></span>
<span data-ttu-id="b54f3-162">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [roleDefinition](../resources/intune-rbac-roledefinition.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b54f3-162">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b54f3-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b54f3-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="b54f3-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b54f3-164">Request</span></span>
<span data-ttu-id="b54f3-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b54f3-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b54f3-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="b54f3-166">Response</span></span>
<span data-ttu-id="b54f3-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b54f3-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




