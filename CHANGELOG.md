# Version: 1.2

New:
- [#CR-93] added Management interface to deal with NEM-API(Tactilon-API) needs
- [#CR-93] added txCoverageInfo element to give ability to inform clients about "transmission coverage information in a group call."
- [#CR-93] changed DR-GW-Interface/DR-GW-Radio.CommonTypes typeRadioTrackingData.dmoState from xs:boolean to enum typeDmoState
- [#CR-93] DR-GW-Interface/DR-GW-SDS.CommonTypes typeSDSValidity was not used, now typeSDS.validity is of type typeSDSValidity
- [#CR-93] DR-GW-Interface/CommonTypes typeSourceSystem new enumeration TACTILON-API
- [#CR-93] DR-GW-Interface/DR-GW-SDS.CommonTypes typeSDS new element "shortFormReportAllowed" + corresponding DR-GW-Interface/DR-GW-SDS method SDS_SendShortFormReport()
- [#CR-98] new OPTIONAL element "talkingPartyBasestationId" within DR-GW-Interface/DR-GW-Call.CommonTypes\typeTxGranted to be able to inform over which TBS the talking party currently speaks(LS1 VoIP)
- [#CR-99] added Recording interface to support Archive recording API needs

Fix:
- make alias and orgBlockId OPTIONAL in typeRadio, because this type is used also in request, so the Df-Client doesn't have to know
- change group element type in typeGroupAppMemberEvent to typeSubscriberAddress, to unify it with other group event types
- [#CR-GH-105] DR-GW-Group/DR-GW-Group limit group subscription requests to a single group per request.
---
# Version: 1.1.1

Fix:
- [#CR-92] add missing Call_Response into DR-GW-Interface/DR-GW-Call.Events