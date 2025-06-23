# cm1k-scraper

This program is designed to scrape the DOCSIS Status page of 
a Netgear CM1000 modem to pull the QAM, Upload, and OFDM channel
status tables. This will allow you to monitor the correctable and
uncorrectable codewords over time. When data is pulled, this program
automatically rounds to the nearest 30 minutes. For example, if you run
at 12:35PM, the timestamp will be 12:30PM. It is recommended to 
only run this once every 30 minutes. 
    
The default url, username/password will work for any factory modem.
Change the output folder under the Settings section, run it,
and three csv files will be produced for the QAM, OFDM, and Upload
channels.

| Output    | Description |
| --------- | ----------- |
| df_qam_channel_statusl.csv    | QAM channel status table    |
| df_upload_channel_status.csv  | Upload channel status table |
| df_ofdm_channel_status.csv    | OFDM channel status table   |
