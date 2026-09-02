# ParticipationCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**acquired_at** | **date** | Datum des Erwerbs der Beteiligung. | [optional] 
**board_appointment** | **bool** | Bestellungsrecht für Geschäftsführung/Aufsichtsrat (§ 290 Abs. 2 Nr. 2 HGB). | [optional] 
**company_name** | **str** | Name des Beteiligungsunternehmens (§ 271 HGB). | [optional] 
**control_agreement** | **bool** | Beherrschungsvertrag (§ 290 Abs. 2 Nr. 3 HGB). | [optional] 
**legal_form** | **str** | Rechtsform, z. B. \&quot;GmbH\&quot;. | [optional] 
**ownership_pct** | **str** | Anteilsquote in Prozent (§ 271 HGB; &gt; 20 % widerlegbare Vermutung). | [optional] 
**purpose_vehicle** | **bool** | Zweckgesellschaft (§ 290 Abs. 2 Nr. 4 HGB). | [optional] 
**voting_majority** | **bool** | Stimmrechtsmehrheit (§ 290 Abs. 2 Nr. 1 HGB). | [optional] 

## Example

```python
from simplebilly_api.models.participation_create import ParticipationCreate

# TODO update the JSON string below
json = "{}"
# create an instance of ParticipationCreate from a JSON string
participation_create_instance = ParticipationCreate.from_json(json)
# print the JSON string representation of the object
print(ParticipationCreate.to_json())

# convert the object into a dict
participation_create_dict = participation_create_instance.to_dict()
# create an instance of ParticipationCreate from a dict
participation_create_from_dict = ParticipationCreate.from_dict(participation_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


