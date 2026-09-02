# ContactUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_holder** | **str** |  | [optional] 
**acquisition_cost** | **str** |  | [optional] 
**address_supplement** | **str** |  | [optional] 
**attention** | **str** |  | [optional] 
**bank_name** | **str** |  | [optional] 
**bic** | **str** |  | [optional] 
**buyer_reference** | **str** |  | [optional] 
**category** | **str** |  | [optional] 
**certificate_authority** | **str** |  | [optional] 
**certificate_number** | **str** |  | [optional] 
**certificate_paragraph** | **str** |  | [optional] 
**certificate_valid_until** | **date** |  | [optional] 
**city** | **str** |  | [optional] 
**company_name** | **str** |  | [optional] 
**contact_persons** | **object** |  | [optional] 
**contact_type** | [**ContactType**](ContactType.md) |  | [optional] 
**country** | [**CountryCode**](CountryCode.md) |  | [optional] 
**credit_limit** | **str** |  | [optional] 
**creditor_account_skr03** | **str** |  | [optional] 
**creditor_account_skr04** | **str** |  | [optional] 
**currency** | **str** |  | [optional] 
**custom_fields** | **object** |  | [optional] 
**customer_number** | **str** |  | [optional] 
**debitor_account_skr03** | **str** |  | [optional] 
**debitor_account_skr04** | **str** |  | [optional] 
**default_debitor_number** | **str** |  | [optional] 
**delivery_block** | **bool** |  | [optional] 
**department** | **str** |  | [optional] 
**discount_days** | **int** |  | [optional] 
**discount_percentage** | **str** |  | [optional] 
**donation_receipt_eligible** | **bool** |  | [optional] 
**email** | **str** |  | [optional] 
**external_id** | **str** |  | [optional] 
**fax** | **str** |  | [optional] 
**iban** | **str** |  | [optional] 
**industry** | **str** |  | [optional] 
**is_active** | **bool** |  | [optional] 
**is_member** | **bool** |  | [optional] 
**is_nonprofit** | **bool** |  | [optional] 
**last_contact_date** | **date** |  | [optional] 
**last_purchase_date** | **date** |  | [optional] 
**leitweg_id** | **str** |  | [optional] 
**lifetime_value** | **str** |  | [optional] 
**mandate_date** | **date** |  | [optional] 
**mandate_reference** | **str** |  | [optional] 
**marketing_consent** | **bool** |  | [optional] 
**marketing_consent_at** | **datetime** |  | [optional] 
**marketing_consent_source** | **str** |  | [optional] 
**mobile** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**next_contact_date** | **date** |  | [optional] 
**notes** | **str** |  | [optional] 
**opening_balance** | **str** |  | [optional] 
**opening_balance_date** | **date** |  | [optional] 
**order_reference** | **str** |  | [optional] 
**payment_block** | **bool** |  | [optional] 
**payment_grace_period_days** | **int** |  | [optional] 
**payment_methods** | **List[str]** |  | [optional] 
**payment_terms** | **str** |  | [optional] 
**phone** | **str** |  | [optional] 
**rating** | **int** |  | [optional] 
**sales_representative** | **str** |  | [optional] 
**sepa_batch_booking** | **bool** |  | [optional] 
**sepa_sequence_type** | [**SepaSequenceType**](SepaSequenceType.md) |  | [optional] 
**social_media** | **object** |  | [optional] 
**source** | **str** |  | [optional] 
**state** | **str** |  | [optional] 
**street** | **str** |  | [optional] 
**street_number** | **str** |  | [optional] 
**supplier_number** | **str** |  | [optional] 
**tags** | **List[str]** |  | [optional] 
**tax_country** | [**CountryCode**](CountryCode.md) |  | [optional] 
**tax_number** | **str** |  | [optional] 
**tax_office** | **str** |  | [optional] 
**total_invoices** | **int** |  | [optional] 
**total_revenue** | **str** |  | [optional] 
**vat_id** | **str** |  | [optional] 
**vat_id_validated** | **bool** |  | [optional] 
**vat_id_validation_date** | **date** |  | [optional] 
**website** | **str** |  | [optional] 
**zip** | **str** |  | [optional] 

## Example

```python
from simplebilly_api.models.contact_update import ContactUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of ContactUpdate from a JSON string
contact_update_instance = ContactUpdate.from_json(json)
# print the JSON string representation of the object
print(ContactUpdate.to_json())

# convert the object into a dict
contact_update_dict = contact_update_instance.to_dict()
# create an instance of ContactUpdate from a dict
contact_update_from_dict = ContactUpdate.from_dict(contact_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


