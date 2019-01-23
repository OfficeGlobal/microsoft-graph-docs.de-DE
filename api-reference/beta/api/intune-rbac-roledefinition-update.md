---
title: roleDefinition aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs roleDefinition.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b13f82e30e8bf67a78bd31db678de5b5a46051c3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412625"
---
# <a name="update-roledefinition"></a><span data-ttu-id="575bd-103">roleDefinition aktualisieren</span><span class="sxs-lookup"><span data-stu-id="575bd-103">Update roleDefinition</span></span>

> <span data-ttu-id="575bd-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="575bd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="575bd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="575bd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="575bd-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="575bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="575bd-107">Aktualisiert die Eigenschaften von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="575bd-107">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="575bd-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="575bd-108">Prerequisites</span></span>
<span data-ttu-id="575bd-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="575bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="575bd-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="575bd-111">Permission type</span></span>|<span data-ttu-id="575bd-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="575bd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="575bd-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="575bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="575bd-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="575bd-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="575bd-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="575bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="575bd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="575bd-116">Not supported.</span></span>|
|<span data-ttu-id="575bd-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="575bd-117">Application</span></span>|<span data-ttu-id="575bd-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="575bd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="575bd-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="575bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="575bd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="575bd-120">Request headers</span></span>
|<span data-ttu-id="575bd-121">Header</span><span class="sxs-lookup"><span data-stu-id="575bd-121">Header</span></span>|<span data-ttu-id="575bd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="575bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="575bd-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="575bd-123">Authorization</span></span>|<span data-ttu-id="575bd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="575bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="575bd-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="575bd-125">Accept</span></span>|<span data-ttu-id="575bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="575bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="575bd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="575bd-127">Request body</span></span>
<span data-ttu-id="575bd-128">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md) an.</span><span class="sxs-lookup"><span data-stu-id="575bd-128">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="575bd-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [roleDefinition](../resources/intune-rbac-roledefinition.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="575bd-129">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="575bd-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="575bd-130">Property</span></span>|<span data-ttu-id="575bd-131">Typ</span><span class="sxs-lookup"><span data-stu-id="575bd-131">Type</span></span>|<span data-ttu-id="575bd-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="575bd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="575bd-133">id</span><span class="sxs-lookup"><span data-stu-id="575bd-133">id</span></span>|<span data-ttu-id="575bd-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="575bd-134">String</span></span>|<span data-ttu-id="575bd-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="575bd-135">Key of the entity.</span></span> <span data-ttu-id="575bd-136">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="575bd-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="575bd-137">displayName</span><span class="sxs-lookup"><span data-stu-id="575bd-137">displayName</span></span>|<span data-ttu-id="575bd-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="575bd-138">String</span></span>|<span data-ttu-id="575bd-139">Anzeigename der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="575bd-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="575bd-140">description</span><span class="sxs-lookup"><span data-stu-id="575bd-140">description</span></span>|<span data-ttu-id="575bd-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="575bd-141">String</span></span>|<span data-ttu-id="575bd-142">Beschreibung der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="575bd-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="575bd-143">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="575bd-143">permissions</span></span>|<span data-ttu-id="575bd-144">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="575bd-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="575bd-145">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="575bd-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="575bd-146">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="575bd-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="575bd-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="575bd-147">rolePermissions</span></span>|<span data-ttu-id="575bd-148">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="575bd-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="575bd-149">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="575bd-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="575bd-150">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="575bd-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="575bd-151">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="575bd-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="575bd-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="575bd-152">Boolean</span></span>|<span data-ttu-id="575bd-153">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="575bd-153">Type of Role.</span></span> <span data-ttu-id="575bd-154">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="575bd-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="575bd-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="575bd-155">isBuiltIn</span></span>|<span data-ttu-id="575bd-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="575bd-156">Boolean</span></span>|<span data-ttu-id="575bd-157">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="575bd-157">Type of Role.</span></span> <span data-ttu-id="575bd-158">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="575bd-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="575bd-159">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="575bd-159">roleScopeTagIds</span></span>|<span data-ttu-id="575bd-160">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="575bd-160">String collection</span></span>|<span data-ttu-id="575bd-161">Liste der Bereich Tags für diese Instanz der Entität.</span><span class="sxs-lookup"><span data-stu-id="575bd-161">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="575bd-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="575bd-162">Response</span></span>
<span data-ttu-id="575bd-163">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [roleDefinition](../resources/intune-rbac-roledefinition.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="575bd-163">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="575bd-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="575bd-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="575bd-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="575bd-165">Request</span></span>
<span data-ttu-id="575bd-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="575bd-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="575bd-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="575bd-167">Response</span></span>
<span data-ttu-id="575bd-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="575bd-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




