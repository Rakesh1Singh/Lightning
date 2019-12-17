# Create custom buttons and links that pass default field values to a new record.

To construct a custom button or link that launches a new record with prepopulated field values, use this sample formula:

```javascript
/lightning/o/Account/new?defaultFieldValues=
    Name={!URLENCODE(Account.Name)},
    OwnerId={!Account.OwnerId},
    AccountNumber={!Account.AccountNumber},
    NumberOfEmployees=35000,
    CustomCheckbox__c={!IF(Account.SomeCheckbox__c, true, false)}
```
