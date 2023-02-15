# Form Started

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "form_start",
  "detailed_event": "Form Started",
    "event_data": {
        "form_field_id": "<form_field_id>",
        "form_field_position": "<form_field_position>",
        "form_field_section": "<form_field_section>",
        "identifier": "<identifier>",
        "name": "<name>",
        "type": "<type>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.form_field_id|string|Captures the ID of each field contained on a form.||||||||
|event_data.form_field_position|string|Captures the numeric position of each form field within a form \(i.e. 1, 2, 3\).|1, 2, 3, 4, 5||||1|||
|event_data.form_field_section|string|Captures the section containing each form field \(i.e. CC Info, Address\).|address1, address2, cc info, terms acceptance|||||||
|event_data.identifier|string|Captures the unique ID of the form.|F-0113, 2543, CU001, PI-0988|||||||
|event_data.name|string|Captures the human-friendly name of the form.|Payment Info, Mailing Address, Payment Address, Contact Us|||||||
|event_data.type|string|Captures the type of form \(i.e. demo, free trial, contact us\).|Address, Contact, Comment, Review, Payment|||||||




