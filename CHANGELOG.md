# Version: 2.0

New:
- define tetraCallId as typeTetraCallId(xs:string) to avoid problems with signed/unsigned long from TCS-API
- new OPTIONAL element "targetIsGroup" in typeSds
- make alias and orgBlockId OPTIONAL in typeRadio, because this type is used also in request, so the Df-Client doesn't have to know
- change group element type in typeGroupAppMemberEvent to typeSubscriberAddress, to unify it with other group event types