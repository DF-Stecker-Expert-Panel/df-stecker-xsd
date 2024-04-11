# Version: 1.2

Fix:
- make alias and orgBlockId OPTIONAL in typeRadio, because this type is used also in request, so the Df-Client doesn't have to know
- change group element type in typeGroupAppMemberEvent to typeSubscriberAddress, to unify it with other group event types
---
# Version: 1.1.1

Fix:
- [#CR-92] add missing Call_Response into DR-GW-Interface/DR-GW-Call.Events