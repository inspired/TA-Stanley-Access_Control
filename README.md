# TA-Stanley-Access_Control
Splunk TA for Stanley Access Control Logs retrieved from database with DB Connect

## Sample event

<pre>
"2016-10-03 14:46:14" TxnID="12314123", DeviceType="82", ChainID="12", NodeAddress="01", DoorControlUnitID="1", DeviceNumber="0", AlarmEventType="0", DeviceID="38", NumberRepeats="0", DateTimeOfTxn="2016-10-03 14:46:14.0", DateTimeOfLastRepeat="NULL", DateTimeOfReception="2016-10-03 14:46:19.0", DateTimeOfProcessing="2016-10-03 14:46:19.0", CompanyID="1", CompanyName="ACME", WhereName="1-1-5000", PatrolTourID="0", ResponseMnemonic="17232", TxnConditionName="Wrong PIN [10191919]", AlarmPriority="30", AlarmColour="255", AlarmInstructionText="NULL", CustomerCodeNumber="1000", CardNumber="-128128128", FirstName="Ola", LastName="Nordmann", AckedFlag="0", AckedUserName="NULL", AckedDateTime="NULL", ResetFlag="0", ResetDateTime="NULL", ClearedFlag="0", ClearedUserName="NULL", ClearedDateTime="NULL", ClearedAtMachine="NULL", CommentFlag="0", MachineID="0", MachinePort="0", TimeBefore="0", TimeAfter="0", MachineDateTime="2016-10-03 14:46:14.0", EmployeeNumber="890005", VisitorCard="0", AckedTimeZoneCode="NULL", ClearTimeZoneCode="NULL", RegionID="NULL", APTransactionID="0", SubDeviceType="0", SubDeviceID="0", DriverID="0", CardID="953121", HasVideo="0"
</pre>

## Inputs

Set up DB Connect to read your Access Control logs using TxnID as the incrementing field. Set the sourcetype as "access-log"
