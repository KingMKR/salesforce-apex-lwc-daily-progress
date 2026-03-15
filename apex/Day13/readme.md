Problem: Build a Generic Trigger Framework

Salesforce best practice is to avoid writing business logic inside triggers.
Instead, build a reusable trigger framework that can support multiple objects.

Requirements

Create a Generic Trigger Framework that:

1️⃣ Handles all trigger events

before insert

before update

before delete

after insert

after update

after delete

after undelete

2️⃣ Uses a Base Trigger Handler Class

3️⃣ Allows developers to extend the base class for each object.

Example:

AccountTriggerHandler extends BaseTriggerHandler
OpportunityTriggerHandler extends BaseTriggerHandler

4️⃣ Prevents recursive trigger execution

5️⃣ Keeps triggers one line only