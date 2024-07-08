# Version: 1.2

New:
- added Management interface to deal with NEM-API(Tactilon-API) needs
- added txCoverageInfo element to give ability to inform clients about "transmission coverage information in a group call."
- changed DR-GW-Interface/DR-GW-Radio.CommonTypes typeRadioTrackingData.dmoState from xs:boolean to enum typeDmoState
- DR-GW-Interface/DR-GW-SDS.CommonTypes typeSDSValidity was not used, now typeSDS.validity is of type typeSDSValidity

Fix:
- make alias and orgBlockId OPTIONAL in typeRadio, because this type is used also in request, so the Df-Client doesn't have to know
- change group element type in typeGroupAppMemberEvent to typeSubscriberAddress, to unify it with other group event types
---
# Version: 1.1.1

Fix:
- [#CR-92] add missing Call_Response into DR-GW-Interface/DR-GW-Call.Events