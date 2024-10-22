JDK: 17

Task: Fix the issues shown in 2 unit tests (CampaignStatServiceTest)

Updates in the getSPCampaignsStatistics method
The method now includes a check for existing campaign statistics:

If statistics for a campaign already exist, the new report is added to the existing one using the add() method.
If there are no existing statistics, a new object is created based on the current report.
