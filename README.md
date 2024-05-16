# What is SetupAuditTrail-SCH-SendPriorDayEntriesEmail?

Glad you asked! 

SetupAuditTrail-SCH-SendPriorDayEntriesEmail is a repo that includes a scheduled flow whose purpose is to 
run daily and get all SetupAuditTrail record entries from the prior day and send them via email to the designated recipient.

For the purpose of demonstration, a custom label is included with the recipient address which the flow targets for the daily send. This can be modified for more suitable use cases as needed within the flow or using custom metadata. 

Special thanks to ForcePanda for his [article](forcepanda.wordpress.com/2021/03/23/how-to-send-table-in-emails-via-flow) on sending a table in emails in flow!

The below installation links are also available to install as an unlocked package:

Install in [Sandbox](test.salesforce.com/packaging/installPackage.apexp?p0=04tU1000000LFNRIA4).

Install in [Production](login.salesforce.com/packaging/installPackage.apexp?p0=04tU1000000LFNRIA4).

# Why create this and make it available?

The SetupAuditTrail object contains valuable insights into org changes that require 'pull' effort (read SOQL to Excel) to visualize (read additional spend for Event Monitoring, etc). 

This simple automation delivers a daily email to recipient(s) with a tabular list of SetupAuditTrail entries. The flow is expandible to include additional filters or other modifications that apply to your use case.

# Why scheduled automation?

SetupAuditTrail only supports query and retrieve calls. Record-triggered automation is not currently supported.