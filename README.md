# ABAP-Serial-Port---AT-COMMAND
SAP ABAP Serial Port - AT COMMAND
ABAP Retrieve data from USB GSM Modem
Step by step:
1. Register/activate ActiveX component MSCOMM32.OCX on Windows 7 
Tutorial:
https://blogs.sap.com/2014/10/02/how-to-registeractivate-activex-component-mscomm32ocx-on-windows-7/
2. Create ABAP Z program.
3. Create New Screen with Custom Control (for text area) 
4. Test ABAP Z program with AT COMMAND

Note:
1. Please close Putty apps while you test AT COMMAND in the ABAP Z program.
2. Send SMS AT COMMAND by sequence:
AT+CSCS="GSM"
AT+CMGF=1
AT+CMGS="+628561811XXX" <CR> <message> <Ctrl+Z>
Remark: <CR> = Carriage Return (Enter)
   
 
Reference:
1. https://blogs.sap.com/2013/07/10/read-comm-port-using-abap-wo-third-party-software/
2. https://blogs.sap.com/2014/10/02/how-to-registeractivate-activex-component-mscomm32ocx-on-windows-7/
3. https://avtech.com/articles/65/how-to-test-a-gsm-modem-manually/
