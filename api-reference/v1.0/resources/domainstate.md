<span data-ttu-id="06a8a-p102">Typ des asynchronen Vorgangs. Mögliche Werte sind *ForceDelete* und *Verification*</span><span class="sxs-lookup"><span data-stu-id="06a8a-p102">Type of asynchronous operation. The values can be *ForceDelete* or *Verification*</span></span> | Typ des asynchronen Vorgangs. Mögliche Werte sind *ForceDelete* und *Verification* |
| <span data-ttu-id="06a8a-115">status</span><span class="sxs-lookup"><span data-stu-id="06a8a-115">status</span></span> | <span data-ttu-id="06a8a-116">String</span><span class="sxs-lookup"><span data-stu-id="06a8a-116">String</span></span> | <span data-ttu-id="06a8a-117">Der aktuellen Status des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="06a8a-117">Current status of the operation.</span></span> <br> <span data-ttu-id="06a8a-118">*Scheduled*: Der Vorgang wurde geplant, aber noch nicht gestartet.</span><span class="sxs-lookup"><span data-stu-id="06a8a-118">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="06a8a-119">*InProgress*: Der Vorgang wurde gestartet und wird ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="06a8a-119">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="06a8a-120">*Failed*: Ein Fehler ist im Vorgang aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="06a8a-120">*Failed* - Operation has failed.</span></span> |

## <span data-ttu-id="06a8a-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="06a8a-121">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="06a8a-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="06a8a-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainState"
}-->

```json
{
  "lastActionDateTime": "String (timestamp)",
  "operation": "String",
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->